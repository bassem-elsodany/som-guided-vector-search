# Comprehensive Search Comparison Report

**Generated:** 2025-07-08T12:30:12.483939
**Collection:** SkillPilotDataSet_v7
**Total Queries:** 21


## Model & Search Parameters

### Trained SOM Model Parameters

| Parameter | Value | Description |
|-----------|-------|-------------|
| **Model Path** | som_output/som_model.pkl | Path to trained SOM model file |
| **Grid Size** | 25×25 | SOM grid dimensions (width × height) |
| **Model Loaded** |  Yes | Whether SOM model is successfully loaded |
| **Total Documents** | 11,412 | Total documents in collection |
| **Documents with SOM** | 1,000 | Documents with SOM cluster assignments |
| **Unique Clusters** | 346 | Number of unique clusters used |
| **Cluster Range** | 0-2420 | Range of cluster IDs |
| **Grid Coverage** | 346 | Number of grid positions with documents |
| **Avg Docs/Cluster** | 2.9 | Average documents per cluster |

### Optimized Search Parameters

| Parameter | Value | Description |
|-----------|-------|-------------|
| **Cluster Expansion Factor** | 3 | Number of top clusters to search in (optimized for 25×25 grid result coverage) |
| **Alpha (α)** | 0.10 | Weight factor for combining semantic and topological scores |
| **Search Strategy** | 25×25 Grid | Maximum performance configuration for enhanced SOM |
| **Traditional Alpha** | 0.5 | Weight for traditional hybrid search (vector vs keyword) |
| **Results per Query** | 3 | Number of results returned per search |

### Parameter Optimization History

- **Initial Grid**: 50×50 (over-clustered, poor performance)
- **Second Grid**: 6×6 (good coverage, limited granularity)
- **Final Grid**: 15×15 (optimal balance of coverage and granularity)
- **Expansion Factor**: Optimized from 2→3 for better overlap
- **Alpha**: Optimized from 0.7→0.20 for balanced semantic-topological scoring

## Executive Summary

| Metric | Traditional | SOM-Enhanced | Improvement |
|--------|-------------|--------------|-------------|
| Avg Duration | 0.874s | 1.669s | 0.60x |
| Avg Score | 0.014 | 0.023 | 68.8% |
| Clusters Used | 5.4 | 1.5 | 253.1% reduction |
| Result Overlap | - | - | 32.4% |

## Performance Analysis

- **Average Traditional Search Duration:** 0.874 seconds
- **Average SOM-Enhanced Search Duration:** 1.669 seconds
- **Average Speedup:** 0.60x
- **Performance Improvement:** -47.6%

## Quality Analysis

- **Average Traditional Score:** 0.014
- **Average SOM Score:** 0.023
- **Average Result Overlap:** 32.4%
- **Jaccard Similarity:** 0.218

## Cluster Analysis

- **Total Traditional Clusters Used:** 73
- **Total SOM Clusters Used:** 22
- **Cluster Efficiency:** 7.38 results/cluster
- **Cluster Reduction:** 231.8%

## Detailed Query Results

### Query 1: How do I configure OAuth2 authentication?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 1.338s | 2.101s |
| Results Count | 10 | 10 |
| Clusters Used | 6 | 2 |
| Avg Score | 0.013 | 0.056 |
| Overlap | - | 20.0% |

**Performance:** SOM-enhanced search is 0.64x faster

**Cluster Usage:** Traditional used clusters [209, 1012, 309, 1204, 314, 2108], SOM used clusters [314, 1014]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 314 | mulesoft | https://docs.mulesoft.com/oauth2-provider-module/latest | # OAuth2 Provider Module 1.2<br>The OAuth2 Provider module enables a Mule runtime engine (Mule) app to be configured as an Authentication Manager in an OAuth2 dance. With this role, the application can authenticate to previously registered clients, grant tokens, validate tokens, or register and delete clients, all during the execution of a flow.<br>The following documentation assumes a basic knowledge of the OAuth2 authorization protocol. For further reference, see the RFC-6749.<br>... |
| **SOM-Enhanced** | 0.061 | 1014 | mulesoft | https://docs.mulesoft.com/connectors/introduction/intro-config-oauth2 | 6. Run the app.<br><br><br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 2108 | mulesoft | https://docs.mulesoft.com/oauth2-provider-module/latest/oauth2-provider-module-reference | # OAuth2 Provider Module 1.2 Reference<br>The OAuth2 Provider module allows a Mule runtime engine (Mule) app to be configured as an Authentication Manager in an OAuth2 dance. With this role, the application will be able to authenticate previously registered clients, grant tokens, validate tokens, or register and delete clients, all during the execution of a flow.<br>## Configurations<br>... |
| **SOM-Enhanced** | 0.061 | 1014 | mulesoft | https://docs.mulesoft.com/connectors/introduction/intro-config-oauth2-cloudhub | ## Performing the OAuth Dance<br>After you complete the OAuth 2.0 configuration, you can deploy your app to CloudHub and initialize the OAuth dance by navigating to your public hostname on your authorization endpoint. For example, with the previous configuration, you can navigate to `{ch-app-name}.{region}.cloudhub.io/authorize`. This starts the OAuth dance and prompts you to log in with your OAuth provider.<br>## See Also<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 314 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/mule-secure-token-service | # Mule Secure Token Service OAuth 2.0<br>The Mule runtime engine supports the OAuth 2.0 protocol. The way to configure OAuth 2.0 authorization differs, depending on the OAuth role and your objective:<br>* Configure authentication in your client Mule app when sending requests to a service that requires authentication, such as the Github OAuth2 server. Use the OAuth Module for the OAuth2 configuration.<br>... |
| **SOM-Enhanced** | 0.061 | 1014 | mulesoft | https://docs.mulesoft.com/microsoft-dynamics-365-connector/latest/microsoft-dynamics-365-connector-studio | The following image shows an example OAuth client credentials configuration using property placeholder values:<br>### OAuth 2.0 Username and Password Authentication<br>With OAuth 2.0 username and password authentication, the app makes a POST request that includes a username and password. If the credentials are valid, the server returns an access token.<br>... |

#### Overlap Analysis

- **Overlapping Results:** 2/10 (20.0%)
- **Jaccard Similarity:** 0.111

---

### Query 2: What are the best practices for API security?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.974s | 1.169s |
| Results Count | 10 | 10 |
| Clusters Used | 7 | 1 |
| Avg Score | 0.009 | 0.007 |
| Overlap | - | 10.0% |

**Performance:** SOM-enhanced search is 0.83x faster

**Cluster Usage:** Traditional used clusters [2213, 2024, 2411, 813, 209, 309, 701], SOM used clusters [209]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.012 | 209 | mulesoft | https://docs.mulesoft.com/release-notes/anypoint-security/anypoint-security-release-notes | # Anypoint Security Release Notes<br>Anypoint Security provides a layered approach to secure your application network. These layers work together to protect both the application network and its individual nodes by controlling access to APIs, enforcing policies, and proxying all inbound or outbound traffic to mitigate external threats.<br>These capabilities are optimized for security, providing you with a dedicated endpoint to detect attacks and validate traffic without taxing your implementations.<br>... |
| **SOM-Enhanced** | 0.007 | 209 | mulesoft | https://docs.mulesoft.com/api-manager/latest/api-proxy-landing-page | # Configure Proxies for Your APIs<br>Protect your APIs or web services against attacks by using API proxies, which function as intermediaries between the external applications and the backend server. The API proxy is agnostic to your backend’s location and programming language. Additionally, your backend can be a non-Mule application.<br>When you deploy an API proxy in front of your API, the proxy adopts API gateway capabilities to secure the API by using different types of policies. Anypoint Platform enables you to deploy the proxy application directly to CloudHub or Anypoint Runtime Fabric. Your proxy application is then automatically tracked by API Manager.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.011 | 2213 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/hardening-your-mule-installation | For instructions specific to Runtime Fabric, see Hardening Mule Runtime on Runtime Fabric.<br>### About Running Mule as a Non-Privileged User<br>On Linux and Unix, you can run Mule as any user with the following caveats:<br>... |
| **SOM-Enhanced** | 0.007 | 209 | mulesoft | https://docs.mulesoft.com/api-manager/latest/api-proxy-landing-page | # Configure Proxies for Your APIs<br>Protect your APIs or web services against attacks by using API proxies, which function as intermediaries between the external applications and the backend server. The API proxy is agnostic to your backend’s location and programming language. Additionally, your backend can be a non-Mule application.<br>When you deploy an API proxy in front of your API, the proxy adopts API gateway capabilities to secure the API by using different types of policies. Anypoint Platform enables you to deploy the proxy application directly to CloudHub or Anypoint Runtime Fabric. Your proxy application is then automatically tracked by API Manager.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.010 | 209 | mulesoft | https://docs.mulesoft.com/mcp-connector/latest/mcp-connector-studio | ### Best Practices for MCP Policies<br>* Always apply authentication policies to production MCP servers.<br>* Use logging policies to track MCP client activity.<br>... |
| **SOM-Enhanced** | 0.007 | 209 | mulesoft | https://docs.mulesoft.com/api-manager/latest/api-proxy-landing-page | # Configure Proxies for Your APIs<br>Protect your APIs or web services against attacks by using API proxies, which function as intermediaries between the external applications and the backend server. The API proxy is agnostic to your backend’s location and programming language. Additionally, your backend can be a non-Mule application.<br>When you deploy an API proxy in front of your API, the proxy adopts API gateway capabilities to secure the API by using different types of policies. Anypoint Platform enables you to deploy the proxy application directly to CloudHub or Anypoint Runtime Fabric. Your proxy application is then automatically tracked by API Manager.<br>... |

#### Overlap Analysis

- **Overlapping Results:** 1/10 (10.0%)
- **Jaccard Similarity:** 0.053

---

### Query 3: How to implement JWT token validation?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.752s | 3.602s |
| Results Count | 10 | 10 |
| Clusters Used | 1 | 1 |
| Avg Score | 0.015 | 0.106 |
| Overlap | - | 90.0% |

**Performance:** SOM-enhanced search is 0.21x faster

**Cluster Usage:** Traditional used clusters [2413], SOM used clusters [2413]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 2413 | mulesoft | https://docs.mulesoft.com/gateway/latest/policies-included-jwt-validation | # JWT Validation Policy<br>**Policy name** |  JWT Validation<br>---|---<br>... |
| **SOM-Enhanced** | 0.106 | 2413 | mulesoft | https://docs.mulesoft.com/pdk/latest/policies-pdk-configure-features-jwt | The `SigningKeyLength` enum defines the available signing key lengths:<br>```<br>pub enum SigningKeyLength {<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 2413 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-jwt-validation | # JWT Validation Policy<br>**Policy name** |  JWT Validation<br>---|---<br>... |
| **SOM-Enhanced** | 0.106 | 2413 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-jwt-validation | Element | Description | Example<br>---|---|---<br>Specifies from where in the request to extract the JWT:<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 2413 | mulesoft | https://docs.mulesoft.com/gateway/latest/policies-included-jwt-validation | JWKS URL | This field appears if you selected the **JWKS** method as JWT Key Origin. Ignore this field if you selected **none** as JWT Signing Method. | JWKS server URLs that contain the public keys for the signature validation. Configure multiple JWKS servers with a comma-separated list of the URLs.<br>JWKS Caching Time To Live | Amount of time, in minutes, that the JWKS is valid. When the JWKS expires, the policy retrieves the JWKS from each JWKS server again. The default value is 60 minutes. Ignore this field if you selected **none** as JWT Signing Method. | This field input is the amount of time, in minutes, during which the policy considers the JWKS valid.<br>JWKS Service connection timeout (milliseconds) | Maximum time, in milliseconds, to wait for a response from each JWKS service when authenticating the access token validation endpoint. The default value is 10 seconds.<br>... |
| **SOM-Enhanced** | 0.106 | 2413 | mulesoft | https://docs.mulesoft.com/pdk/latest/policies-pdk-configure-features-jwt | # Using JWT Library Functions<br>To view an example policy project that uses Flex Gateway Policy Development Kit (PDK)'s JWT library, see JWT Validation Policy Example.<br>---<br>... |

#### Overlap Analysis

- **Overlapping Results:** 9/10 (90.0%)
- **Jaccard Similarity:** 0.818

---

### Query 4: How to create a REST API endpoint?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.478s | 1.052s |
| Results Count | 10 | 10 |
| Clusters Used | 8 | 1 |
| Avg Score | 0.014 | 0.014 |
| Overlap | - | 20.0% |

**Performance:** SOM-enhanced search is 0.45x faster

**Cluster Usage:** Traditional used clusters [1800, 424, 1900, 2220, 209, 309, 503, 922], SOM used clusters [503]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1800 | mulesoft | https://docs.mulesoft.com/general/api-led-deploy | 3. In Advanced Rest Client, send a request to the base URI that you just copied. Be sure to add the API endpoint `/api/greeting`:<br>```<br>GET http://hello-world-greeting.sandy-kim.us-e2.cloudhub.io/api/greeting<br>... |
| **SOM-Enhanced** | 0.014 | 503 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-gateway-k8-getting-started | ## Step 5: Publish and Deploy a Simple API to Flex Gateway<br>Create and deploy a simple API to your gateway in Anypoint API Manager:<br>1. In Runtime Manager, click the **View APIs** menu option for your gateway to navigate to its **View APIs** page.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 209 | mulesoft | https://docs.mulesoft.com/apikit/latest/apikit-4-implement-rest-api | # Building, Implementing, and Testing a REST API<br>This workflow guides you through the process of designing, implementing, and testing a REST API.<br>For example purposes, this workflow uses the free online REST service {JSON} Placeholder, which provides mocked user information in JSON format.<br>... |
| **SOM-Enhanced** | 0.014 | 503 | mulesoft | https://docs.mulesoft.com/api-manager/latest/getting-started-proxy | # Getting Started with Managing an API<br>You can use API Manager to apply policies and to add contracts, alerts, and SLA tiers to your API instance. Additionally, you can configure a runtime for your API that runs in CloudHub or CloudHub 2.0. Although you can also deploy your API runtime using Mule runtime engine (Mule) and Hybrid, deploying your API proxy directly to CloudHub is the fastest and easiest.<br>If you are running an API with a standalone server, use the classic API creation flows to manage your API.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 922 | mulesoft | https://docs.mulesoft.com/exchange/publish-an-http-api | # Publish an HTTP API Asset<br>The HTTP API enables Exchange users specify a placeholder for an endpoint. After you create the HTTP API endpoint, you can optionally manage the endpoint with API Manager.<br>The HTTP API asset describes what the API endpoint does and how users can connect the API to their programs.<br>... |
| **SOM-Enhanced** | 0.014 | 503 | mulesoft | https://docs.mulesoft.com/api-manager/latest/create-instance-task-flex | * Click **Create new API** :<br>1. Enter a **Name** for the new API asset.<br>2. Select the **Asset type** from the following options:<br>... |

#### Overlap Analysis

- **Overlapping Results:** 2/10 (20.0%)
- **Jaccard Similarity:** 0.111

---

### Query 5: What is the difference between SOAP and REST?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.737s | 1.475s |
| Results Count | 10 | 10 |
| Clusters Used | 7 | 1 |
| Avg Score | 0.014 | 0.006 |
| Overlap | - | 10.0% |

**Performance:** SOM-enhanced search is 0.50x faster

**Cluster Usage:** Traditional used clusters [1920, 424, 105, 618, 1008, 209, 208], SOM used clusters [209]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 424 | mulesoft | https://docs.mulesoft.com/apikit/latest/apikit-4-for-soap | # APIkit for SOAP<br>APIkit for SOAP is a framework for simplifying the development and integration of SOAP-based APIs. SOAP (Simple Object Access Protocol) is a messaging protocol for exchanging structured information between web services. APIkit for SOAP manages SOAP message formats and headers to ensure seamless integration with SOAP infrastructure. With APIkit for SOAP, you can create robust and reliable SOAP-based APIs, accelerating your development workflow and delivering enhanced integration capabilities.<br>## APIkit for SOAP Features<br>... |
| **SOM-Enhanced** | 0.006 | 209 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-troubleshoot-soap-apis | # Troubleshooting SOAP APIs<br>Flex Gateway does not natively support SOAP APIs and does not provide any schema validation for XML. However, you can publish an HTTP API instance to a secure SOAP upstream service.<br>To create an HTTP API instance to a secure SOAP API upstream service, refer to the following:<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 208 | mulesoft | https://docs.mulesoft.com/api-manager/latest/building-soap-proxy | # Build SOAP API Proxies<br>API Manager 2.x enables you to use SOAP API proxies for your SOAP-based web services. The SOAP proxy requires a WSDL definition that describes the backend service. The WSDL defines how the API proxy must perform validations on incoming requests and correctly routes outbound requests for the corresponding API endpoint.<br>## SOAP Proxy Schema Validation<br>... |
| **SOM-Enhanced** | 0.006 | 209 | mulesoft | https://docs.mulesoft.com/api-manager/latest/proxy-advantages | # Reviewing API Proxy Benefits and Impacts<br>The tables below describe the main benefits and impacts of implementing the different types of API Proxies.<br>## Benefits<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 209 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-troubleshoot-soap-apis | # Troubleshooting SOAP APIs<br>Flex Gateway does not natively support SOAP APIs and does not provide any schema validation for XML. However, you can publish an HTTP API instance to a secure SOAP upstream service.<br>To create an HTTP API instance to a secure SOAP API upstream service, refer to the following:<br>... |
| **SOM-Enhanced** | 0.006 | 209 | mulesoft | https://docs.mulesoft.com/api-manager/latest/api-proxy-landing-page | ## How API Proxies Work<br>The API proxy intercepts incoming API requests, and can provide authentication, rate limiting, request and response transformation, and logging features.<br>When a client application sends a request to your backend API, the request is first intercepted by the API proxy. The proxy applies policies for the requested backend API, and the policies determine whether, and how, to forward the request to your backend API.<br>... |

#### Overlap Analysis

- **Overlapping Results:** 1/10 (10.0%)
- **Jaccard Similarity:** 0.053

---

### Query 6: How to handle API rate limiting?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.935s | 1.316s |
| Results Count | 10 | 10 |
| Clusters Used | 3 | 2 |
| Avg Score | 0.015 | 0.019 |
| Overlap | - | 70.0% |

**Performance:** SOM-enhanced search is 0.71x faster

**Cluster Usage:** Traditional used clusters [1512, 1316, 1423], SOM used clusters [1512, 1423]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1316 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-rate-limiting | # Rate Limiting Policy<br>**Policy name** |  Rate Limiting<br>---|---<br>... |
| **SOM-Enhanced** | 0.021 | 1423 | mulesoft | https://docs.mulesoft.com/gateway/latest/policies-included-rate-limiting-sla | In the first window, because the quota is reached with the third request, all subsequent requests are rejected until the window closes. In the second window, only two of the three requests are processed. Because the time elapses in this window, the remaining quota is unused.<br>An accepted request passes through the API to the backend. Conversely, a rejected request displays a `429 status for HTTP` (or 400, or 500 if the API is WSDL) and does not reach the backend.<br>* Requests of Client with ID “ID#2”:<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1512 | mulesoft | https://docs.mulesoft.com/gateway/latest/policies-included-rate-limiting | By default, the X-RateLimit headers are disabled in the response. You can enable these headers by selecting **Expose Headers** when you configure the policy.<br>**When should I use Rate Limiting instead of Rate-Limiting SLA or Spike Control?**<br>Use Rate Limiting and **Rate-Limiting SLA** policies for accountability and to enforce a hard limit to a group (using the identifier in Rate Limiting) or to a client application (using **Rate-Limiting SLA**). If you want to protect your backend, use the **Spike Control** policy instead. |
| **SOM-Enhanced** | 0.021 | 1423 | mulesoft | https://docs.mulesoft.com/gateway/latest/policies-included-spike-control | Queuing a request requires retaining a thread and an HTTP connection. When you specify a `Queuing Limit` for the policy, the parameter protects the gateway from running out of resources and ensures that the API does not fail in case of an attack.<br>## Request Timelines<br>The following diagram illustrates the lifespan of each request accepted by the algorithm, using the configuration defined in the previous section:<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1512 | mulesoft | https://docs.mulesoft.com/gateway/latest/policies-included-rate-limiting-sla | By default, the X-RateLimit headers are disabled in the response. You can enable these headers by selecting **Expose Headers** when you configure the policy.<br>When on distributed mode, the X-Ratelimit-Remaining header is not perfectly synchronized with all the replicas. With multiple replicas on distributed mode, the X-Ratelimit-Remaining header is an estimation of how much quota the replica has available for itself. It does not represent the actual value of the remaining quota available for the API. The following describes a valid scenario:<br>* Created a SLA tier name "Titanium" having rate limit of "999999999 req per 10 min"<br>... |
| **SOM-Enhanced** | 0.021 | 1423 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-spike-control | Queuing a request requires retaining a thread and an HTTP connection. When you specify a `Queuing Limit` for the policy, the parameter protects the gateway from running out of resources and ensures that the API does not fail in case of an attack.<br>## Request Timelines<br>The following diagram illustrates the lifespan of each request accepted by the algorithm, using the configuration defined in the previous section:<br>... |

#### Overlap Analysis

- **Overlapping Results:** 7/10 (70.0%)
- **Jaccard Similarity:** 0.538

---

### Query 7: How to optimize database queries?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.482s | 1.284s |
| Results Count | 10 | 10 |
| Clusters Used | 6 | 2 |
| Avg Score | 0.014 | 0.006 |
| Overlap | - | 30.0% |

**Performance:** SOM-enhanced search is 0.38x faster

**Cluster Usage:** Traditional used clusters [1601, 1706, 1808, 209, 309, 408], SOM used clusters [408, 309]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 209 | mulesoft | https://docs.mulesoft.com/datagraph/configure-apq-cdn | # Using Automatic Persisted Queries and Content Delivery Networks with Anypoint DataGraph<br>To improve performance and decrease potential bottlenecks in your network traffic, DataGraph supports automatic persisted queries. You can also use persisted queries in conjunction with content delivery networks (CDNs) to deliver cached results much faster than requiring a roundtrip to the DataGraph server.<br>## How Automatic Persisted Queries Work in DataGraph<br>... |
| **SOM-Enhanced** | 0.008 | 309 | mulesoft | https://docs.mulesoft.com/mongodb-connector/latest/mongodb-connector-upgrade-migrate | To optimize pagination and improve performance when migrating to MongoDB Connector 6.x, the following approaches are recommended:<br>* Avoid using `skip()` for large offsets.<br>Instead of using the **Num To Skip** field, it is more efficient to refine query conditions to exclude unwanted documents directly.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 309 | mulesoft | https://docs.mulesoft.com/mongodb-connector/latest/mongodb-connector-upgrade-migrate | To optimize pagination and improve performance when migrating to MongoDB Connector 6.x, the following approaches are recommended:<br>* Avoid using `skip()` for large offsets.<br>Instead of using the **Num To Skip** field, it is more efficient to refine query conditions to exclude unwanted documents directly.<br>... |
| **SOM-Enhanced** | 0.008 | 309 | mulesoft | https://docs.mulesoft.com/mule-sdk/latest/object-streaming | # Object Streaming (Pagination)<br>Object streaming is similar to binary streaming, except that it streams Java objects, not a raw byte stream.<br>Note that if you are familiar with the Devkit (for Mule 3), you can think of this feature as an evolution of the Auto Pagination feature. The main difference between this and Devkit is that the Mule SDK supports repeatable, random, and concurrent access.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 408 | mulesoft | https://docs.mulesoft.com/db-connector/latest | # Database Connector 1.14<br>Anypoint Connector for Database (Database Connector) establishes communication between your Mule app and a relational database. Database Connector can connect to almost any Java Database Connectivity (JDBC) relational database and run SQL operations. An application can support multi-tenant scenarios using the same configuration element, changing the connection attributes based on, for example, information coming from each request.<br>Database Connector has connection providers that automatically set the driver class name and create JDBC URLs with given parameters for the following databases:<br>... |
| **SOM-Enhanced** | 0.008 | 309 | mulesoft | https://docs.mulesoft.com/mongodb-connector/latest/mongodb-connector-upgrade-migrate | ## Removed Operations<br>The following operations were removed from the MongoDB connector:<br>Removed from MongoDB 5.x | Can be reproduced in MongoDB 6.0.0 through<br>... |

#### Overlap Analysis

- **Overlapping Results:** 3/10 (30.0%)
- **Jaccard Similarity:** 0.176

---

### Query 8: What are the different types of database indexes?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.811s | 1.503s |
| Results Count | 10 | 10 |
| Clusters Used | 5 | 2 |
| Avg Score | 0.013 | 0.005 |
| Overlap | - | 0.0% |

**Performance:** SOM-enhanced search is 0.54x faster

**Cluster Usage:** Traditional used clusters [1601, 1808, 1814, 408, 2301], SOM used clusters [309, 1007]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 1814 | mulesoft | https://docs.mulesoft.com/db-connector/latest/database-documentation | Indicates whether to create the database if it does not already exist<br>**Connection Properties** |  Specifies a list of custom key-value connection properties for the configuration<br>**Reconnection** |  |  When the application is deployed, a connectivity test is performed on all connectors. If set to `true`, deployment fails if the test doesn’t pass after exhausting the associated reconnection strategy.<br>... |
| **SOM-Enhanced** | 0.006 | 309 | mulesoft | https://docs.mulesoft.com/azure-cosmos-db-connector/latest | # Azure Cosmos DB Connector 1.0<br>Where possible, we changed noninclusive terms to align with our company value of Equality. We maintained certain terms to avoid any effect on customer implementations.<br>---<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 408 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/creating-and-managing-a-cluster-manually | The database’s tables are created automatically, as this feature creates tables for each different object store that you want to persist. Two tables are created per object store:<br>* One table stores data<br>* Another table stores partitions.<br>... |
| **SOM-Enhanced** | 0.006 | 309 | mulesoft | https://docs.mulesoft.com/composer/ms_composer_netsuite_reference | ## Record Types<br>The following record types are supported:<br>Record Type | Trigger | Action<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 408 | mulesoft | https://docs.mulesoft.com/db-connector/latest/database-connector-connection | 8. In **Global Elements** , click **Create** to open the **Choose Global Type** window.<br>9. In **Filter** , type `database`, select **Database Config** , and click **OK**.<br>10. In **Database Config** > **Connection** , select **Data Source Reference Connection**.<br>... |
| **SOM-Enhanced** | 0.006 | 309 | mulesoft | https://docs.mulesoft.com/mongodb-connector/latest/mongodb-connector-upgrade-migrate | To optimize pagination and improve performance when migrating to MongoDB Connector 6.x, the following approaches are recommended:<br>* Avoid using `skip()` for large offsets.<br>Instead of using the **Num To Skip** field, it is more efficient to refine query conditions to exclude unwanted documents directly.<br>... |

#### Overlap Analysis

- **Overlapping Results:** 0/10 (0.0%)
- **Jaccard Similarity:** 0.000

---

### Query 9: How to implement database connection pooling?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 1.037s | 1.271s |
| Results Count | 10 | 10 |
| Clusters Used | 2 | 1 |
| Avg Score | 0.015 | 0.044 |
| Overlap | - | 60.0% |

**Performance:** SOM-enhanced search is 0.82x faster

**Cluster Usage:** Traditional used clusters [408, 1814], SOM used clusters [408]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.017 | 408 | mulesoft | https://docs.mulesoft.com/db-connector/latest/database-connector-connection | ## Configure Connection Pools<br>Establishing connections is costly in terms of connectors, the relational database management system (RDBMS) network, and processing overhead. Database Connector supports the use of pooling profiles that enable you to build a connection pool. This is a group of established connections that the connector can use to perform required operations without having to establish new connections every time.<br>When you configure the **Pooling profile** field in the global element of your application, deselect the **Test connection on checkout** field to improve the connector performance with connection pooling. If you leave the field selected as default (`TRUE`), every time a connection is checked out of the pool, the connection pool performs connectivity checks against the database, which increases the time required for each operation to complete.<br>... |
| **SOM-Enhanced** | 0.044 | 408 | mulesoft | https://docs.mulesoft.com/db-connector/latest/database-connector-connection | ## Configure Connection Pools<br>Establishing connections is costly in terms of connectors, the relational database management system (RDBMS) network, and processing overhead. Database Connector supports the use of pooling profiles that enable you to build a connection pool. This is a group of established connections that the connector can use to perform required operations without having to establish new connections every time.<br>When you configure the **Pooling profile** field in the global element of your application, deselect the **Test connection on checkout** field to improve the connector performance with connection pooling. If you leave the field selected as default (`TRUE`), every time a connection is checked out of the pool, the connection pool performs connectivity checks against the database, which increases the time required for each operation to complete.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 408 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-pooling-profiles | # Pooling Profiles<br>Unlike singleton components, pooled components configure their component pool which contains multiple instances of the component to process simultaneous incoming requests. Each pooled component has its pooling profile.<br>Connectors such as Anypoint Connector for FTP (FTP Connector) and Anypoint Connector for SFTP (SFTP Connector) pool connections by default and use a `pooling-profile` to customize the connection pool. When performance tests show it necessary, add the `pooling-profile` parameter to connectors.<br>... |
| **SOM-Enhanced** | 0.044 | 408 | mulesoft | https://docs.mulesoft.com/db-connector/latest/database-documentation | |  The transaction isolation level to set on the driver when connecting the database |  `NOT_CONFIGURED`<br>**Use XA Transactions** |  Indicates whether or not the created datasource must support XA transactions<br>Configures the host of the database<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 1814 | mulesoft | https://docs.mulesoft.com/db-connector/latest/database-documentation | Indicates whether to create the database if it does not already exist<br>**Connection Properties** |  Specifies a list of custom key-value connection properties for the configuration<br>**Reconnection** |  |  When the application is deployed, a connectivity test is performed on all connectors. If set to `true`, deployment fails if the test doesn’t pass after exhausting the associated reconnection strategy.<br>... |
| **SOM-Enhanced** | 0.044 | 408 | mulesoft | https://docs.mulesoft.com/mule-sdk/latest/connections | Example of the XML for this config with the example `MyConnectionProvider`:<br>```<br><xyz:config name="a-xyz-config" someParameter="value"><br>... |

#### Overlap Analysis

- **Overlapping Results:** 6/10 (60.0%)
- **Jaccard Similarity:** 0.429

---

### Query 10: How to debug API errors?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.962s | 5.232s |
| Results Count | 10 | 10 |
| Clusters Used | 7 | 1 |
| Avg Score | 0.013 | 0.041 |
| Overlap | - | 20.0% |

**Performance:** SOM-enhanced search is 0.18x faster

**Cluster Usage:** Traditional used clusters [810, 1516, 209, 403, 309, 1302, 506], SOM used clusters [403]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.017 | 209 | mulesoft | https://docs.mulesoft.com/pdk/latest/policies-pdk-debug-deployed-policies | # Debugging Deployed Custom Policies<br>Errors that are not present in the PDK debugging playground or PDK’s integration might be present when the policy is applied to an API instance in a production environment.<br>To use debug logs in a production environment, see Troubleshooting Self-Managed Gateway with Debug Logs.<br>... |
| **SOM-Enhanced** | 0.041 | 403 | mulesoft | https://docs.mulesoft.com/design-center/design-troubleshooting | # Troubleshooting<br>Troubleshoot errors you recieve when using API Designer:<br>* Common Problems in Conforming to RAML 0.8<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 506 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-troubleshoot-debug-logs | # Troubleshooting Self-Managed Gateway with Debug Logs<br>When troubleshooting Flex Gateway, set the runtime log level to `debug` for more verbose runtime logs.<br>This page explains how to configure debug runtime logs. To configure debug access logs, set the `level` parameter in your Message Logging policy to `DEBUG`.<br>... |
| **SOM-Enhanced** | 0.041 | 403 | mulesoft | https://docs.mulesoft.com/datagraph/troubleshoot-schemas-queries | ## Troubleshooting Schema Errors<br>If you encounter runtime errors when attempting to generate an API schema, troubleshoot them as follows.<br>### Potential Errors When Generating an API Schema<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 1516 | mulesoft | https://docs.mulesoft.com/anypoint-code-builder/int-debug-mule-apps | # Debugging Mule Applications<br>Cloud IDE<br>Desktop IDE<br>... |
| **SOM-Enhanced** | 0.041 | 403 | mulesoft | https://docs.mulesoft.com/datagraph/troubleshoot-schemas-queries | ## Troubleshooting mTLS Errors<br>If you encounter mTLS errors, troubleshoot them as follows:<br>* Uploading a file that cannot be read error<br>... |

#### Overlap Analysis

- **Overlapping Results:** 2/10 (20.0%)
- **Jaccard Similarity:** 0.111

---

### Query 11: What are common HTTP status codes?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.422s | 1.207s |
| Results Count | 10 | 10 |
| Clusters Used | 5 | 1 |
| Avg Score | 0.014 | 0.017 |
| Overlap | - | 40.0% |

**Performance:** SOM-enhanced search is 0.35x faster

**Cluster Usage:** Traditional used clusters [1313, 804, 1204, 1109, 1501], SOM used clusters [1109]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1109 | mulesoft | https://docs.mulesoft.com/api-manager/latest/wsdl-raml-http-proxy-reference | # Handling API Proxy Status Codes<br>In Mule 4, WSDL, RAML, HTTP, and HTTPS proxies handle errors and requests as described in the following tables. Mule 4 returns different error codes, depending on the proxy type, or no error code in response to problematic requests. This table shows whether or not Mule returns a 504, 400, or 404 error code when your WSDL, RAML, HTTP, and HTTPS proxy receives a problematic request.<br>Error Code | WSDL | RAML | OAS | HTTP | HTTPS<br>... |
| **SOM-Enhanced** | 0.017 | 1109 | mulesoft | https://docs.mulesoft.com/http-connector/latest/http-request-ref | For a more detailed example of an HTTP response body during an HTTP request call, refer to the HTTP Error Response example documentation.<br>In the HTTP **Request** operation configuration, you can customize HTTP responses by configuring the **Response validator** field to any of these options:<br>* **None** Uses the default validator, which throws an error when the status code is greater than or equal to 400.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1109 | mulesoft | https://docs.mulesoft.com/http-connector/latest/http-request-ref | For a more detailed example of an HTTP response body during an HTTP request call, refer to the HTTP Error Response example documentation.<br>In the HTTP **Request** operation configuration, you can customize HTTP responses by configuring the **Response validator** field to any of these options:<br>* **None** Uses the default validator, which throws an error when the status code is greater than or equal to 400.<br>... |
| **SOM-Enhanced** | 0.017 | 1109 | mulesoft | https://docs.mulesoft.com/http-connector/latest/http-troubleshooting | ## Understand Common Throws<br>Here is a list of common throw messages and how to interpret them:<br>* HTTP:BAD_REQUEST<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 804 | mulesoft | https://docs.mulesoft.com/design-center/apid-behavioral-headers | If MS2-Randomize were set to `true`, the payload in the response from the mocking service might look like this, with the value of `id` conforming to the constraints:<br>```<br>{<br>... |
| **SOM-Enhanced** | 0.017 | 1109 | mulesoft | https://docs.mulesoft.com/api-manager/latest/wsdl-raml-http-proxy-reference | # Handling API Proxy Status Codes<br>In Mule 4, WSDL, RAML, HTTP, and HTTPS proxies handle errors and requests as described in the following tables. Mule 4 returns different error codes, depending on the proxy type, or no error code in response to problematic requests. This table shows whether or not Mule returns a 504, 400, or 404 error code when your WSDL, RAML, HTTP, and HTTPS proxy receives a problematic request.<br>Error Code | WSDL | RAML | OAS | HTTP | HTTPS<br>... |

#### Overlap Analysis

- **Overlapping Results:** 4/10 (40.0%)
- **Jaccard Similarity:** 0.250

---

### Query 12: How to implement proper error handling?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.981s | 2.239s |
| Results Count | 10 | 10 |
| Clusters Used | 3 | 2 |
| Avg Score | 0.014 | 0.035 |
| Overlap | - | 20.0% |

**Performance:** SOM-enhanced search is 0.44x faster

**Cluster Usage:** Traditional used clusters [505, 1116, 1109], SOM used clusters [705, 1109]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1116 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/error-handling | If you instead create the same Mule app using On Error Propagate (`on-error-propagate`) instead of On Error Continue (`on-error-continue`), you receive the same error messages in the Studio console, but you also see the logged error message in your browser. This behavior is identical to the default error handling behavior because both use On Error Propagate.<br>Note that within each On-Error component, the error path you define can incorporate any number of event processors to handle specific error types as precisely as you want. You can select specific Mule errors for the On-Error component to handle. The Error Handler component routes an error to the first On-Error component that matches the error.<br>For more complex error handling configurations at the flow level, see Introduction to Mule 4: Error Handlers. For more information about On Error Continue and On Error Propagate, see On-Error components.<br>... |
| **SOM-Enhanced** | 0.035 | 705 | mulesoft | https://docs.mulesoft.com/munit/latest/test-mock-errors-cookbook | If the On Error scope is an `on-error-propagate`, the verifications won’t be executed since the flow will propagate the error and fail, then the `validation` section of the test will be skipped.<br>In this case the error could be caught with a try scope and then the verifications can be performed:<br>Mock Error with On Error Propagate<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1109 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/error-handling | # Error Handlers<br>Errors that occur in Mule belong to one of two major categories:<br>*   * Messaging Errors<br>... |
| **SOM-Enhanced** | 0.035 | 705 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/on-error-scope-concept | # On-Error Components<br>When an error occurs in a Mule app, an Error Handler component routes the error to the first On-Error component (On Error Continue or On Error Propagate) configuration that matches the Mule error, such as `HTTP:NOT_FOUND`, `DB:CONNECTIVITY`, or `ANY` (the default for all Mule errors). If no error handling is configured for the error, the app follows a default error handling process.<br>Figure 1. Error Handling Components in Studio<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 1116 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/error-handling | ### Using On-Error Components to Handle Messaging Errors<br>Instead of relying on the default error-handling mechanism, you can use On-Error components (On Error Continue and On Error Propagate) inside a built-in or external Error Handler component.<br>The following example shows a simple flow that is configured in Studio to return the results of an HTTP request when the HTTP listener is triggered. Unlike the default error-handling example, this example configures On Error Continue (`on-error-continue`) inside the flow’s built-in Error Handler (`error-handler`) component, and On Error Continue contains a Logger that writes a description of the error.<br>... |
| **SOM-Enhanced** | 0.035 | 705 | mulesoft | https://docs.mulesoft.com/munit/latest/test-mock-errors-cookbook | # Testing and Mocking Errors<br>Anypoint Code Builder<br>Anypoint Studio<br>... |

#### Overlap Analysis

- **Overlapping Results:** 2/10 (20.0%)
- **Jaccard Similarity:** 0.111

---

### Query 13: How to improve application performance?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 1.117s | 1.152s |
| Results Count | 10 | 10 |
| Clusters Used | 5 | 2 |
| Avg Score | 0.015 | 0.019 |
| Overlap | - | 50.0% |

**Performance:** SOM-enhanced search is 0.97x faster

**Cluster Usage:** Traditional used clusters [1414, 1803, 1616, 1105, 600], SOM used clusters [1313, 1803]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-guide | # Performance Tuning Guide<br>To achieve optimal performance from your Mule applications, you must evaluate both the applications themselves and the environment in which they run. Although Mule 4 is designed to tune itself, your applications might exhibit performance issues due to their initial construction or dependencies.<br>Similarly, for on-premises installations, you might need to tune the environment itself so that your Mule applications can take full advantage of it. Because many variables influence it, tuning the performance of your application requires some trial and error.<br>... |
| **SOM-Enhanced** | 0.027 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-guide | # Performance Tuning Guide<br>To achieve optimal performance from your Mule applications, you must evaluate both the applications themselves and the environment in which they run. Although Mule 4 is designed to tune itself, your applications might exhibit performance issues due to their initial construction or dependencies.<br>Similarly, for on-premises installations, you might need to tune the environment itself so that your Mule applications can take full advantage of it. Because many variables influence it, tuning the performance of your application requires some trial and error.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-recommendations | See Repeatable vs Non-repeatable Streaming for details.<br>## Back-Pressure and MaxConcurrency<br>Understand back-pressure and learn how to use the `maxConcurrency` parameter to tune the number of concurrent messages sent to your flow.<br>... |
| **SOM-Enhanced** | 0.027 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-recommendations | See Repeatable vs Non-repeatable Streaming for details.<br>## Back-Pressure and MaxConcurrency<br>Understand back-pressure and learn how to use the `maxConcurrency` parameter to tune the number of concurrent messages sent to your flow.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-test-validations | Using this information, you can then create different repeatable, common, and high-load scenarios that test the performance limits of Mule without causing failure. To imitate actual customer behavior, introduce variables such as think time between requests and latency to the backend service.<br>## Execute Performance Test Validations<br>Before you start the test execution, ideally remove the ramp-up, tear down, and error percentage settings that can affect the throughput calculation results. Considering the best practices from the previous section, execute the testing:<br>... |
| **SOM-Enhanced** | 0.027 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-test-validations | Using this information, you can then create different repeatable, common, and high-load scenarios that test the performance limits of Mule without causing failure. To imitate actual customer behavior, introduce variables such as think time between requests and latency to the backend service.<br>## Execute Performance Test Validations<br>Before you start the test execution, ideally remove the ramp-up, tear down, and error percentage settings that can affect the throughput calculation results. Considering the best practices from the previous section, execute the testing:<br>... |

#### Overlap Analysis

- **Overlapping Results:** 5/10 (50.0%)
- **Jaccard Similarity:** 0.333

---

### Query 14: What is caching and how to implement it?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.890s | 1.356s |
| Results Count | 10 | 10 |
| Clusters Used | 3 | 2 |
| Avg Score | 0.015 | 0.039 |
| Overlap | - | 60.0% |

**Performance:** SOM-enhanced search is 0.66x faster

**Cluster Usage:** Traditional used clusters [209, 323, 1515], SOM used clusters [2320, 323]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 323 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-http-caching | Follow HTTP Caching directives | Enables the use of Cache-Control header directives. Default value: `true`<br>Invalidation Header | Name of the header used to invalidate a single entry or the entire cache.<br>Conditional Request Caching Expression | The DataWeave expression that is used to decide which requests are to be cached (caches the response only if the condition is true). Default value: `#[attributes.method == 'GET' or attributes.method == 'HEAD']`<br>... |
| **SOM-Enhanced** | 0.072 | 2320 | mulesoft | https://docs.mulesoft.com/api-community-manager/cache | # Configure the Platform Cache<br>Improve the performance of pages and components in your Salesforce Experience Cloud site by using the platform cache.<br>The platform cache has two parts: a session cache that holds data specific to one user and their session, and an organization cache that holds data accessed by multiple users in the organization.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 323 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-http-caching | The following command invalidates the entry with key “/my/policy" from the cache:<br>`curl http://<MyAppURL>/my/policy -H “myInvalidationHeader:invalidate”`<br>The following request invalidates all entries from the cache:<br>... |
| **SOM-Enhanced** | 0.072 | 2320 | mulesoft | https://docs.mulesoft.com/api-community-manager/cache | Cache size defaults to zero. To finish configuring the caches, set the cache size:<br>1. Log in to your Salesforce organization.<br>2. In **Setup** , click **Platform Cache**.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 209 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-caching | # Caching<br>Identifying key aspects of your data such as when to use cache and which cache strategy to follow, helps you to improve processing performance:<br>* Is the data frequently called, with often repeated results?<br>... |
| **SOM-Enhanced** | 0.031 | 323 | mulesoft | https://docs.mulesoft.com/mule-gateway/policies-included-http-caching | # HTTP Caching Policy<br>**Policy Name** | HTTP caching<br>---|---<br>... |

#### Overlap Analysis

- **Overlapping Results:** 6/10 (60.0%)
- **Jaccard Similarity:** 0.429

---

### Query 15: How to optimize memory usage?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 1.050s | 1.388s |
| Results Count | 10 | 10 |
| Clusters Used | 4 | 2 |
| Avg Score | 0.013 | 0.005 |
| Overlap | - | 30.0% |

**Performance:** SOM-enhanced search is 0.76x faster

**Cluster Usage:** Traditional used clusters [2008, 1619, 1616, 1119], SOM used clusters [2320, 1616]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 2008 | mulesoft | https://docs.mulesoft.com/runtime-manager/monitoring-dashboards | You can also navigate to a server’s monitoring dashboard from the server group or cluster dashboard that includes the server.<br>### Navigate the Server Monitoring Dashboard<br>The server monitoring dashboard displays metrics divided into two tabs:<br>... |
| **SOM-Enhanced** | 0.026 | 2320 | mulesoft | https://docs.mulesoft.com/api-community-manager/cache | Cache size defaults to zero. To finish configuring the caches, set the cache size:<br>1. Log in to your Salesforce organization.<br>2. In **Setup** , click **Platform Cache**.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 2008 | mulesoft | https://docs.mulesoft.com/runtime-manager/monitoring-dashboards | See the Breakdown tab for details about each of the components of the heap memory.<br><br>CPU<br>... |
| **SOM-Enhanced** | 0.026 | 2320 | mulesoft | https://docs.mulesoft.com/api-community-manager/cache | # Configure the Platform Cache<br>Improve the performance of pages and components in your Salesforce Experience Cloud site by using the platform cache.<br>The platform cache has two parts: a session cache that holds data specific to one user and their session, and an organization cache that holds data accessed by multiple users in the organization.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.013 | 1616 | mulesoft | https://docs.mulesoft.com/runtime-fabric/latest/deploy-resource-allocation-self-managed | ## Memory Allocation<br>The minimum values for the amount of memory allocated to each replica of a Mule application or API gateway is:<br>* 0.7 GiB memory for Mule 4<br>... |
| **SOM-Enhanced** | 0.000263 | 1616 | mulesoft | https://docs.mulesoft.com/runtime-fabric/2.4/deploy-resource-allocation-self-managed | ## Memory Allocation<br>The minimum values for the amount of memory allocated to each replica of a Mule application or API gateway are the following:<br>* 0.7 GiB memory for Mule 4<br>... |

#### Overlap Analysis

- **Overlapping Results:** 3/10 (30.0%)
- **Jaccard Similarity:** 0.176

---

### Query 16: How to use Docker containers?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 1.246s | 1.192s |
| Results Count | 10 | 10 |
| Clusters Used | 7 | 1 |
| Avg Score | 0.014 | 0.004 |
| Overlap | - | 20.0% |

**Performance:** SOM-enhanced search is 1.05x faster

**Cluster Usage:** Traditional used clusters [518, 2407, 201, 106, 1519, 24, 1208], SOM used clusters [1208]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.017 | 24 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-troubleshoot-docker | # Troubleshooting Docker Command Issues<br>Troubleshoot errors returned by a `docker` command:<br>* Docker Is Not Started<br>... |
| **SOM-Enhanced** | 0.004 | 1208 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-install | Due to issues with the CentOS package manager you might encounter the following error:<br>```<br>Error: Failed to download metadata for repo 'AppStream': Cannot prepare internal mirrorlist: No URLs in mirrorlist<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1208 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-install | Due to issues with the CentOS package manager you might encounter the following error:<br>```<br>Error: Failed to download metadata for repo 'AppStream': Cannot prepare internal mirrorlist: No URLs in mirrorlist<br>... |
| **SOM-Enhanced** | 0.004 | 1208 | mulesoft | https://docs.mulesoft.com/gateway/latest/flex-gateway-getting-started | ## Run Flex Gateway<br>To run Flex Gateway, run the following in a terminal window:<br>```<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 201 | mulesoft | https://docs.mulesoft.com/runtime-fabric/1.13/configure-local-registry | You should see a message that the login was successful.<br>3. To pull and synchronize images, log in into your own private container registry and run the following command, replacing `<docker-server>` where appropriate:<br>For the US control plane:<br>... |
| **SOM-Enhanced** | 0.004 | 1208 | mulesoft | https://docs.mulesoft.com/gateway/latest | * A standalone runtime in a Docker container<br>* A sidecar to a backend application in a Docker container, thereby protecting a single backend application<br>* A Kubernetes `Deployment` for high-availability, high-performance use cases<br>... |

#### Overlap Analysis

- **Overlapping Results:** 2/10 (20.0%)
- **Jaccard Similarity:** 0.111

---

### Query 17: What is Kubernetes and how does it work?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.949s | 1.357s |
| Results Count | 10 | 10 |
| Clusters Used | 6 | 2 |
| Avg Score | 0.014 | 0.012 |
| Overlap | - | 40.0% |

**Performance:** SOM-enhanced search is 0.70x faster

**Cluster Usage:** Traditional used clusters [1412, 518, 1420, 813, 1104, 1203], SOM used clusters [1312, 1412]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1412 | mulesoft | https://docs.mulesoft.com/runtime-fabric/2.4 | # Anypoint Runtime Fabric Overview<br>Anypoint Runtime Fabric enables you to deploy Mule applications and API proxies to a Kubernetes cluster that you create, configure, and manage.<br>If you work in public clouds and have some level of expertise in managing a Kubernetes cluster, Runtime Fabric supports:<br>... |
| **SOM-Enhanced** | 0.013 | 1312 | mulesoft | https://docs.mulesoft.com/runtime-fabric/latest/rtfctl-permissions | pods/exec<br>configmaps, secrets<br>rtfctl-audit | create, get, patch, update<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 1412 | mulesoft | https://docs.mulesoft.com/runtime-fabric/1.13 | # Anypoint Runtime Fabric Overview<br>Anypoint Runtime Fabric is a container service that allows you to run Mule applications, composite APIs and API gateways across any environment with centralized management via Anypoint Platform.<br>Some of the capabilities of Anypoint Runtime Fabric include:<br>... |
| **SOM-Enhanced** | 0.013 | 1312 | mulesoft | https://docs.mulesoft.com/runtime-fabric/latest/customize-kubernetes-crd | # Customizing Mule App Kubernetes Resources<br>Anypoint Runtime Fabric enables you to customize your Mule app Kubernetes resources through the custom resource `kubernetestemplates.rtf.mulesoft.com` template.<br>Name the `kubernetestemplate` resource as `mule-application`. You can define the template in two different namespaces:<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 813 | mulesoft | https://docs.mulesoft.com/runtime-fabric/latest/configure-kubernetes | # Configuring Kubernetes for Runtime Fabric<br>To configure Kubernetes for Anypoint Runtime Fabric, review the following topics:<br>* Kubernetes (K8s) Best Practices for Runtime Fabric Review scalability benchmarks and cluster configurations best practices.<br>... |
| **SOM-Enhanced** | 0.013 | 1312 | mulesoft | https://docs.mulesoft.com/runtime-fabric/latest/rtfctl-permissions | cronjobs | create, get, patch, update<br>rtf.mulesoft.com | persistencegateways | get, list, watch<br>rtfctl-audit | create, get, patch, update<br>... |

#### Overlap Analysis

- **Overlapping Results:** 4/10 (40.0%)
- **Jaccard Similarity:** 0.250

---

### Query 18: How to implement microservices architecture?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.759s | 1.253s |
| Results Count | 10 | 10 |
| Clusters Used | 7 | 1 |
| Avg Score | 0.013 | 0.014 |
| Overlap | - | 20.0% |

**Performance:** SOM-enhanced search is 0.61x faster

**Cluster Usage:** Traditional used clusters [623, 209, 210, 914, 2104, 1112, 1212], SOM used clusters [209]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 209 | mulesoft | https://docs.mulesoft.com/release-notes/platform/event-driven-api | # AsyncAPI Support to Implement Event-Driven Architecture<br>## Overview<br>Implement event-driven architecture (EDA) as part of your API-led strategy using the AsyncAPI support in Anypoint Platform. AsyncAPI is an open-source, industry-standard language that describes messaging interfaces.<br>... |
| **SOM-Enhanced** | 0.014 | 209 | mulesoft | https://docs.mulesoft.com/release-notes/platform/event-driven-api | # AsyncAPI Support to Implement Event-Driven Architecture<br>## Overview<br>Implement event-driven architecture (EDA) as part of your API-led strategy using the AsyncAPI support in Anypoint Platform. AsyncAPI is an open-source, industry-standard language that describes messaging interfaces.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 2104 | mulesoft | https://docs.mulesoft.com/mule-gateway | # Anypoint Platform Gateways<br>An API gateway allows you to add a dedicated orchestration layer on top of your backend APIs and services to help you separate orchestration from implementation concerns. You can then leverage the governance capabilities of API Manager to apply, among other capabilities, throttling, security, caching, and logging to your APIs.<br>Anypoint Platform offers three different runtime options for managing and securing your APIs.<br>... |
| **SOM-Enhanced** | 0.014 | 209 | mulesoft | https://docs.mulesoft.com/cloudhub-2/ch2-architecture | # CloudHub 2.0 Architecture<br>To understand CloudHub 2.0 security and availability, you should understand the architecture behind CloudHub 2.0.<br>CloudHub 2.0 architecture comprises two major components: Anypoint Platform services and shared global regions. These two components, along with Anypoint Runtime Manager through which you access them, work together to run your integration applications.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.015 | 210 | mulesoft | https://docs.mulesoft.com/runtime-manager/runtime-manager-agent-architecture | # Runtime Manager Agent Architecture<br>Private Cloud Edition<br>The Anypoint Runtime Manager agent is a Mule plugin that exposes the Mule JAVA API as a service, allowing users to manipulate and monitor Mule instances from external systems.<br>... |
| **SOM-Enhanced** | 0.014 | 209 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/hadr-guide | System backups are a major component of a solid disaster recovery program. There are three types of recovery: cold, warm, and hot.<br>Term | Definition | Example<br>---|---|---<br>... |

#### Overlap Analysis

- **Overlapping Results:** 2/10 (20.0%)
- **Jaccard Similarity:** 0.111

---

### Query 19: How to implement a complete authentication system with OAuth2, JWT tokens, and role-based access control?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.772s | 1.262s |
| Results Count | 10 | 10 |
| Clusters Used | 7 | 2 |
| Avg Score | 0.013 | 0.012 |
| Overlap | - | 30.0% |

**Performance:** SOM-enhanced search is 0.61x faster

**Cluster Usage:** Traditional used clusters [2409, 2413, 209, 1010, 1012, 309, 314], SOM used clusters [209, 314]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 314 | mulesoft | https://docs.mulesoft.com/oauth2-provider-module/latest | # OAuth2 Provider Module 1.2<br>The OAuth2 Provider module enables a Mule runtime engine (Mule) app to be configured as an Authentication Manager in an OAuth2 dance. With this role, the application can authenticate to previously registered clients, grant tokens, validate tokens, or register and delete clients, all during the execution of a flow.<br>The following documentation assumes a basic knowledge of the OAuth2 authorization protocol. For further reference, see the RFC-6749.<br>... |
| **SOM-Enhanced** | 0.016 | 314 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/mule-secure-token-service | # Mule Secure Token Service OAuth 2.0<br>The Mule runtime engine supports the OAuth 2.0 protocol. The way to configure OAuth 2.0 authorization differs, depending on the OAuth role and your objective:<br>* Configure authentication in your client Mule app when sending requests to a service that requires authentication, such as the Github OAuth2 server. Use the OAuth Module for the OAuth2 configuration.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 2409 | mulesoft | https://docs.mulesoft.com/access-management/creating-connected-apps-dev | ### Refresh Token<br>Use the `refresh_token` grant type to grant access to user data when the user isn’t signed in. Refresh tokens expire after 90 days. Access tokens expire after the user’s session expires.<br>To work with OpenID Connect, apps exchange refresh tokens for new access tokens after the initial authorization to continue accessing user data.<br>... |
| **SOM-Enhanced** | 0.016 | 314 | mulesoft | https://docs.mulesoft.com/api-manager/latest/mule-oauth-provider-landing-page | ## OAuth 2.0 Dance<br>The authentication performed by the OAuth 2.0 provider, API, and client application conforms to RFC 6749. This authentication process is known as the OAuth 2.0 dance.<br>Mule OAuth 2.0 Provider supports all grant types. The entity that requests access to a resource protected by the Mule OAuth 2.0 Access Token Enforcement policy is a `Client`.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.014 | 2413 | mulesoft | https://docs.mulesoft.com/pdk/latest/policies-pdk-configure-features-jwt | # Using JWT Library Functions<br>To view an example policy project that uses Flex Gateway Policy Development Kit (PDK)'s JWT library, see JWT Validation Policy Example.<br>---<br>... |
| **SOM-Enhanced** | 0.016 | 314 | mulesoft | https://docs.mulesoft.com/oauth2-provider-module/latest | # OAuth2 Provider Module 1.2<br>The OAuth2 Provider module enables a Mule runtime engine (Mule) app to be configured as an Authentication Manager in an OAuth2 dance. With this role, the application can authenticate to previously registered clients, grant tokens, validate tokens, or register and delete clients, all during the execution of a flow.<br>The following documentation assumes a basic knowledge of the OAuth2 authorization protocol. For further reference, see the RFC-6749.<br>... |

#### Overlap Analysis

- **Overlapping Results:** 3/10 (30.0%)
- **Jaccard Similarity:** 0.176

---

### Query 20: What are the best practices for designing a scalable microservices architecture with proper error handling and monitoring?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.750s | 1.407s |
| Results Count | 10 | 10 |
| Clusters Used | 8 | 2 |
| Avg Score | 0.011 | 0.007 |
| Overlap | - | 30.0% |

**Performance:** SOM-enhanced search is 0.53x faster

**Cluster Usage:** Traditional used clusters [1803, 1116, 911, 209, 309, 1109, 2104, 1212], SOM used clusters [209, 1109]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.013 | 1116 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/error-handling | If you instead create the same Mule app using On Error Propagate (`on-error-propagate`) instead of On Error Continue (`on-error-continue`), you receive the same error messages in the Studio console, but you also see the logged error message in your browser. This behavior is identical to the default error handling behavior because both use On Error Propagate.<br>Note that within each On-Error component, the error path you define can incorporate any number of event processors to handle specific error types as precisely as you want. You can select specific Mule errors for the On-Error component to handle. The Error Handler component routes an error to the first On-Error component that matches the error.<br>For more complex error handling configurations at the flow level, see Introduction to Mule 4: Error Handlers. For more information about On Error Continue and On Error Propagate, see On-Error components.<br>... |
| **SOM-Enhanced** | 0.009 | 1109 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/intro-error-handlers | Consider the following application where an HTTP listener triggers a Flow Reference component to another flow that performs an HTTP request. If everything goes right when a message is received (1 below), the reference is triggered (2), and the request performed (3), which results in a successful response (HTTP status code 200) (4).<br>If the HTTP request fails with an `HTTP:NOT_FOUND` error (see 3 below) because of the error handler configuration in `inner-flow`, the error is propagated (4), and the Flow Reference component fails (2). However, because `primary-flow` handles the error with `on-error-continue`, the Logger it contains (5) executes, and a successful response (HTTP status code 200) is returned (6).<br>If the request fails with an unauthorized error instead (3), then `inner-flow` handles it with an `on-error-continue` by retrieving static content from a file (4). Then the Flow Reference component is successful as well (2), and a successful response (HTTP status code 200) is returned (5).<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.012 | 309 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/build-app-practices | # Best Practices to Build Mule Applications<br>As you build your applications, consider the following best practices for creating a clean, organized, and sustainable project. These practices include guidelines on using Anypoint Studio, avoiding certain app-building issues, and specific settings for using Mule runtime engine (Mule) components and connectors.<br>## Anypoint Studio Best Practices<br>... |
| **SOM-Enhanced** | 0.009 | 1109 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/intro-error-handlers | # Introduction to Mule 4: Error Handlers<br>In Mule 4, error handling is no longer limited to a Java exception handling process that requires you to check the source code or force an error in order to understand what happened. Though Java `Throwable` errors and exceptions are still available, Mule 4 introduces a formal Error concept that’s easier to use. Now, each component declares the type of errors it can throw, so you can identify potential errors at design time.<br>## Mule Errors<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.012 | 1212 | mulesoft | https://docs.mulesoft.com/cloudhub/cloudhub-architecture | ## Availability and Scalability<br>CloudHub is designed to be highly available and scalable through redundancy, intelligent healing, and zero-downtime updates. It also enables customers to scale and benefit from added reliability through high availability features.<br>### Redundant Platform<br>... |
| **SOM-Enhanced** | 0.009 | 1109 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/error-handling | # Error Handlers<br>Errors that occur in Mule belong to one of two major categories:<br>*   * Messaging Errors<br>... |

#### Overlap Analysis

- **Overlapping Results:** 3/10 (30.0%)
- **Jaccard Similarity:** 0.176

---

### Query 21: How to optimize database performance for high-traffic applications with proper indexing and caching strategies?

#### Query Metrics

| Metric | Traditional | SOM-Enhanced |
|--------|-------------|--------------|
| Duration | 0.909s | 1.229s |
| Results Count | 10 | 10 |
| Clusters Used | 6 | 1 |
| Avg Score | 0.014 | 0.015 |
| Overlap | - | 10.0% |

**Performance:** SOM-enhanced search is 0.74x faster

**Cluster Usage:** Traditional used clusters [323, 1512, 1803, 1616, 209, 600], SOM used clusters [600]

#### Results Comparison Table

**Rank 1**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.017 | 209 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-caching | # Caching<br>Identifying key aspects of your data such as when to use cache and which cache strategy to follow, helps you to improve processing performance:<br>* Is the data frequently called, with often repeated results?<br>... |
| **SOM-Enhanced** | 0.015 | 600 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/mule-high-availability-ha-clusters | ## Clustering Best Practices<br>There are a number of recommended practices related to clustering. These include:<br>* As much as possible, organize your application into a series of steps where each step moves the message from one transactional store to another.<br>... |

**Rank 2**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1803 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/tuning-recommendations | See Repeatable vs Non-repeatable Streaming for details.<br>## Back-Pressure and MaxConcurrency<br>Understand back-pressure and learn how to use the `maxConcurrency` parameter to tune the number of concurrent messages sent to your flow.<br>... |
| **SOM-Enhanced** | 0.015 | 600 | mulesoft | https://docs.mulesoft.com/cloudhub-2/ch2-clustering | You have a high-stakes process for which you need to protect against message loss, but you are not experiencing issues with handling processing load and are OK with some service interruption in the case of a data center outage. |  Number of Replicas: One Clustering enabled |<br>* The application can experience some queue latency.<br>* Configure your application to support queues before deploying.<br>... |

**Rank 3**

| Method | Score | Cluster | Source | Source URL | Content Preview |
|--------|-------|---------|--------|------------|----------------|
| **Traditional** | 0.016 | 1616 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/mule-high-availability-ha-clusters | ## Clustering and Load Balancing<br>When Mule clusters are used to serve TCP requests (where TCP includes SSL/TLS, UDP, Multicast, HTTP, and HTTPS), some load balancing is needed to distribute the requests among the clustered instances. Though Anypoint Runtime Fabric includes load-balancer capability as part of the underlying Docker Kubernetes (K8s) infrastructure, customer-hosted, manually-provisioned clusters require you to supply a third party load balancer or perform client-side load balancing and fail-over. There are various software load balancers available, two of them are:<br>* NGINX, an open-source HTTP server and reverse proxy. You can use NGINX’s `HttpUpstreamModule` for HTTP(S) load balancing.<br>... |
| **SOM-Enhanced** | 0.015 | 600 | mulesoft | https://docs.mulesoft.com/mule-runtime/latest/choosing-the-right-clustering-topology | Cons:<br>* Requires lots of transactions, and transactions can be complicated<br>* Performance hit if you’re using XA<br>... |

#### Overlap Analysis

- **Overlapping Results:** 1/10 (10.0%)
- **Jaccard Similarity:** 0.053

---