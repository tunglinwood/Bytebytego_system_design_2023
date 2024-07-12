![image](https://github.com/user-attachments/assets/88ab4fdf-9b55-48ea-b417-a84a0e8a5ecc)![image](https://github.com/user-attachments/assets/2e44dc79-cfd6-49fd-bf94-2daf51fb4c0b)# Bytebytego_system_design_2023

# 解释九种 API 测试类型  Explaining 9 types of API testing
![image](https://github.com/user-attachments/assets/67059ebe-2789-491e-a4f1-0b06c41f2e3c)

1. **烟雾测试 (Smoke Testing)**
    - **定义**: 在 API 开发完成后进行的初步测试。
    - **目标**: 简单验证 API 是否正常工作且没有出现重大问题。
    - **例子**: 检查 API 是否能够正确启动和处理基本请求。

2. **功能测试 (Functional Testing)**
    - **定义**: 根据功能要求创建测试计划，并将结果与预期结果进行比较。
    - **目标**: 确保 API 的每个功能按照预期工作。
    - **例子**: 测试 API 的登录功能是否在输入正确凭据时返回正确的用户信息。

3. **集成测试 (Integration Testing)**
    - **定义**: 结合多个 API 调用进行端到端测试。
    - **目标**: 测试服务内的通信和数据传输。
    - **例子**: 测试用户注册 API 后，是否能够正确创建用户并在用户数据库中添加记录。

4. **回归测试 (Regression Testing)**
    - **定义**: 确保修复的错误或新功能不会破坏 API 的现有行为。
    - **目标**: 确保更新后的 API 依然稳定。
    - **例子**: 在 API 新增了密码重置功能后，测试以前的所有功能仍能正常工作。

5. **负载测试 (Load Testing)**
    - **定义**: 通过模拟不同的负载来测试应用程序的性能。
    - **目标**: 测试 API 在各种负载条件下的响应时间和性能。
    - **例子**: 测试 API 在每秒处理1000个请求时的性能表现。

6. **压力测试 (Stress Testing)**
    - **定义**: 故意对 API 施加高负载，测试其稳定性。
    - **目标**: 确保 API 在极端负载条件下依然能正常工作。
    - **例子**: 测试 API 在每秒处理5000个请求时是否会崩溃。

7. **安全测试 (Security Testing)**
    - **定义**: 测试 API 是否能够抵御所有可能的外部威胁。
    - **目标**: 确保 API 的安全性，防止未授权访问和数据泄露。
    - **例子**: 测试 API 是否能有效防止 SQL 注入攻击。

8. **UI 测试 (UI Testing)**
    - **定义**: 测试 UI 与 API 的交互，确保数据能够正确显示。
    - **目标**: 确保前端应用程序正确使用 API 并显示返回的数据。
    - **例子**: 测试用户界面在调用用户信息 API 后是否能正确显示用户详情。

9. **模糊测试 (Fuzz Testing)**
    - **定义**: 向 API 注入无效或意外的输入数据，尝试使 API 崩溃。
    - **目标**: 识别 API 的漏洞和弱点。
    - **例子**: 向 API 提交随机生成的无效数据，观察其如何处理并防止崩溃。

# Kafka 的五大使用场景 Top 5 Kafka use cases
![image](https://github.com/user-attachments/assets/368107c5-ecc0-43b8-8855-4df5d65ee321)

1. **日志处理和分析 (Log Processing and Analytics)**
    - **概述**: Kafka 最初是为大规模日志处理而构建的。它保留消息直到过期，并让消费者以自己的节奏拉取消息。
    - **应用场景**: 
        - **服务器日志**: 收集和存储服务器日志数据。
        - **用户活动跟踪**: 监控和分析用户在应用程序上的行为。
    - **优势**: 提供实时数据处理和存储能力，支持后续的数据分析和监控。

2. **推荐系统中的数据流 (Data Streaming in Recommendation Systems)**
    - **概述**: 实时处理用户行为数据，以提供个性化推荐。
    - **应用场景**: 
        - **电商网站**: 根据用户浏览和购买历史推荐商品。
        - **流媒体平台**: 根据用户观看历史推荐视频或音乐。
    - **优势**: 提供实时数据处理，提升用户体验和推荐准确性。

3. **系统监控和报警 (System Monitoring and Alerting)**
    - **概述**: 使用 Kafka 收集和处理系统监控数据，以便实时监控和报警。
    - **应用场景**: 
        - **服务器性能监控**: 收集 CPU、内存、磁盘使用情况数据。
        - **异常检测**: 监控应用程序异常情况并及时报警。
    - **优势**: 实时处理和分析大量监控数据，及时发现和响应系统问题。

4. **数据变更捕获 (Change Data Capture, CDC)**
    - **概述**: 监控数据库中的数据变更，并将这些变更实时推送到其他系统或服务。
    - **应用场景**: 
        - **数据库同步**: 在不同数据库之间同步数据变更。
        - **事件驱动架构**: 根据数据库变更触发相应的业务逻辑。
    - **优势**: 提供实时数据同步和处理能力，支持事件驱动的系统架构。

5. **系统迁移 (System Migration)**
    - **概述**: 在系统迁移过程中，使用 Kafka 实时复制数据，确保数据一致性和系统无缝切换。
    - **应用场景**: 
        - **云迁移**: 将本地系统迁移到云平台。
        - **数据库迁移**: 在不同数据库系统之间迁移数据。
    - **优势**: 确保数据在迁移过程中的一致性和完整性，减少系统停机时间。

# 数据如何通过互联网传输？这与 OSI 模型有什么关系？TCP/IP 在其中如何应用？How is data sent over the ianternet? What does that have to do with the OSI model? How does TCP/IP fit into this?
![image](https://github.com/user-attachments/assets/e6f3a78d-47a8-4c73-9d4b-60b71baeb5cf)

#### 数据通过互联网传输的过程

1. **数据分段**：当你在计算机上发送数据时，这些数据会被分割成更小的片段，称为数据包。每个数据包包含一部分数据以及一些控制信息，如目的地址和源地址。

2. **数据封装**：每个数据包会通过多层封装，添加不同层级的头信息，以便在网络中传输。

3. **数据传输**：数据包通过各种网络设备（如路由器、交换机）从源地址传输到目的地址。

4. **数据解封装**：到达目的地后，数据包的封装层会逐层被去除，直到获取原始数据。

5. **数据重组**：目的地设备接收到所有数据包后，将它们重新组装成原始数据。

#### OSI 模型与数据传输的关系

OSI 模型（开放系统互连模型）是一个抽象的框架，用于理解和设计网络系统的通信。它将网络通信过程分成七个层级，每一层负责特定的功能：

1. **物理层 (Physical Layer)**：负责物理连接和传输原始比特流。
2. **数据链路层 (Data Link Layer)**：负责节点间的可靠传输，处理错误检测和纠正。
3. **网络层 (Network Layer)**：负责路径选择和逻辑地址（如IP地址）。
4. **传输层 (Transport Layer)**：负责端到端的传输控制和数据完整性（如TCP/UDP）。
5. **会话层 (Session Layer)**：负责建立、管理和终止会话。
6. **表示层 (Presentation Layer)**：负责数据格式化、加密和解密。
7. **应用层 (Application Layer)**：提供网络服务和应用程序接口（如HTTP、FTP）。

#### TCP/IP 与 OSI 模型的关系

TCP/IP（传输控制协议/互联网协议）是一组通信协议，用于互联网和其他网络的连接。它是一个四层模型，与 OSI 模型有很多相似之处：

1. **网络接口层 (Network Interface Layer)**：相当于 OSI 模型的物理层和数据链路层。
2. **网络层 (Internet Layer)**：相当于 OSI 模型的网络层，负责路由和逻辑地址（如IP地址）。
3. **传输层 (Transport Layer)**：与 OSI 模型的传输层对应，负责端到端的传输控制和数据完整性（如TCP/UDP）。
4. **应用层 (Application Layer)**：相当于 OSI 模型的会话层、表示层和应用层，提供网络服务和应用程序接口（如HTTP、FTP）。

#### 数据传输示例

当你在浏览器中访问一个网站时，以下是数据通过互联网传输的过程：

1. **应用层**：浏览器使用HTTP协议发送请求。
2. **传输层**：请求被分割成数据包，并通过TCP协议进行封装，确保数据可靠传输。
3. **网络层**：每个数据包被分配IP地址，并通过互联网路由传输到目标服务器。
4. **网络接口层**：数据包通过物理网络（如以太网、Wi-Fi）传输到下一跳。

到达目的服务器后，数据包会经过解封装、重组和处理，服务器将响应数据以同样的方式返回到你的浏览器。

# 提高 API 性能的五种常见方法 Top 5 common ways to improve API performance
![image](https://github.com/user-attachments/assets/c66fba42-644d-4e68-837c-563e5e8d17f7)

1. **结果分页 (Result Pagination)**
    - **定义**: 将大量结果集分割成更小的页，每次请求只返回一个页的数据。
    - **优势**: 通过流式传输大型结果集来优化响应时间，减少服务器负载，并提升用户体验。
    - **实施方式**: 例如，在查询数据库时，只返回特定页的数据（使用 `LIMIT` 和 `OFFSET` 或类似机制）。

    ```sql
    SELECT * FROM users LIMIT 10 OFFSET 20;
    ```

2. **异步日志记录 (Asynchronous Logging)**
    - **定义**: 将日志发送到无锁缓冲区并立即返回，而不是在每次调用时处理磁盘写入。
    - **优势**: 大大减少了 I/O 开销，提升 API 的响应速度。
    - **实施方式**: 使用异步日志框架，如 Log4j 的异步日志记录功能。

    ```java
    import org.apache.logging.log4j.LogManager;
    import org.apache.logging.log4j.Logger;

    public class MyService {
        private static final Logger logger = LogManager.getLogger(MyService.class);

        public void processRequest() {
            logger.info("Processing request...");
            // 其他处理逻辑
        }
    }
    ```

3. **数据缓存 (Data Caching)**
    - **定义**: 将频繁访问的数据存储在缓存中以加速检索。
    - **优势**: 加快数据读取速度，减少数据库查询次数，提高整体性能。
    - **实施方式**: 使用像 Redis 这样的缓存系统，将数据缓存到内存中。

    ```python
    import redis

    cache = redis.StrictRedis(host='localhost', port=6379, db=0)

    def get_user(user_id):
        user = cache.get(f"user:{user_id}")
        if not user:
            user = database_query(user_id)  # 假设这是一个查询数据库的函数
            cache.set(f"user:{user_id}", user)
        return user
    ```

4. **负载压缩 (Payload Compression)**
    - **定义**: 对请求和响应数据进行压缩，以减少数据传输时间。
    - **优势**: 加快上传和下载过程，特别是在网络带宽有限的情况下。
    - **实施方式**: 使用 gzip 或类似压缩算法压缩 HTTP 响应。

    ```python
    from flask import Flask, request, jsonify
    from flask_compress import Compress

    app = Flask(__name__)
    Compress(app)

    @app.route('/data')
    def get_data():
        data = {"key": "value"}
        return jsonify(data)
    ```

5. **连接池化 (Connection Pooling)**
    - **定义**: 使用连接池来管理数据库连接，避免每次请求都建立和关闭连接。
    - **优势**: 减少了数据库连接建立的开销，提高了数据库操作的效率。
    - **实施方式**: 使用连接池库，如 SQLAlchemy 的连接池功能。

    ```python
    from sqlalchemy import create_engine
    from sqlalchemy.orm import sessionmaker

    engine = create_engine('postgresql://user:password@localhost/dbname', pool_size=20, max_overflow=0)
    Session = sessionmaker(bind=engine)

    def get_user(user_id):
        session = Session()
        user = session.query(User).filter_by(id=user_id).first()
        session.close()
        return user
    ```

# CI/CD 简化视觉指南 CI/CD Simplified Visual Guide
![image](https://github.com/user-attachments/assets/28b33e62-5a66-4a42-bb8d-cbeb3432ea7a)

#### 1. 持续集成 (CI) 和持续交付/部署 (CD) 概述

**CI/CD** 是现代软件开发和运维的核心实践，通过自动化测试、构建和部署流程，提高软件交付速度和质量。

---

#### 2. CI/CD 流程图

```
+----------------+       +--------------------+      +-------------------+      +-------------------+      +-------------------+
|                |       |                    |      |                   |      |                   |      |                   |
|    开发人员       +----->   代码提交到版本控制      +----->   自动化测试执行       +----->   构建应用程序         +----->   部署到测试环境       |
|                |       |    (Git, SVN 等)      |      |   (单元测试、集成测试等)  |      |  (编译、打包等)          |      |                   |
+----------------+       +--------------------+      +-------------------+      +-------------------+      +-------------------+
                                                                                                      
                                                                                                      +-------------------+
                                                                                                      |                   |
                                                                                                      |   部署到生产环境        |
                                                                                                      |                   |
                                                                                                      +-------------------+
```

---

#### 3. CI/CD 流程的关键步骤

1. **代码提交 (Code Commit)**
    - 开发人员将代码提交到版本控制系统（如 Git、SVN 等）。
    - 触发 CI/CD 流程的开始。

2. **自动化测试 (Automated Testing)**
    - CI 系统自动拉取最新代码并运行预定义的测试套件。
    - 包括单元测试、集成测试等，以确保代码质量。

3. **构建应用程序 (Build Application)**
    - 成功通过测试后，代码被编译和打包成可部署的应用程序。
    - 构建工件（如 JAR 文件、Docker 镜像）被创建。

4. **部署到测试环境 (Deploy to Staging)**
    - 构建的应用程序被自动部署到测试环境。
    - 进行进一步的集成测试和用户验收测试（UAT）。

5. **部署到生产环境 (Deploy to Production)**
    - 最终验证后，应用程序被部署到生产环境。
    - 用户可以访问最新版本的应用程序。

---

#### 4. CI/CD 工具和技术

- **版本控制系统 (VCS)**: Git, SVN
- **CI/CD 工具**: Jenkins, GitLab CI, CircleCI, Travis CI
- **构建工具**: Maven, Gradle
- **容器化技术**: Docker, Kubernetes
- **测试框架**: JUnit, Selenium, Postman

---

#### 5. CI/CD 流程的好处

- **自动化测试和部署**: 减少人为错误，提高交付效率。
- **快速反馈循环**: 开发人员能迅速获得代码变更的反馈。
- **持续交付**: 确保每次代码提交都能通过自动化流程发布。
- **改进协作**: 团队成员可以更高效地协作，共享构建和测试结果。

---

### 总结

通过实施 CI/CD 流程，团队能够显著提高软件开发和交付的效率和质量。自动化的测试和部署流程使得代码更快、更可靠地交付到生产环境，从而提供更好的用户体验。

---

**视觉指南的示例图：**

```plaintext
+----------------+       +--------------------+      +-------------------+      +-------------------+      +-------------------+
|                |       |                    |      |                   |      |                   |      |                   |
|    开发人员       +----->   代码提交到版本控制      +----->   自动化测试执行       +----->   构建应用程序         +----->   部署到测试环境       |
|                |       |    (Git, SVN 等)      |      |   (单元测试、集成测试等)  |      |  (编译、打包等)          |      |                   |
+----------------+       +--------------------+      +-------------------+      +-------------------+      +-------------------+
                                                                                                      
                                                                                                      +-------------------+
                                                                                                      |                   |
                                                                                                      |   部署到生产环境        |
                                                                                                      |                   |
                                                                                                      +-------------------+
```

# 用户最喜欢的九大工程博客 There are over 1,000 engineering blogs. Here are my top 9 favorites:
![image](https://github.com/user-attachments/assets/004c033f-3665-4c26-bacd-85de728cf015)

1. **Netflix Tech Blog**
    - **网址**: [Netflix Tech Blog](https://netflixtechblog.com/)
    - **简介**: Netflix 的工程博客分享了该公司在大规模系统、数据科学、微服务和机器学习方面的技术实践和经验。
    - **内容类型**: 系统设计、数据流处理、云计算、A/B 测试等。

2. **Uber Engineering Blog**
    - **网址**: [Uber Engineering Blog](https://eng.uber.com/)
    - **简介**: Uber 的工程博客涵盖了该公司在实时数据处理、地图服务、分布式系统和人工智能方面的技术突破。
    - **内容类型**: 大数据处理、后端开发、移动开发、机器学习等。

3. **Facebook Engineering Blog**
    - **网址**: [Facebook Engineering Blog](https://engineering.fb.com/)
    - **简介**: Facebook 的工程博客介绍了他们在基础设施、数据中心、网络、人工智能和增强现实方面的创新。
    - **内容类型**: 基础设施、人工智能、数据分析、系统优化等。

4. **Google Cloud Blog**
    - **网址**: [Google Cloud Blog](https://cloud.google.com/blog)
    - **简介**: Google 云的官方博客，分享关于云计算、数据分析、机器学习和安全性方面的最新发展和实践。
    - **内容类型**: 云计算、数据管理、机器学习、开发工具等。

5. **AWS News Blog**
    - **网址**: [AWS News Blog](https://aws.amazon.com/blogs/aws/)
    - **简介**: Amazon Web Services 的官方博客，提供关于 AWS 服务、最佳实践和最新发布的详细信息。
    - **内容类型**: 云计算、服务器管理、DevOps、数据存储等。

6. **Airbnb Engineering & Data Science Blog**
    - **网址**: [Airbnb Engineering Blog](https://medium.com/airbnb-engineering)
    - **简介**: Airbnb 的工程和数据科学博客，分享他们在后端系统、数据科学、用户体验和基础设施方面的工作。
    - **内容类型**: 数据科学、用户体验、后端开发、系统架构等。

7. **Slack Engineering Blog**
    - **网址**: [Slack Engineering Blog](https://slack.engineering/)
    - **简介**: Slack 的工程博客，介绍他们在实时消息传递、API 集成、前端和后端开发方面的技术创新。
    - **内容类型**: 实时通信、API 开发、前端技术、后端架构等。

8. **Spotify Engineering Blog**
    - **网址**: [Spotify Engineering Blog](https://engineering.atspotify.com/)
    - **简介**: Spotify 的工程博客，探讨该公司在数据工程、机器学习、音频流处理和微服务架构方面的技术实践。
    - **内容类型**: 数据流处理、音频技术、机器学习、微服务等。

9. **Medium Engineering Blog**
    - **网址**: [Medium Engineering Blog](https://medium.engineering/)
    - **简介**: Medium 的工程博客，分享他们在内容分发、数据分析、性能优化和用户体验方面的经验和见解。
    - **内容类型**: 内容管理、数据分析、前端优化、用户体验等。

# REST API 认证方法 REST API Authentication Methods
![image](https://github.com/user-attachments/assets/413b57c8-fb9e-4641-ab56-5aed4da55f1e)

REST API 的认证方法多种多样，每种方法都有其独特的优点和适用场景。以下是几种常见的 REST API 认证方法：

1. **基本认证 (Basic Authentication)**
    - **概述**: 在 HTTP 请求头中使用 Base64 编码的用户名和密码进行认证。
    - **优点**: 实现简单，广泛支持。
    - **缺点**: 安全性较低，除非在 HTTPS 上使用，否则容易被窃听。
    - **示例**:
        ```http
        GET /api/resource HTTP/1.1
        Host: example.com
        Authorization: Basic dXNlcm5hbWU6cGFzc3dvcmQ=
        ```

2. **OAuth 2.0**
    - **概述**: 一个用于访问令牌的授权框架，支持多种授权方式（如授权码、密码、客户端凭证等）。
    - **优点**: 安全性高，支持细粒度权限控制和第三方授权。
    - **缺点**: 实现相对复杂，需要额外的授权服务器。
    - **示例**:
        ```http
        GET /api/resource HTTP/1.1
        Host: example.com
        Authorization: Bearer your_access_token
        ```

3. **JWT (JSON Web Token)**
    - **概述**: 使用 JSON 对象作为令牌，以声明特定数量的声明，通常用于会话管理。
    - **优点**: 自包含的令牌，减少了服务器存储负担，易于扩展。
    - **缺点**: 如果令牌没有妥善管理，可能带来安全隐患。
    - **示例**:
        ```http
        GET /api/resource HTTP/1.1
        Host: example.com
        Authorization: Bearer your_jwt_token
        ```

4. **API 密钥 (API Key)**
    - **概述**: 每个客户端被分配一个唯一的密钥，用于标识和认证客户端。
    - **优点**: 实现简单，易于管理。
    - **缺点**: 安全性较低，如果密钥泄露，可能被滥用。
    - **示例**:
        ```http
        GET /api/resource?api_key=your_api_key HTTP/1.1
        Host: example.com
        ```

5. **HMAC (Hash-based Message Authentication Code)**
    - **概述**: 使用密钥和消息的哈希值进行认证，确保消息的完整性和真实性。
    - **优点**: 安全性高，可以防止消息被篡改。
    - **缺点**: 实现相对复杂，需要客户端和服务器都支持 HMAC。
    - **示例**:
        ```http
        GET /api/resource HTTP/1.1
        Host: example.com
        Authorization: hmac username:hash
        ```

6. **OpenID Connect**
    - **概述**: 基于 OAuth 2.0 的身份认证协议，提供统一的用户身份验证。
    - **优点**: 提供用户信息，易于与 OAuth 2.0 集成。
    - **缺点**: 需要 OpenID 提供者支持，可能增加复杂性。
    - **示例**:
        ```http
        GET /api/resource HTTP/1.1
        Host: example.com
        Authorization: Bearer your_access_token
        ```

### 总结

选择合适的认证方法取决于具体的应用场景、安全需求和实现复杂度。以下是一些推荐：
- **基本认证**适用于简单、低安全性要求的应用。
- **OAuth 2.0**和**JWT**适用于需要高安全性和灵活权限控制的应用。
- **API 密钥**适用于简单、快速集成的应用。
- **HMAC**适用于需要高消息完整性和真实性的应用。
- **OpenID Connect**适用于需要统一用户身份认证的应用。


# Linux 启动过程图解Linux Boot Process Illustrated

#### 概述

Linux 的启动过程是从系统加电到操作系统内核完成初始化并开始运行用户空间程序的整个过程。它可以分为以下主要阶段：

1. BIOS/UEFI 初始化
2. 引导加载程序（Bootloader）
3. 内核引导
4. 初始化系统（Init System）

#### 详细流程图
![image](https://github.com/user-attachments/assets/d11b0f5b-31e7-44e3-8675-afd7dacb1e30)

```
+--------------------------------+
|           开机加电 (Power On)         |
+--------------------------------+
                |
                v
+--------------------------------+
|       BIOS/UEFI 初始化        |
|  (POST，自检，加载引导加载程序)     |
+--------------------------------+
                |
                v
+--------------------------------+
|        引导加载程序 (Bootloader)     |
|  (如 GRUB, LILO)                |
+--------------------------------+
                |
                v
+--------------------------------+
|            内核加载 (Kernel Loading)  |
|  (解压内核，启动内核)                |
+--------------------------------+
                |
                v
+--------------------------------+
|          内核初始化 (Kernel Initialization) |
|  (加载驱动程序，挂载根文件系统)        |
+--------------------------------+
                |
                v
+--------------------------------+
|        初始化系统 (Init System)        |
|  (如 systemd, SysVinit)            |
+--------------------------------+
                |
                v
+--------------------------------+
|         用户空间初始化          |
|   (User Space Initialization)  |
|  (启动用户空间进程，进入登录界面) |
+--------------------------------+
```

#### 详细步骤

1. **开机加电 (Power On)**
    - 计算机被加电，电源开始供应电力，硬件初始化。

2. **BIOS/UEFI 初始化**
    - **BIOS（Basic Input/Output System）** 或 **UEFI（Unified Extensible Firmware Interface）** 执行自检（POST，Power-On Self Test）。
    - 初始化硬件组件（如 CPU、内存、硬盘等）。
    - 查找引导设备，并加载引导加载程序到内存中。

3. **引导加载程序 (Bootloader)**
    - 常见的引导加载程序有 GRUB（GRand Unified Bootloader）和 LILO（Linux Loader）。
    - 显示引导菜单，允许用户选择不同的内核或操作系统。
    - 将选定的内核加载到内存中，并将控制权移交给内核。

4. **内核加载 (Kernel Loading)**
    - 内核被解压缩并加载到内存中。
    - 内核开始执行，初始化内存管理、进程管理、文件系统等核心功能。

5. **内核初始化 (Kernel Initialization)**
    - 内核启动初始的系统进程（如 `init`）。
    - 加载必要的驱动程序，检测并初始化所有硬件。
    - 挂载根文件系统（通常是 `/` 文件系统）。

6. **初始化系统 (Init System)**
    - 初始化系统是用户空间的第一个进程，PID 为 1。
    - 常见的初始化系统有 `systemd` 和 `SysVinit`。
    - 初始化系统根据配置文件（如 `/etc/inittab` 或 `systemd` 的单元文件）启动各种系统服务和守护进程。

7. **用户空间初始化 (User Space Initialization)**
    - 初始化系统启动各种用户空间进程和服务，如网络服务、数据库服务等。
    - 最后，启动登录界面（如 `getty` 提供的终端登录界面或图形登录界面）。

### 关键组件解释

- **BIOS/UEFI**: 基本输入输出系统，负责硬件初始化和引导加载程序的加载。
- **引导加载程序**: 负责加载内核，并将控制权移交给内核。
- **内核**: 操作系统的核心，负责系统资源管理和硬件抽象。
- **初始化系统 (Init System)**: 第一个用户空间进程，负责启动其他系统服务和守护进程。
- **用户空间**: 运行应用程序和服务的环境。

### 示例图

```plaintext
Power On
   |
   v
+--------------------+
| BIOS/UEFI          |
+--------------------+
   |
   v
+--------------------+
| Bootloader         |
| (GRUB, LILO, etc.) |
+--------------------+
   |
   v
+--------------------+
| Kernel             |
| (Linux)            |
+--------------------+
   |
   v
+--------------------+
| Init System        |
| (systemd, SysVinit)|
+--------------------+
   |
   v
+--------------------+
| User Space         |
| Initialization     |
+--------------------+
   |
   v
+--------------------+
| Login Prompt       |
+--------------------+
```

# SQL 联接 (SQL Joins) 工作原理 How do SQL Joins Work?

![image](https://github.com/user-attachments/assets/b2d38dbe-9f84-4f19-8bf6-a544259f563c)

### SQL 联接 (SQL Joins) 工作原理

SQL 联接（Join）用于在关系数据库中组合来自两个或多个表的数据。不同类型的联接可以根据需要选择和组合记录。以下是常见的 SQL 联接类型及其工作原理。

#### 1. 内联接 (INNER JOIN)

**定义**: 只返回两个表中满足联接条件的匹配行。

**示例**:
```sql
SELECT A.column1, B.column2
FROM TableA A
INNER JOIN TableB B
ON A.common_column = B.common_column;
```

**解释**: 这个查询会返回 `TableA` 和 `TableB` 中所有 `common_column` 相等的行。

```plaintext
TableA:
+------+--------------+
| ID   | Name         |
+------+--------------+
| 1    | Alice        |
| 2    | Bob          |
| 3    | Charlie      |
+------+--------------+

TableB:
+------+-------------+
| ID   | Department  |
+------+-------------+
| 1    | HR          |
| 2    | IT          |
| 4    | Finance     |
+------+-------------+

Result (INNER JOIN on ID):
+------+---------+
| Name | Department |
+------+---------+
| Alice| HR      |
| Bob  | IT      |
+------+---------+
```

#### 2. 左外联接 (LEFT JOIN 或 LEFT OUTER JOIN)

**定义**: 返回左表中所有行以及右表中满足联接条件的行；如果右表中没有匹配，则结果中包含空值（NULL）。

**示例**:
```sql
SELECT A.column1, B.column2
FROM TableA A
LEFT JOIN TableB B
ON A.common_column = B.common_column;
```

**解释**: 这个查询会返回 `TableA` 中所有的行，即使在 `TableB` 中没有匹配的行。

```plaintext
Result (LEFT JOIN on ID):
+--------+---------+
| Name   | Department |
+--------+---------+
| Alice  | HR      |
| Bob    | IT      |
| Charlie| NULL    |
+--------+---------+
```

#### 3. 右外联接 (RIGHT JOIN 或 RIGHT OUTER JOIN)

**定义**: 返回右表中所有行以及左表中满足联接条件的行；如果左表中没有匹配，则结果中包含空值（NULL）。

**示例**:
```sql
SELECT A.column1, B.column2
FROM TableA A
RIGHT JOIN TableB B
ON A.common_column = B.common_column;
```

**解释**: 这个查询会返回 `TableB` 中所有的行，即使在 `TableA` 中没有匹配的行。

```plaintext
Result (RIGHT JOIN on ID):
+--------+---------+
| Name   | Department |
+--------+---------+
| Alice  | HR      |
| Bob    | IT      |
| NULL   | Finance |
+--------+---------+
```

#### 4. 全外联接 (FULL JOIN 或 FULL OUTER JOIN)

**定义**: 返回两个表中所有的行，如果某一表中没有匹配则包含空值（NULL）。

**示例**:
```sql
SELECT A.column1, B.column2
FROM TableA A
FULL OUTER JOIN TableB B
ON A.common_column = B.common_column;
```

**解释**: 这个查询会返回 `TableA` 和 `TableB` 中所有的行，如果没有匹配则结果中包含空值。

```plaintext
Result (FULL OUTER JOIN on ID):
+--------+---------+
| Name   | Department |
+--------+---------+
| Alice  | HR      |
| Bob    | IT      |
| Charlie| NULL    |
| NULL   | Finance |
+--------+---------+
```

#### 5. 交叉联接 (CROSS JOIN)

**定义**: 返回两个表的笛卡尔积（即每个行的所有组合）。

**示例**:
```sql
SELECT A.column1, B.column2
FROM TableA A
CROSS JOIN TableB B;
```

**解释**: 这个查询会返回 `TableA` 中每一行和 `TableB` 中每一行的所有组合。

```plaintext
Result (CROSS JOIN):
+--------+---------+
| Name   | Department |
+--------+---------+
| Alice  | HR      |
| Alice  | IT      |
| Alice  | Finance |
| Bob    | HR      |
| Bob    | IT      |
| Bob    | Finance |
| Charlie| HR      |
| Charlie| IT      |
| Charlie| Finance |
+--------+---------+
```

### 总结

SQL 联接允许我们从多个表中获取和组合数据。选择适当的联接类型取决于具体的需求和数据关系：

- **INNER JOIN**: 只取匹配的行。
- **LEFT JOIN**: 取左表的所有行，右表中没有匹配则填充 NULL。
- **RIGHT JOIN**: 取右表的所有行，左表中没有匹配则填充 NULL。
- **FULL OUTER JOIN**: 取两表的所有行，没有匹配则填充 NULL。
- **CROSS JOIN**: 取两个表的所有组合。
 

# Netflix's Tech Stack
![image](https://github.com/user-attachments/assets/fcd4e2a9-54b1-4afb-b990-a704babf96d4)

# Top Architectural Styles
![image](https://github.com/user-attachments/assets/278792a5-544d-4d61-97e1-bb750314c5ab)

# What does ACID mean?
![image](https://github.com/user-attachments/assets/7302eb3c-77ea-4ac1-bc0b-9e97105dabc6)

# Oauth 2.0 Explained With Simple Terms
![image](https://github.com/user-attachments/assets/dbf5fd11-6080-4e69-ad83-2aad8e917c01)

# The Evolving Landscape of API Protocols in 2023
![image](https://github.com/user-attachments/assets/d18c85b5-8d38-4ace-a733-8e50a9672a4a)

# Explaining 8 Popular Network Protocols in 1 Diagram
![image](https://github.com/user-attachments/assets/553b1a99-8dd3-4e90-8fd4-7c989c4704f6)

# Data Pipelines Overview
![image](https://github.com/user-attachments/assets/ab065a35-a5f6-4f45-9b8c-ca2d6954b79a)

# CAP, BASE, SOLID, KISS, What do these acronyms mean?
![image](https://github.com/user-attachments/assets/e86221b5-4aaa-408f-b41c-22e857d5c10c)

# GET, POST, PUT... Common HTTP “verbs” in one figure
![image](https://github.com/user-attachments/assets/e1b7708d-58f8-410b-b0b3-1fd262f5ea40)

# How Do C++, Java, Python Work?
![image](https://github.com/user-attachments/assets/6a8ebc6f-3ec5-4b9c-abf5-df79cc72ad2b)

# Top 12 Tips for API Security
![image](https://github.com/user-attachments/assets/5a3bd2f6-6588-4a66-b9eb-9cb64413739d)

# Our recommended materials to crack your next tech interview
![image](https://github.com/user-attachments/assets/85fdac8e-b77b-48e2-9245-45124e861178)

# How To Release A Mobile App
![image](https://github.com/user-attachments/assets/5b364e14-cb45-4405-a396-d16782184efa)

# A handy cheat sheet for the most popular cloud services
![image](https://github.com/user-attachments/assets/29d83f18-db04-455f-b8ad-dd94cfe1b993)

# Best ways to test system functionality
![image](https://github.com/user-attachments/assets/b868f23e-eb39-4ce5-8be8-cd768863c856)

# Explaining JSON Web Token (JWT) to a 10 year old Kid
![image](https://github.com/user-attachments/assets/889f793a-cfb3-429d-a1fa-8b88b48d21fc)

# How do companies ship code to production?
![image](https://github.com/user-attachments/assets/91a1e990-c9c9-48e3-9818-b69b5daf21c0)

# How does Docker Work? Is Docker still relevant?
![image](https://github.com/user-attachments/assets/6bff3de6-ae2c-4fa9-b58f-bc7a4a39e854)

# System Design Blueprint: The Ultimate Guide
![image](https://github.com/user-attachments/assets/9ecfe0d6-ad03-4981-bbde-ccd55bceedcf)

# Key Concepts to Understand Database Sharding
![image](https://github.com/user-attachments/assets/6427df44-78ae-413a-950b-36cc1bd2ab7c)

# A nice cheat sheet of different monitoring infrastructure in cloud services
![image](https://github.com/user-attachments/assets/2983b5d0-4063-47fd-8df9-65eed7491a0e)

# Top 5 Software Architectural Patterns
![image](https://github.com/user-attachments/assets/34f54d56-ee63-44e2-b2bb-11010a6c1b57)

# OAuth 2.0 Flows
![image](https://github.com/user-attachments/assets/4e8ca6ac-5ec2-4650-b896-0d7cc1d3d7ac)

# How did AWS grow from just a few services in 2006 to over 200 fully-featured services?
![image](https://github.com/user-attachments/assets/d053c8e2-ab97-4ec7-9cee-d500b64018b1)

# What is GraphQL? Is it a replacement for the REST API?
![image](https://github.com/user-attachments/assets/3fd61b84-a519-4163-a7d5-81b341566edb)

# HTTPS, SSL Handshake, and Data Encryption Explained to Kids
![image](https://github.com/user-attachments/assets/ecd5bc1e-ef75-4d68-9eaf-617ba8dd5315)

# A nice cheat sheet of different databases in cloud services
![image](https://github.com/user-attachments/assets/5b9d21d5-53cc-4e86-94d0-a2dcc1e931fb)

# CI/CD Pipeline Explained in Simple Terms
![image](https://github.com/user-attachments/assets/46f1c57d-1506-42af-8d7b-6e6920726d28)

# What does API gateway do?
![image](https://github.com/user-attachments/assets/bc6c5468-40e2-4e50-b2eb-3bd0904f70ca)

# The Code Review Pyramid
![image](https://github.com/user-attachments/assets/47759d8f-9ad2-4177-a94e-544bf7a9aab2)

# A picture is worth a thousand words: 9 best practices for developing microservices
![image](https://github.com/user-attachments/assets/f34ec05d-e28f-4191-a384-946c8a8f8db8)

# The Code Review Pyramid
![image](https://github.com/user-attachments/assets/b0e12558-cb58-4dfc-a5b5-675285a81cac)

# What are the greenest programming languages?
![image](https://github.com/user-attachments/assets/4ecfc82b-b259-4be4-ac67-8f7acbd51c97)

# URL, URI, URN - Do you know the differences?
![image](https://github.com/user-attachments/assets/99f375f8-d35f-4991-a172-2e9f928430ce)

# What branching strategies does your team use?
![image](https://github.com/user-attachments/assets/6ece2459-e763-4d0f-b124-552a171f4a28)

# Linux file system explained
![image](https://github.com/user-attachments/assets/a0a8fa13-2373-4fd6-98a0-16c7dec26593)

# Do you believe that Google, Meta, Uber, and Airbnb put almost all of their code in one repository?
![image](https://github.com/user-attachments/assets/0ec0f22d-b7cc-4870-8cd5-d3dca680c72f)

# What are the data structures used in daily life?
![image](https://github.com/user-attachments/assets/995fcf43-1706-4c2e-93b8-05c85d8ad573)

# Why did Amazon Prime Video monitoring move from serverless to monolithic? How can it save 90% cost?
![image](https://github.com/user-attachments/assets/f6142b0c-24f6-4ea1-af58-90ac5f5cf20f)

# 18 Most-used Linux Commands You Should Know
![image](https://github.com/user-attachments/assets/e37d7aba-29b9-42c4-adf9-f4946240a143)

# Would it be nice if the code we wrote automatically turned into architecture diagrams?
![image](https://github.com/user-attachments/assets/fa083569-f3e4-4993-8ed2-4247a2c11a82)

# Netflix Tech Stack - Part 1 (CI/CD Pipeline)
![image](https://github.com/user-attachments/assets/576b0783-7c08-4a03-8c63-8b688920fde7)

# 18 Key Design Patterns Every Developer Should Know
![image](https://github.com/user-attachments/assets/130bf042-efaf-433c-9ecf-ab5b5eb78f15)

# How many API architecture styles do you know?
![image](https://github.com/user-attachments/assets/d9d0abc3-6d40-42c3-8229-0711f51c24a7)

# Visualizing a SQL query
![image](https://github.com/user-attachments/assets/aa9bc6f1-3d00-4f37-8e87-0ae0443b73fe)

# What distinguishes MVC, MVP, MVVM, MVVM-C, and VIPER architecture patterns from each other?
![image](https://github.com/user-attachments/assets/94f72efd-85fd-4542-8e9d-129952b5adf5)

# Almost every software engineer has used Git before, but only a handful know how it works :)
![image](https://github.com/user-attachments/assets/9c42f6e3-0cb6-42aa-94c5-c37d22a717d3)

# I read something unbelievable today: Levels. fyi scaled to millions of users using Google Sheets as a backend!
![image](https://github.com/user-attachments/assets/081f1157-7ec9-4d8e-b182-dc39f6c19ccd)

# Logging, tracing and metrics are 3 pillars of system observability
![image](https://github.com/user-attachments/assets/81ca06d3-d2ec-4a4d-a4d5-14e71a743db0)

# Internet Traffic Routing Policies
![image](https://github.com/user-attachments/assets/04d42a9e-6a33-448c-83a9-487212888fef)

# Subjects that should be mandatory in schools
![image](https://github.com/user-attachments/assets/96325f3a-c118-47d7-a96f-230c33c26082)

# Do you know all the components of a URL?
![image](https://github.com/user-attachments/assets/2129b054-0758-484f-b326-ea4b766c05fa)

# What are the differences between cookies and sessions?
![image](https://github.com/user-attachments/assets/99abc397-5fad-4921-b309-c3cceb1eed3a)

# How do DevOps, NoOps change the software development lifecycle (SDLC)?
![image](https://github.com/user-attachments/assets/db883b47-2c47-4e69-bea3-0e4a8eb29356)

# Popular interview question: What is the difference between Process and Thread?
![image](https://github.com/user-attachments/assets/925c0c76-293c-4b14-a2d4-a76dcff98f85)

# Top 6 Load Balancing Algorithms
![image](https://github.com/user-attachments/assets/4b3174a0-b6f0-4980-9b82-8f42bc0770dd)

# Symmetric encryption vs asymmetric encryption
![image](https://github.com/user-attachments/assets/07685bdc-da7c-461d-881f-1e58d68759f7)

# How does Redis persist data?
![image](https://github.com/user-attachments/assets/c2907735-da30-4028-a919-e0ad5025e70b)

# IBM MQ -> RabbitMQ -> Kafka ->Pulsar, How do message queue architectures evolve?
![image](https://github.com/user-attachments/assets/07758618-8961-4ed4-bda0-4810fabf05a9)

# Top 4 Kubernetes Service Types in one diagram
![image](https://github.com/user-attachments/assets/ef7c20f3-f813-4ae1-b5cd-2edd5e0bf730)

# Explaining 5 unique ID generators in distributed systems
![image](https://github.com/user-attachments/assets/9cbb3bc4-0176-462e-b850-5d61a3a2b34e)

# How Do C++, Java, and Python Function?
![image](https://github.com/user-attachments/assets/42f1251a-3f66-4fec-8152-7187fe4679a1)

# How will you design the Stack Overflow website?
![image](https://github.com/user-attachments/assets/8101b249-b560-4def-86e7-8244225a8f92)

# Explain the Top 6 Use Cases of Object Stores
![image](https://github.com/user-attachments/assets/c3d53fff-23f5-4f5a-9f42-6f28fbe78a9d)

# API Vs SDK!
![image](https://github.com/user-attachments/assets/6e41b83f-536f-4a6b-86ab-c6452ca1f09f)

# A picture is worth a thousand words: 9 best practices for developing microservices
![image](https://github.com/user-attachments/assets/22106969-9a0f-4fbf-a9e3-e8b510898157)

# Proxy Vs reverse proxy
![image](https://github.com/user-attachments/assets/050bf553-1552-49e9-935c-0da59b73f4a6)

# Git Vs Github
![image](https://github.com/user-attachments/assets/33e388a9-d45b-47ea-acbb-b1bb22cad37b)

# Which latency numbers should you know
![image](https://github.com/user-attachments/assets/030ebd2e-67d6-44c2-ab64-fe795698f224)

# Eight Data Structures That Power Your Databases. Which one should we pick?
![image](https://github.com/user-attachments/assets/6bbaf6ed-732d-42d2-a68c-562b6c93e390)

# How Git Commands Work
![image](https://github.com/user-attachments/assets/530dc2dd-1e7c-4727-8f16-58f7dbf1f2cf)

# How to store passwords safely in the database and how to validate a password?
<img width="400" alt="image" src="https://github.com/user-attachments/assets/830c3fbf-884e-4bde-87de-29c289bcd91f">

# What is a database? What are some common types of databases?
![image](https://github.com/user-attachments/assets/b22291e9-2aa7-4822-8a50-6b63bd52f1e2)

# How does Docker Work? Is Docker still relevant? 
![image](https://github.com/user-attachments/assets/535fd11c-963c-4e50-916f-14fa9be98208)

# Docker vs. Kubernetes. Which one should we use?
![image](https://github.com/user-attachments/assets/94467f43-482a-4f0b-9fec-3072feac10b4)

# Writing Code that Runs on All Platforms
![image](https://github.com/user-attachments/assets/c2ffffdb-f8d2-401b-8caf-01144f5c23de)

# HTTP Status Code You Should Know
![image](https://github.com/user-attachments/assets/1231fb08-a751-4a9b-906e-000cbf8ca0f6)

# Docker 101: Streamlining App Deployment
![image](https://github.com/user-attachments/assets/af89a5d3-e550-4fbd-9d6a-371a7b5ba97c)

# Git Merge vs. Rebase vs. Squash Commit
![image](https://github.com/user-attachments/assets/9056bb6d-2df3-4b5c-8155-4cfbf7ec7d99)

# Cloud Network Components Cheat Sheet
![image](https://github.com/user-attachments/assets/f5b19050-8003-4b90-9dc1-73e42c43868a)

# SOAP vs REST vs GraphQL vs RPC
![image](https://github.com/user-attachments/assets/91f040ac-e4f7-4214-99d2-61cca03bedb6)

# 10 Key Data Structures We Use Every Day
![image](https://github.com/user-attachments/assets/36615c2b-97c4-4686-901c-facff11a7ea5)

# What does a typical microservice architecture look like?
![image](https://github.com/user-attachments/assets/6babdb12-0b4c-45d2-96bd-d8c46ce31461)

# Uber Tech Stack
![image](https://github.com/user-attachments/assets/890d6569-d489-4cea-aabe-565c25dedaf0)

# Top 5 Caching Strategies
![image](https://github.com/user-attachments/assets/f97ee043-dbaf-48f2-9ea2-684c663d88b3)

# How many message queues do you know?
![image](https://github.com/user-attachments/assets/9821cf82-f644-4f5f-85d2-5e12c73cee66)

# Why is Kafka fast?
![image](https://github.com/user-attachments/assets/b418ddba-4a3d-4e44-bdc1-2258aaca4789)

# How slack decides to send a notification
![image](https://github.com/user-attachments/assets/b7256e36-69c5-48f9-8ca7-25f359b37b24)

# Kubernetes Tools Ecosystem
![image](https://github.com/user-attachments/assets/67a51d67-c277-49ad-aaa5-76dd65c8d477)

# Cloud Native Landscape
![image](https://github.com/user-attachments/assets/1e8850d6-e369-4f8c-af11-0f0d331c3abd)

# How does VISA work when we swipe a credit card at a merchant’s shop?
![image](https://github.com/user-attachments/assets/d4d798cd-8a46-41ee-99ab-636741e7664c)

# What tech stack is commonly used for microservices?
![image](https://github.com/user-attachments/assets/7652cd43-609c-4cde-b7ba-42564a71c8d5)

# How do we transform a system to be Cloud Native?
![image](https://github.com/user-attachments/assets/ca53adee-79ae-400c-8539-5399d3550490)

# Explaining Sessions, Tokens, JWT, SSO, and OAuth in One Diagram
![image](https://github.com/user-attachments/assets/0a311235-9e89-4d91-a2f1-606cf75112f6)

# Most Used Linux Commands Map
![image](https://github.com/user-attachments/assets/a37b00c0-ef2c-4ab4-a22a-1e5d3da3af97)

# What is Event Sourcing? How is it different from normal CRUD design?
![image](https://github.com/user-attachments/assets/923e1806-1c2f-49fa-8902-6faa9db2a4c1)

# What is k8s (Kubernetes)?
![image](https://github.com/user-attachments/assets/8f63265a-0739-4b40-b6fd-002b0bbf5f29)

# How does Git Work?
![image](https://github.com/user-attachments/assets/bc66da92-aeb8-449c-85c2-8587d87cd25e)

# How does Google Authenticator (or other types of 2-factor authenticators) work?
<img width="400" alt="image" src="https://github.com/user-attachments/assets/f7b39177-4fe2-4cd8-980e-55a2a655e2f0">

# IaaS, PaaS, Cloud Native How do we get here?
![image](https://github.com/user-attachments/assets/34e4fdab-4785-4bb8-b907-c6af080492bb)

# How does ChatGPT work?
![image](https://github.com/user-attachments/assets/43c0be8a-bd62-4ef7-9802-5204965c5a0d)

# Top Hidden Costs of Cloud Providers
![image](https://github.com/user-attachments/assets/37d9a537-2bf4-4efa-aca9-eb790ab23f8c)

# Algorithms You Should Know Before You Take System Design Interviews
![image](https://github.com/user-attachments/assets/78c7fb3e-b836-43ce-8d09-ed352f49ed0a)

# Understanding Database Types
![image](https://github.com/user-attachments/assets/2b56f030-7f6d-4a1d-8083-d44df181b5c3)

# How does gRPC work?
![image](https://github.com/user-attachments/assets/d1090ab5-a545-43d5-a437-6d14d20e9e74)

# How does a Password Manager such as 1Password or Lastpass work? How does it keep our passwords safe?
![image](https://github.com/user-attachments/assets/ae2954c0-a7d5-4ced-8662-09f43a588f62)

# Types of Software Engineers and Their Typically Required Skills
![image](https://github.com/user-attachments/assets/d508b558-6113-4bc4-8cd1-ba25ed3ae249)

# How does REST API work?
![image](https://github.com/user-attachments/assets/8b9e5a95-bf9b-4780-b064-f8355aac89c5)

# Session, cookie, JWT, token, SSO, and OAuth 2.0 - what are they?
![image](https://github.com/user-attachments/assets/41612aa5-dfde-4b71-854e-0f7223ff9755)

# Linux commands illustrated on one page!
![image](https://github.com/user-attachments/assets/5315b9a2-3512-4318-9421-839b4aa6142c)

# The Payments Ecosystem
![image](https://github.com/user-attachments/assets/f86599f9-900f-40a3-84f2-98e5abd39cf8)

# Algorithms You Should Know Before You Take System Design Interviews (updated list)
![image](https://github.com/user-attachments/assets/f073c8e9-cf40-4cbe-8759-47a1172d01c9)

# How is data transmitted between applications?
![image](https://github.com/user-attachments/assets/63597933-fc4a-4c0c-85ac-230665687934)

# Cloud Native Anti Patterns
![image](https://github.com/user-attachments/assets/4f000b3a-277d-4e1b-ba71-0d404a94c65d)

# Uber Tech Stack - CI/CD
![image](https://github.com/user-attachments/assets/967eed8b-497a-4e86-a7e7-e0bba4268044)

# How Discord Stores Trillions Of Messages
![image](https://github.com/user-attachments/assets/094b1938-a78f-41b5-b112-23d69f15ff52)

# How to diagnose a mysterious process that’s taking too much CPU, memory, IO, etc?.
![image](https://github.com/user-attachments/assets/ef42bd0c-0bca-4cad-be7f-8eafc01f64cf)

# How does Chrome work?
![image](https://github.com/user-attachments/assets/bbc990f7-3759-4ee6-94d7-098ae164a240)

# Differences in Event SOurcing System Design
![image](https://github.com/user-attachments/assets/100a5733-aec5-42dc-b7ed-fd483cb6b117)

# Firewall explained to Kids and Adults
![image](https://github.com/user-attachments/assets/f91639c8-8e15-469e-9011-b2a3111ed66e)

# Paradigm Shift: How Developer to Tester Ratio Changed From 1:1 to 100:1
<img width="400" alt="image" src="https://github.com/user-attachments/assets/761565cb-8965-46ed-83a1-496874610699">

# Why is PostgreSQL voted as the most loved database by developers?
![image](https://github.com/user-attachments/assets/f5f42d12-0111-486a-906c-40abbe3729e3)

# 8 Key OOP Concepts Every Developer Should Know
![image](https://github.com/user-attachments/assets/08dfd068-4aba-4b6b-9c66-e131e96429d5)

# Top 6 most commonly used Server Types
![image](https://github.com/user-attachments/assets/b44c7875-15b4-4899-94d3-652af09ae588)

# DevOps vs. SRE vs. Platform Engineering. Do you know the differences?
![image](https://github.com/user-attachments/assets/a84460d0-5725-45c5-bcd8-decfdba43974)

# 5 important components of Linux
![image](https://github.com/user-attachments/assets/de7013df-99c1-464e-b39f-ed3a7938841e)

# How to scale a website to support millions of users?
![image](https://github.com/user-attachments/assets/f614c13a-eca0-4f07-8941-3ad288d05f32)

# What is FedNow (instant payment)
![image](https://github.com/user-attachments/assets/5de8c125-cf13-40bd-a8a9-bd48c40fe9eb)

# 5 ways of Inter-Process Communication
![image](https://github.com/user-attachments/assets/33ce5bff-c6c7-480d-858f-468656523797)

# What is a webhook?
![image](https://github.com/user-attachments/assets/8cbf5b5e-595c-444e-b9c8-a425785096df)

# What tools does your team use to ship code to production and ensure code quality?
![image](https://github.com/user-attachments/assets/92ea8f48-0cb1-400c-a53b-cbf3cb9b6887)

# Stack Overflow's Architecture: A Very Interesting Case Study
![image](https://github.com/user-attachments/assets/5ce1a86c-f234-4718-a4ec-8557b2549dcd)

# Are you familiar with the Java Collection Framework?
![image](https://github.com/user-attachments/assets/6b54f816-97d8-4d78-a76d-3de6d681c505)

# Twitter 1.0 Tech Stack
![image](https://github.com/user-attachments/assets/e0e0b5b1-18df-4455-b6c1-42dacdd957b5)

# Linux file permission illustrated
![image](https://github.com/user-attachments/assets/6faa32b5-e40b-4130-a71b-eda52dcb867c)

# What are the differences between a data warehouse and a data lake?
![image](https://github.com/user-attachments/assets/9e15195a-176e-4a0e-9985-34fbdd9929cb)

# 10 principles for building resilient payment systems (by Shopify).
![image](https://github.com/user-attachments/assets/1ed867c2-fe4c-4064-8298-1af63c010647)

# Kubernetes Periodic Table
![image](https://github.com/user-attachments/assets/27d7c396-55c6-4d39-b7cd-e1f7512e1ce6)

# Evolution of the Netflix API Architecture
![image](https://github.com/user-attachments/assets/87e6b54a-dc66-4239-b3f3-331214ac2758)

# Where do we cache data?
![image](https://github.com/user-attachments/assets/48e9e272-5902-434f-b5e3-36a127e14c53)

# Top 7 Most-Used Distributed System Patterns
![image](https://github.com/user-attachments/assets/8f589c58-97a4-499a-8024-55f490b2369f)

# How much storage could one purchase with the price of a Tesla Model S
![image](https://github.com/user-attachments/assets/c3a416f4-8821-4737-b031-42de20945947)

# How to choose between RPC and RESTful?
![image](https://github.com/user-attachments/assets/48c99f62-34ea-463b-b776-8957d8aefa14)

# Netflix Tech Stack - Databases
![image](https://github.com/user-attachments/assets/ed5cfe0f-7818-456d-abb1-98147ba5e85f)

# The 10 Algorithms That Dominate Our World
![image](https://github.com/user-attachments/assets/5640c096-ed24-4509-8cf4-3d25345b532c)

# What is the difference between “pull” and “push” payments?
![image](https://github.com/user-attachments/assets/f6df0e13-5010-4776-808f-d153bbf0920b)

# ChatGPT - timeline
![image](https://github.com/user-attachments/assets/f45c5940-d0c6-4e05-8f87-609a04f715a5)

# Why did Amazon Prime Video monitoring move from serverless to monolithic? How can it save 90% cost?
![image](https://github.com/user-attachments/assets/8f2d4c09-9644-483b-9e1e-052c1f5d2ffe)

# What is the journey of a Slack message?
![image](https://github.com/user-attachments/assets/39650677-6a86-4eff-a9e0-b6c29c6c1e1a)

# How does GraphQL work in the real world?
![image](https://github.com/user-attachments/assets/53f69aba-de5a-498b-98bd-4ebd208d863a)

# Important Things About HTTP Headers You May Not Know!
![image](https://github.com/user-attachments/assets/619bf1dd-8d1d-4f79-9ec9-c985c5d86451)

# Think you know everything about McDonald's? What about its event-driven architecture
![image](https://github.com/user-attachments/assets/8837a2fb-af32-44c8-ae99-742f95737149)

# How ChatGPT works technically

# Choosing the right database is probably the most important technical decision a company will make.

#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#





















































