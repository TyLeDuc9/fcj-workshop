---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# Introducing Open Source Skills for AWS SDK Best Practices

We have released a collection of AWS SDK Skills as part of the Open Source Agent Toolkit for AWS. These are artificial intelligence skills that help coding agents follow AWS SDK best practices. The project is available on GitHub under the Apache-2.0 license.

---

## 1. Problem

AI coding agents understand the general structure of using AWS SDKs, but they often make mistakes in the implementation details. They generate incorrect API names, use invalid parameter types, and fail to utilize SDK-specific features such as paginators, waiters, and high-level APIs like the Amazon Simple Storage Service (Amazon S3) Transfer Manager. These issues are particularly common in newer SDKs such as AWS SDK for Swift, where generated code may appear correct but fails to compile.

As developers increasingly rely on AI coding agents to generate AWS SDK code, it is essential to ensure that these agents produce code that compiles successfully, follows best practices, and uses each SDK as intended.

## 2. What Are Skills?

Skills are modular packages that provide AI coding agents with specialized knowledge about AWS SDKs. Each skill is developed by the SDK team responsible for a specific programming language and is based on common mistakes AI agents make when working with that SDK.

A skill typically includes:

- **`SKILL.md`**
  - Contains core instructions.
  - Includes SDK usage patterns.
  - Provides practical examples.

- **`references/`**
  - Contains reference materials for advanced topics.
  - Loaded only when necessary.

- **`scripts/`**
  - Contains automation scripts for:
    - Build
    - Test
    - Validation

Skills are designed independently of any coding agent, allowing them to work with any AI agent that supports the **Open Skill Format**.

## 3. How Skills Prevent Common Errors

Skills help AI coding agents avoid common mistakes when working with AWS SDKs, ranging from compilation errors to performance and exception-handling issues.

### 3.1. Code That Fails to Compile

This is the most common issue when working with newer SDKs because the AI agent's training data may be limited or outdated.

For example, with **AWS SDK for Swift**, AI agents often generate the following code:

```swift
let client = S3Client()
let response = client.listBuckets(input: ListBucketsInput())
```

The above code does not compile because:

- `S3Client()` is an `async throws` initializer.
- `listBuckets()` is also an `async throws` function.

After installing the Swift skill, the agent generates the correct code:

```swift
let config = try await S3Client.S3ClientConfig(region: "us-west-2")
let client = S3Client(config: config)
let response = try await client.listBuckets(input: ListBucketsInput())
```

As a result, the generated code compiles successfully and works correctly from the first attempt.

---

### 3.2. Code That Runs but Performs Poorly

Some AI agents generate code that functions correctly but does not take advantage of AWS SDK optimization features, such as:

- Not using **Paginator** for APIs like `ListObjects`.
- Not using **Waiter** to monitor resource status.
- Not using high-level methods such as:
  - `upload_file`
  - `download_file`

This can lead to:

- Retrieving only the first page of results.
- Making unnecessary API calls.
- Ignoring multipart upload capabilities.
- Poor performance when processing large datasets.

Once the appropriate skill is installed, the AI agent automatically applies these SDK features to improve both performance and cost efficiency.

---

### 3.3. Code That Runs but Contains Subtle Bugs

Some issues are difficult to detect, for example:

- Manually converting DynamoDB data types such as:

```json
{"S": "value"}
```

- Catching overly generic exceptions (`Exception`) instead of specific exceptions like:

```text
ConditionalCheckFailedException
```

After installing the skill, the AI agent will:

- Use the **Document Client** for automatic data conversion.
- Catch the correct exception type for each API.
- Significantly reduce subtle logic errors.

---

## 4. Measuring Effectiveness

Each skill is evaluated using a comprehensive test suite covering real-world development tasks such as:

- Working with Amazon S3.
- Querying Amazon DynamoDB.
- Configuring SDK clients.
- Generating presigned URLs.
- Managing credentials.

Generated code is evaluated based on:

- Whether it compiles successfully.
- Whether it passes linting.
- Whether it satisfies the task requirements.

Each test is executed twice:

1. Without the skill installed.
2. With the skill installed.

The results demonstrate that code generated with Skills consistently passes more tests and achieves higher overall quality.

---

## 5. Available Skills

| Skill | SDK | Description |
|--------|-----|-------------|
| `aws-sdk-swift-usage` | AWS SDK for Swift | Asynchronous programming patterns, client configuration, client initialization |
| `aws-sdk-js-v3-usage` | AWS SDK for JavaScript v3 | Package structure, Client, Middleware, Runtime Authentication |
| `aws-sdk-python-usage` | Boto3 / Botocore | Client, Resource, Paginator, Waiter, and exception handling |

---

## 6. Getting Started

To install a Skill using the **AWS Agent Toolkit**, run:

```bash
npx skills add aws/agent-toolkit-for-aws/skills --skill <skill>
```

Replace `<skill>` with the desired skill name, for example:

- `aws-sdk-swift-usage`
- `aws-sdk-js-v3-usage`
- `aws-sdk-python-usage`

The `--skill` option can be specified multiple times to install several skills simultaneously.

## 7. Key Takeaways

The article highlights several important lessons:

- AI coding agents require specialized knowledge through **Skills** to use AWS SDKs correctly.
- Skills significantly reduce compilation errors, logic errors, and performance issues in generated code.
- Leveraging built-in AWS SDK features such as **Paginator**, **Waiter**, and **Document Client** helps generated code follow AWS best practices.
- Using Skills saves developers time by reducing debugging efforts and improving the quality of AI-generated code.

## 8. Applications

Skills can be applied in many software development scenarios, including:

- Assisting AI coding agents in generating accurate AWS SDK code.
- Developing applications using Amazon S3, Amazon DynamoDB, and other AWS services.
- Helping new developers quickly become familiar with AWS SDKs.
- Improving software development productivity while reducing maintenance costs.
- Supporting AI-powered coding tools such as Amazon Q Developer, GitHub Copilot, and other coding agents that support the Open Skill Format.

## 9. Conclusion

- Skills play an essential role in improving the quality of AI-generated code when working with AWS SDKs. By providing implementation guidance, practical examples, and best practices, they help reduce compilation errors, improve runtime performance, and minimize subtle logic bugs.
- In addition, Skills enable AI coding agents to correctly leverage AWS SDK features such as Paginator, Waiter, Document Client, and high-level transfer APIs, resulting in code that is accurate, efficient, and aligned with AWS best practices.
- Overall, installing and using Skills is an important step toward enabling AI coding agents to help developers build AWS applications more quickly, more reliably, and with significantly less post-generation code correction.

## Original Article

https://aws.amazon.com/vi/blogs/developer/introducing-open-source-skills-for-aws-sdk-best-practices/