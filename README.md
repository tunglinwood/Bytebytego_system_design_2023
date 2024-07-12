
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
 

# Netflix 技术栈 Netflix's Tech Stack
![image](https://github.com/user-attachments/assets/fcd4e2a9-54b1-4afb-b990-a704babf96d4)

Netflix 作为全球领先的流媒体服务提供商，其技术栈覆盖了广泛的领域，包括前端、后端、数据处理、微服务架构、内容分发等。以下是 Netflix 技术栈的一些关键组成部分：

#### 前端技术

1. **React**
    - **用途**: 用于构建用户界面，特别是 Netflix 的网页端。
    - **特点**: 组件化、虚拟 DOM、单向数据流。

2. **Node.js**
    - **用途**: 用于服务器端 JavaScript 运行时，支持高并发和 I/O 密集型任务。
    - **特点**: 非阻塞、事件驱动、适合实时应用。

#### 后端技术

1. **Java**
    - **用途**: 后端服务的主要编程语言，用于构建核心微服务。
    - **特点**: 跨平台、性能优越、庞大的生态系统。

2. **Spring Boot**
    - **用途**: 基于 Java 的微服务框架，简化了应用程序的配置和部署。
    - **特点**: 自动配置、独立运行、集成良好。

3. **Python**
    - **用途**: 用于数据分析、机器学习、自动化脚本等。
    - **特点**: 易于学习、丰富的库和框架、广泛应用于数据科学领域。

#### 数据存储

1. **Apache Cassandra**
    - **用途**: 分布式 NoSQL 数据库，适用于处理大量的结构化数据。
    - **特点**: 高可用性、线性可扩展性、无单点故障。

2. **Amazon RDS**
    - **用途**: 托管关系数据库服务，支持多种数据库引擎（如 MySQL、PostgreSQL）。
    - **特点**: 高可用性、自动备份和恢复、易于扩展。

3. **Amazon S3**
    - **用途**: 对象存储服务，用于存储和检索任意数量的数据。
    - **特点**: 高可用性、持久性、成本效益。

#### 数据处理

1. **Apache Kafka**
    - **用途**: 分布式流处理平台，用于实时数据流处理和事件驱动架构。
    - **特点**: 高吞吐量、低延迟、持久性存储。

2. **Apache Spark**
    - **用途**: 分布式数据处理引擎，用于大规模数据处理和机器学习。
    - **特点**: 内存计算、高性能、丰富的 API 支持。

3. **Presto**
    - **用途**: 分布式 SQL 查询引擎，用于对大数据集进行交互式查询。
    - **特点**: 高性能、支持多种数据源、低延迟。

#### 微服务和容器化

1. **Docker**
    - **用途**: 容器化平台，用于创建、部署和运行容器。
    - **特点**: 轻量级、隔离性、便于持续集成和部署。

2. **Kubernetes**
    - **用途**: 容器编排平台，用于自动化部署、扩展和管理容器化应用。
    - **特点**: 高可用性、自动化运维、可扩展性。

3. **Eureka**
    - **用途**: Netflix 开源的服务发现工具，用于微服务注册和发现。
    - **特点**: 动态服务注册、高可用性、弹性。

#### 内容分发网络 (CDN)

1. **Netflix Open Connect**
    - **用途**: Netflix 自己的内容分发网络，用于高效传递视频内容。
    - **特点**: 提高内容传递速度、减少带宽成本、提升用户体验。

#### 数据科学与机器学习

1. **TensorFlow**
    - **用途**: 开源的机器学习框架，用于构建和训练深度学习模型。
    - **特点**: 灵活性、可扩展性、丰富的社区支持。

2. **Apache Hive**
    - **用途**: 数据仓库基础设施，提供数据查询和分析功能。
    - **特点**: SQL 兼容、高扩展性、支持大数据处理。

#### 监控与日志

1. **Prometheus**
    - **用途**: 开源监控和报警系统，用于实时系统监控。
    - **特点**: 多维数据模型、强大的查询语言、可视化支持。

2. **Grafana**
    - **用途**: 开源数据可视化和监控平台，用于展示监控数据。
    - **特点**: 丰富的图表类型、灵活的面板配置、广泛的数据源支持。

3. **ELK Stack (Elasticsearch, Logstash, Kibana)**
    - **用途**: 日志管理和分析平台，用于收集、存储和可视化日志数据。
    - **特点**: 强大的搜索和分析能力、灵活的数据处理管道、直观的可视化。

### 总结

Netflix 的技术栈涵盖了从前端到后端、从数据存储到数据处理、从微服务到内容分发的各个方面。这些技术组件的结合使 Netflix 能够提供高性能、高可用性和高扩展性的流媒体服务。

# 顶级架构风格 Top Architectural Styles
![image](https://github.com/user-attachments/assets/278792a5-544d-4d61-97e1-bb750314c5ab)

在软件系统设计中，架构风格决定了系统组件的组织方式、组件之间的交互方式以及系统的整体行为。以下是一些最常见的架构风格：

#### 1. 分层架构 (Layered Architecture)

**定义**: 系统被划分为多个层，每一层都有特定的职责。常见的层次包括表示层（UI）、业务逻辑层（BLL）、数据访问层（DAL）和数据层（Database）。

**优点**:
- 模块化，易于理解和维护。
- 各层之间松耦合，便于替换和重用。

**缺点**:
- 可能导致性能开销，特别是跨层调用频繁时。
- 层次之间的严格依赖可能导致灵活性不足。

**示例**:
```
+-------------+          +-------------+
| Presentation|          |     UI      |
+-------------+          +-------------+
        |                      |
+-------------+          +-------------+
|  Business   | <----->  |  Business   |
|  Logic      |          |  Logic      |
+-------------+          +-------------+
        |                      |
+-------------+          +-------------+
|  Data Access| <----->  |  Data Access|
+-------------+          +-------------+
        |                      |
+-------------+          +-------------+
|  Database   |          |  Database   |
+-------------+          +-------------+
```

#### 2. 客户端-服务器架构 (Client-Server Architecture)

**定义**: 系统分为客户端和服务器两部分，客户端发出请求，服务器处理请求并返回响应。

**优点**:
- 清晰的职责分离。
- 易于扩展，客户端和服务器可以独立升级。

**缺点**:
- 网络延迟可能影响性能。
- 服务器可能成为单点故障。

**示例**:
```
Client <----> Server
```

#### 3. 事件驱动架构 (Event-Driven Architecture)

**定义**: 系统由事件生产者和事件消费者组成，事件驱动的方式进行通信。

**优点**:
- 松耦合，消费者和生产者相互独立。
- 高扩展性，适合处理大量并发请求。

**缺点**:
- 调试和测试可能比较复杂。
- 需要良好的事件管理和错误处理机制。

**示例**:
```
+------------+     Event     +------------+
|  Producer  | ------------> |  Consumer  |
+------------+               +------------+
```

#### 4. 微服务架构 (Microservices Architecture)

**定义**: 将应用程序划分为多个独立的服务，每个服务实现特定的业务功能，并通过轻量级的通信机制（如 HTTP、消息队列）进行交互。

**优点**:
- 高可维护性和可扩展性。
- 易于部署和独立开发。

**缺点**:
- 复杂的分布式系统管理。
- 服务间的通信开销和数据一致性问题。

**示例**:
```
+--------+     +--------+     +--------+
| Service| <-> | Service| <-> | Service|
+--------+     +--------+     +--------+
```

#### 5. 面向服务架构 (Service-Oriented Architecture, SOA)

**定义**: 使用服务作为基本单元，服务通过定义良好的接口（通常是 SOAP 或 REST）进行通信。

**优点**:
- 促进代码重用和松耦合。
- 支持跨平台和跨语言的服务调用。

**缺点**:
- 比较重的通信协议（如 SOAP）可能导致性能开销。
- 需要良好的服务治理和管理机制。

**示例**:
```
+---------+     +---------+     +---------+
| Service | <-> | Service | <-> | Service |
+---------+     +---------+     +---------+
```

#### 6. REST 架构 (Representational State Transfer)

**定义**: 一种基于资源的架构风格，使用 HTTP 方法（GET、POST、PUT、DELETE）进行操作，每个资源都有唯一的 URI。

**优点**:
- 简单易用，广泛采用。
- 良好的可扩展性和可维护性。

**缺点**:
- 不适合复杂的事务处理。
- 过度使用可能导致网络开销。

**示例**:
```
Client <----> RESTful API <----> Server
```

#### 7. 管道-过滤器架构 (Pipes and Filters Architecture)

**定义**: 系统由一系列过滤器（Filters）和管道（Pipes）组成，每个过滤器处理输入数据并产生输出数据，管道用于传递数据。

**优点**:
- 高可重用性和可扩展性。
- 适合数据流处理和转换。

**缺点**:
- 数据格式转换可能带来性能开销。
- 系统调试和监控可能比较复杂。

**示例**:
```
+--------+     +--------+     +--------+
| Filter | --> | Filter | --> | Filter |
+--------+     +--------+     +--------+
```

#### 8. 抽象工厂架构 (Abstract Factory Pattern)

**定义**: 提供一个接口，创建一系列相关或依赖对象，而无需指定具体类。

**优点**:
- 提高代码灵活性和可维护性。
- 避免类之间的紧耦合。

**缺点**:
- 增加了系统的复杂性。
- 需要理解设计模式的使用。

**示例**:
```java
interface GUIFactory {
    Button createButton();
    Checkbox createCheckbox();
}

class WinFactory implements GUIFactory {
    public Button createButton() {
        return new WinButton();
    }
    public Checkbox createCheckbox() {
        return new WinCheckbox();
    }
}
```

### 总结

不同的架构风格适用于不同类型的应用和需求。选择合适的架构风格可以提高系统的可维护性、可扩展性和性能。在实际项目中，通常会结合使用多种架构风格，以实现最佳效果。

# ACID 的含义 What does ACID mean?
![image](https://github.com/user-attachments/assets/7302eb3c-77ea-4ac1-bc0b-9e97105dabc6)

在数据库系统中，ACID 是指事务处理的四个关键属性：原子性（Atomicity）、一致性（Consistency）、隔离性（Isolation）和持久性（Durability）。这些属性确保了数据库中的数据在事务处理过程中保持完整和可靠。

#### 1. 原子性 (Atomicity)

**定义**: 事务中的所有操作要么全部完成，要么全部不完成。换句话说，事务是不可分割的操作单元。

**示例**: 
在银行转账过程中，从账户 A 转账到账户 B，涉及两个操作：从账户 A 中扣钱和向账户 B 中存钱。原子性保证了这两个操作要么全部成功，要么全部失败。

**解释**:
```plaintext
BEGIN TRANSACTION;
    UPDATE accounts SET balance = balance - 100 WHERE account_id = 'A';
    UPDATE accounts SET balance = balance + 100 WHERE account_id = 'B';
COMMIT;
```
如果任意一个操作失败，整个事务将回滚，两个账户的余额都不会改变。

#### 2. 一致性 (Consistency)

**定义**: 事务执行前后，数据库必须从一个一致状态转换到另一个一致状态。任何事务的执行都不会破坏数据库的完整性约束。

**示例**: 
在银行转账的例子中，一致性要求在整个过程中，账户的总余额保持不变。

**解释**:
```plaintext
账户 A 和 账户 B 的总余额在事务执行前后必须保持一致。
```

#### 3. 隔离性 (Isolation)

**定义**: 并发执行的事务相互之间不能干扰，每个事务在执行时都好像是在单独访问数据库。隔离性保证了事务的中间状态对其他事务不可见。

**示例**: 
在多个用户同时进行银行转账操作时，隔离性保证每个转账操作不会影响其他操作。

**解释**:
```plaintext
用户 1 和 用户 2 同时从账户 A 转账到各自的账户，隔离性保证了两个事务之间不会发生数据冲突或不一致。
```

#### 4. 持久性 (Durability)

**定义**: 一旦事务提交，其结果必须永久保存在数据库中，即使系统发生故障（如电源中断或系统崩溃）。

**示例**: 
在银行转账操作完成并提交后，即使系统崩溃，转账结果也会被永久保存。

**解释**:
```plaintext
事务完成后，从账户 A 扣除的金额和向账户 B 增加的金额会被永久记录在数据库中。
```

### 总结

ACID 属性确保了数据库事务的可靠性和一致性：

- **原子性**: 确保事务要么完全执行，要么完全不执行。
- **一致性**: 确保事务执行前后数据库保持一致状态。
- **隔离性**: 确保并发事务之间互不干扰。
- **持久性**: 确保事务一旦提交，其结果永久保存。

这些属性是构建可靠和高性能数据库系统的基石。

# OAuth 2.0 简单解释 Oauth 2.0 Explained With Simple Terms
![image](https://github.com/user-attachments/assets/dbf5fd11-6080-4e69-ad83-2aad8e917c01)

OAuth 2.0 是一种授权框架，它允许应用程序在用户允许的情况下，安全地访问用户的资源（例如，用户的个人信息、照片或其他数据）而不需要暴露用户的登录凭据。以下是对 OAuth 2.0 的简单解释：

#### 基本概念

- **资源拥有者（Resource Owner）**: 通常是最终用户，拥有要被访问的资源。
- **客户端（Client）**: 希望访问资源的应用程序。例如，一个希望访问用户照片的照片编辑应用。
- **授权服务器（Authorization Server）**: 验证资源拥有者的身份，并在其同意后发放访问令牌（Access Token）。通常由资源拥有者信任的一方提供，例如 Google 或 Facebook。
- **资源服务器（Resource Server）**: 托管资源的服务器，通过访问令牌验证和提供资源。通常与授权服务器是同一个实体。

#### 工作流程

1. **用户同意授权**: 用户希望使用某个应用（客户端），客户端要求访问用户的资源。用户被重定向到授权服务器，在那里用户可以登录并同意授权。
   
2. **客户端请求授权码**: 用户同意授权后，授权服务器生成一个授权码（Authorization Code），并将其发送给客户端。

3. **客户端请求访问令牌**: 客户端使用授权码向授权服务器请求访问令牌。授权服务器验证授权码的有效性后，生成并返回访问令牌。

4. **客户端访问资源**: 客户端使用访问令牌向资源服务器请求访问资源。资源服务器验证令牌的有效性后，提供资源。

#### 示例

假设你在使用一个照片编辑应用，该应用希望访问你存储在 Google Photos 中的照片。流程如下：

1. **用户同意授权**:
    - 你打开照片编辑应用并选择“从 Google Photos 导入照片”。
    - 应用将你重定向到 Google 的授权页面，要求你登录并允许该应用访问你的 Google Photos。
    
    ```plaintext
    App: "我需要访问你的 Google Photos，请登录并授权。"
    ```

2. **客户端请求授权码**:
    - 你在 Google 授权页面登录并同意授权。
    - Google 授权服务器生成一个授权码，并将其返回给照片编辑应用。

    ```plaintext
    Google: "用户已授权，给你一个授权码。"
    ```

3. **客户端请求访问令牌**:
    - 照片编辑应用将授权码发送给 Google 授权服务器，请求访问令牌。
    - Google 验证授权码并返回访问令牌。

    ```plaintext
    App: "这是授权码，给我一个访问令牌。"
    Google: "验证通过，这是访问令牌。"
    ```

4. **客户端访问资源**:
    - 照片编辑应用使用访问令牌请求访问你的 Google Photos。
    - Google Photos 服务器验证令牌，并返回你的照片数据给应用。

    ```plaintext
    App: "这是访问令牌，我要访问用户的照片。"
    Google Photos: "令牌有效，这是用户的照片数据。"
    ```

#### OAuth 2.0 的好处

- **安全性**: 用户不需要将登录凭据（如用户名和密码）提供给第三方应用。
- **授权控制**: 用户可以控制每个应用访问其资源的权限，并随时撤销授权。
- **简化的开发**: 应用开发者可以轻松地集成流行的服务（如 Google、Facebook）的授权功能。

### 总结

OAuth 2.0 通过授权码和访问令牌的机制，安全地授权第三方应用访问用户的资源，同时保护用户的登录凭据。这个框架被广泛应用于各种 Web 和移动应用，提供了一个安全且用户友好的授权方式。

# 2023年API协议的演变格局 The Evolving Landscape of API Protocols in 2023
![image](https://github.com/user-attachments/assets/d18c85b5-8d38-4ace-a733-8e50a9672a4a)

随着技术的发展和需求的变化，API协议也在不断演变，以更好地满足各种应用场景和需求。2023年，API协议的格局展示出以下几种主要趋势和演变方向：

#### 1. REST (Representational State Transfer)

**现状**: REST 依然是最流行的API设计风格，基于HTTP协议，使用HTTP动词（如GET、POST、PUT、DELETE）进行资源操作。

**演变**:
- 增强安全性：更多应用采用OAuth 2.0和JWT（JSON Web Tokens）来保护REST API。
- 更加标准化：OpenAPI（以前称为Swagger）在API设计和文档编制中广泛使用，使得API接口更加标准和易于理解。

**特点**:
- 简单、无状态、易于实现和理解。
- 适用于CRUD（创建、读取、更新、删除）操作。

#### 2. GraphQL

**现状**: 由Facebook开发，GraphQL允许客户端根据需要查询数据，避免了传统REST API的过度获取或不足获取问题。

**演变**:
- 广泛采用：越来越多的公司和开发者选择GraphQL用于构建API，尤其是在需要灵活数据查询的场景中。
- 工具链发展：如Apollo和Relay等GraphQL客户端工具和服务在性能优化、错误处理和缓存等方面不断进步。

**特点**:
- 客户端控制数据查询，避免数据冗余。
- 强类型系统，易于验证和调试。

#### 3. gRPC (Google Remote Procedure Call)

**现状**: 由Google开发，gRPC是一种高性能、通用的开源RPC框架，使用HTTP/2协议和Protocol Buffers序列化。

**演变**:
- 高性能需求：在需要低延迟和高吞吐量的场景中，gRPC变得越来越受欢迎，如微服务通信、实时数据处理等。
- 多语言支持：gRPC支持多种编程语言，使得其在跨语言服务调用中具有优势。

**特点**:
- 双向流、负载均衡、超时和重试等高级功能。
- 适用于低延迟、高性能的分布式系统。

#### 4. AsyncAPI

**现状**: 作为描述异步API的标准，AsyncAPI正逐渐获得关注和使用。

**演变**:
- 事件驱动架构：随着事件驱动架构的流行，AsyncAPI提供了一种标准化的方式来定义和管理异步API。
- 工具支持：越来越多的工具和框架支持AsyncAPI，使得其集成和使用变得更加便捷。

**特点**:
- 适用于消息驱动、事件驱动的系统。
- 提供标准化的异步API描述格式。

#### 5. OData (Open Data Protocol)

**现状**: OData是一种由Microsoft开发的用于构建和消费可查询和可交互数据的协议。

**演变**:
- 标准化：OData已被广泛采用，并作为ISO/IEC批准的国际标准。
- 数据操作：提供丰富的数据操作功能，如过滤、排序、分页等，使其在数据密集型应用中具有优势。

**特点**:
- 强大的查询能力，适用于数据驱动的应用。
- 与REST结合使用，提供更加灵活的数据操作。

### 结论

2023年，API协议呈现出多样化和专业化的趋势。REST依然是主流，但GraphQL、gRPC、AsyncAPI和OData等协议在各自的应用场景中表现出色。随着技术的发展和需求的变化，API协议将继续演变，以提供更高的性能、更好的开发体验和更强的灵活性。选择合适的API协议，取决于具体的应用需求、性能要求和开发团队的技术栈。

# Explaining 8 Popular Network Protocols in 1 Diagram
![image](https://github.com/user-attachments/assets/553b1a99-8dd3-4e90-8fd4-7c989c4704f6)

## 网络协议简介

网络协议是计算机之间通信的规则和标准。它们定义了数据如何格式化、传输和接收。网络协议对于构建可靠和高效的网络通信系统至关重要。

以下是一些常见的网络协议：

* **TCP（传输控制协议）**：是一种面向连接的协议，用于确保数据的可靠传输。TCP将数据分解为较小的数据包，并在发送方和接收方之间建立连接以确保所有数据包都按顺序到达。TCP通常用于需要可靠数据传输的应用程序，例如网页浏览、电子邮件和文件传输。

* **UDP（用户数据报协议）**：是一种无连接协议，用于快速传输数据。UDP不建立连接，因此它比TCP更快，但也不那么可靠。UDP通常用于对速度要求较高而对可靠性要求不高的应用程序，例如视频会议和流媒体。

* **HTTP（超文本传输协议）**：是用于在Web浏览器和服务器之间传输数据的协议。HTTP是一种请求-响应协议，这意味着客户端（通常是Web浏览器）向服务器发送请求，服务器然后响应请求并返回所需的数据。HTTP是构建Web应用程序的基础。

* **HTTPS（超文本传输安全协议）**：是HTTP的安全版本。HTTPS使用加密来保护客户端和服务器之间的通信，使其免受窃听和篡改。HTTPS通常用于需要安全连接的应用程序，例如在线银行和电子商务。

* **SMTP（简单邮件传输协议）**：用于发送和接收电子邮件的协议。SMTP将电子邮件从一个邮件服务器传输到另一个邮件服务器。当您发送电子邮件时，您的电子邮件客户端会将电子邮件连接到您的邮件服务器，该服务器会将电子邮件路由到收件人的邮件服务器，然后将其传递给收件人的电子邮件客户端。

* **FTP（文件传输协议）**：用于在计算机之间传输文件的协议。FTP使用两个连接：一个用于控制命令，另一个用于传输实际的文件数据。FTP通常用于从Web服务器下载文件或将文件上传到Web服务器。

* **WebSocket**：是一种提供全双工通信的协议。这意味着数据可以同时在两个方向上传输，这使其非常适合需要实时通信的应用程序，例如聊天和在线游戏。

* **QUIC（HTTP/3）**：是一种新的传输协议，旨在提高HTTP在UDP上的性能。QUIC仍在开发中，但它有可能比TCP更快、更可靠，尤其是对于经历高延迟或数据包丢失的连接。


请注意，这只是一些最常见的网络协议。还有许多其他协议用于各种目的。

# 数据管道概述 Data Pipelines Overview
![image](https://github.com/user-attachments/assets/ab065a35-a5f6-4f45-9b8c-ca2d6954b79a)

数据管道是数据处理和集成系统的重要组成部分，用于将数据从多个来源提取、转换并加载到目标系统中，以便进行存储、分析或进一步处理。以下是对数据管道的概述：

#### 1. 数据管道的基本组件

**1. 数据源（Source）**:
- 数据的起始点，可以是数据库、文件系统、API、流数据（如Kafka）或其他系统。

**2. 数据提取（Extraction）**:
- 从数据源中提取数据。提取的方式可以是批处理（Batch Processing）或流处理（Stream Processing）。

**3. 数据转换（Transformation）**:
- 对提取的数据进行清洗、过滤、聚合、格式转换等处理，使其符合目标系统的要求。

**4. 数据加载（Load）**:
- 将转换后的数据加载到目标系统，如数据仓库、数据湖、数据库或文件系统。

**5. 数据目标（Destination）**:
- 数据的终点，可以是分析工具、机器学习模型、BI（商业智能）工具或其他应用程序。

#### 2. 数据管道的类型

**1. 批处理管道（Batch Pipeline）**:
- 定期处理大批量数据，常用于夜间批处理任务。适用于处理数据量大且实时性要求不高的场景。

**2. 流处理管道（Stream Pipeline）**:
- 实时处理不断流入的数据，适用于需要实时分析和响应的场景，如金融交易、实时监控等。

**3. 混合管道（Hybrid Pipeline）**:
- 结合批处理和流处理的优点，能够处理大批量历史数据和实时数据流。

#### 3. 数据管道的架构

**1. ETL（Extract, Transform, Load）**:
- 传统的数据管道架构，先提取数据，然后进行转换，最后加载到目标系统中。

**2. ELT（Extract, Load, Transform）**:
- 现代的数据管道架构，先提取并加载数据到目标系统，再在目标系统中进行数据转换。适用于数据仓库和数据湖。

#### 4. 数据管道的工具和技术

**1. 数据提取工具**:
- Sqoop, Apache Flume, Logstash

**2. 数据处理和转换工具**:
- Apache Spark, Apache Beam, Google Dataflow

**3. 数据加载工具**:
- Apache Nifi, Talend, AWS Glue

**4. 数据目标和存储**:
- Amazon S3, Google BigQuery, Apache Hive

#### 5. 数据管道的最佳实践

**1. 自动化和监控**:
- 使用调度工具（如 Apache Airflow）自动化数据管道的工作流程，并实现数据质量监控和异常检测。

**2. 可扩展性和弹性**:
- 设计数据管道时考虑可扩展性和弹性，确保系统能够处理不断增长的数据量和流量。

**3. 数据质量管理**:
- 实施数据清洗、数据验证和数据一致性检查，确保数据的准确性和完整性。

**4. 安全性和合规性**:
- 保护敏感数据，遵守数据隐私和安全法规（如GDPR、HIPAA）。

### 总结

数据管道是现代数据驱动决策和分析的重要基础设施。通过有效地提取、转换和加载数据，企业可以从多种数据源中获取有价值的信息，支持业务分析、预测和优化。选择合适的工具和技术，遵循最佳实践，可以构建高效、可靠和安全的数据管道。

# CAP, BASE, SOLID, KISS, What do these acronyms mean?
![image](https://github.com/user-attachments/assets/e86221b5-4aaa-408f-b41c-22e857d5c10c)

### 1. CAP 定理

**CAP** 定理，也称为布鲁尔定理，由计算机科学家 Eric Brewer 提出，描述了分布式系统中的三个核心属性：

- **C** (Consistency 一致性): 每次读请求都能读取到最近写入的数据。
- **A** (Availability 可用性): 每次请求都能收到响应，无论成功或失败。
- **P** (Partition Tolerance 分区容忍性): 系统即使遇到网络分区（网络故障分隔了节点），也能继续运行。

根据 CAP 定理，一个分布式系统在网络分区时最多只能保证其中两个属性。

### 2. BASE 理论

**BASE** 理论是一种相对于传统 ACID 属性的替代方案，特别适用于分布式系统。BASE 的主要特点是：

- **B** (Basically Available 基本可用): 系统保证在大部分情况下是可用的。
- **A** (Soft state 软状态): 系统的状态可以是软的，允许存在中间状态，不需要强一致性。
- **E** (Eventual consistency 最终一致性): 系统在一定时间内会达到最终一致性，允许短暂的不一致。

BASE 理论关注的是系统的可扩展性和灵活性，特别适用于分布式数据库和NoSQL系统。

### 3. SOLID 原则

**SOLID** 原则是面向对象编程的五个设计原则，由 Robert C. Martin 提出，旨在提高代码的可维护性和可扩展性：

- **S** (Single Responsibility Principle 单一职责原则): 一个类只应有一个引起变化的原因，即一个类只负责一个功能。
- **O** (Open/Closed Principle 开闭原则): 软件实体应当对扩展开放，对修改关闭。
- **L** (Liskov Substitution Principle 里氏替换原则): 子类应当可以替换其基类，而不影响程序的正确性。
- **I** (Interface Segregation Principle 接口隔离原则): 使用多个专门的接口，而不是一个通用的接口。
- **D** (Dependency Inversion Principle 依赖倒置原则): 高层模块不应该依赖低层模块，二者都应该依赖抽象。抽象不应该依赖细节，细节应该依赖抽象。

### 4. KISS 原则

**KISS** 原则，是 "Keep It Simple, Stupid" 的缩写，提倡简单设计。其核心思想是：

- **Keep It Simple, Stupid** (保持简单，笨蛋): 系统和设计应该尽量保持简单，不要过度复杂化。简单的系统更容易理解、维护和修改。

KISS 原则强调避免不必要的复杂性，使代码和设计易于理解和使用。

### 总结

这些原则和理论（CAP, BASE, SOLID, KISS）在不同的上下文中有着不同的应用：
- **CAP 定理和 BASE 理论**: 主要应用于分布式系统和数据库设计。
- **SOLID 原则**: 主要应用于面向对象编程和软件设计。
- **KISS 原则**: 广泛应用于各种系统设计和软件开发，倡导简单性和可维护性。

理解和应用这些原则，有助于构建高效、可靠和可维护的系统。

# GET, POST, PUT... Common HTTP “verbs” in one figure
![image](https://github.com/user-attachments/assets/e1b7708d-58f8-410b-b0b3-1fd262f5ea40)

## HTTP常见请求方法详解

HTTP请求方法（也称为HTTP动词或HTTP Verbs）是客户端用来指示服务器执行的操作的代码。它们是HTTP协议的核心，用于在客户端和服务器之间进行通信。

以下是九种最常见的HTTP请求方法及其用途：

* **GET**：用于从服务器获取资源。它通常用于获取网页、图像或其他数据。GET请求被认为是安全的，因为它不会修改服务器上的现有数据。

* **PUT**：用于更新或创建服务器上的资源。它将指定位置的任何现有资源替换为提供的数据。PUT请求通常用于更新数据库记录或上传文件。

* **POST**：用于向服务器提交数据以创建新资源或更新现有资源。它是从HTML表单提交数据时最常用的方法。POST请求可以用于各种目的，例如注册用户、提交订单或发布评论。

* **DELETE**：用于从服务器删除资源。DELETE请求通常用于删除数据库记录或文件。

* **PATCH**：用于部分修改资源。与替换整个资源的PUT不同，PATCH允许对资源进行特定更改。PATCH请求通常用于更新数据库记录的部分字段或更新软件配置。

* **HEAD**：用于检索资源的头部信息，而不会传输整个主体。这对于检查资源是否已修改或获取其大小很有用。

* **CONNECT**：用于通过代理建立到服务器的隧道连接。这通常用于HTTPS连接。

* **OPTIONS**：用于检索特定资源支持的HTTP方法。

* **TRACE**：将收到的请求回显回客户端，这对于调试目的很有用。


以下是一些HTTP请求方法的示例：

* 要获取`https://www.example.com/index.html`网页，可以使用以下GET请求：

```
GET https://www.example.com/index.html
```

* 要更新数据库中的用户记录，可以使用以下PUT请求：

```
PUT https://www.example.com/users/123
Content-Type: application/json
{"name": "John Doe", "email": "johndoe@example.com"}
```

* 要从HTML表单提交数据，可以使用以下POST请求：

```
POST https://www.example.com/register
Content-Type: application/x-www-form-urlencoded
username=johndoe&password=password123
```

* 要删除文件`https://www.example.com/files/myfile.txt`，可以使用以下DELETE请求：

```
DELETE https://www.example.com/files/myfile.txt
```

* 要检索`https://www.example.com/image.jpg`图像的头部信息，可以使用以下HEAD请求：

```
HEAD https://www.example.com/image.jpg
```


HTTP请求方法是构建Web应用程序和API的重要组成部分。了解每个方法的目的和用法对于开发人员和用户都是必不可少的。

# How Do C++, Java, Python Work?
![image](https://github.com/user-attachments/assets/6a8ebc6f-3ec5-4b9c-abf5-df79cc72ad2b)

## C++, Java 和 Python 的工作原理

C++、Java 和 Python 是三种流行的编程语言，它们在编译和执行过程方面存在一些关键差异。以下是这三种语言工作原理的简要概述：

**C++**

* **源代码:** C++ 代码以纯文本格式编写，并带有 `.cpp` 扩展名。它包含函数、类和其他编程结构，用于定义程序的逻辑。

* **编译器:** C++ 编译器将源代码转换为机器码，这是计算机的 CPU 可以理解和执行的语言。此过程包括检查语法错误、将代码转换为中间表示以及生成最终机器码。

* **机器码:** 生成的机器码由 CPU 直接执行，CPU 会执行代码中指定的指令。这允许程序与硬件交互并执行各种任务。

**Java**

* **源代码:** Java 代码以纯文本格式编写，并带有 `.java` 扩展名。它类似于 C++，但具有面向对象编程和垃圾回收等附加功能。

* **编译器:** Java 编译器（也称为 javac）将源代码转换为字节码，这是一种平台无关的中间表示。这意味着字节码可以在任何 Java 虚拟机 (JVM) 上运行，无论底层操作系统或硬件如何。

* **Java 虚拟机 (JVM):** JVM 是一个执行 Java 字节码的软件程序。它安装在用户系统上并为 Java 程序提供运行环境。JVM 将字节码转换为特定于主机系统的机器码，允许程序与硬件交互。

**Python**

* **源代码:** Python 代码以纯文本格式编写，并带有 `.py` 扩展名。它以其简洁性和可读性而闻名，使用缩进来定义代码块。

* **解释器:** Python 解释器（也称为 CPython）逐行读取源代码并直接执行。这意味着没有编译步骤，代码在运行时被解释。

* **字节码:** Python 也使用字节码，但它针对解释器进行了优化，而不是像 Java 字节码那样平台无关。解释器将源代码转换为字节码，然后直接执行。

**比较:**

| 特性 | C++ | Java | Python |
|---|---|---|---|
| 编译 | 编译为机器码 | 编译为字节码 | 解释 |
| 执行 | 直接由 CPU 执行 | 由 JVM 执行 | 由解释器执行 |
| 性能 | 通常更快 | 可能比 C++ 慢 | 可能比 C++ 和 Java 慢 |
| 平台独立性 | 不支持平台独立性 | 支持平台独立性 | 支持平台独立性 |
| 内存管理 | 手动内存管理 | 自动垃圾回收 | 自动垃圾回收 |
| 应用 | 系统编程、游戏开发、高性能应用 | Web 应用、企业应用、Android 开发 | 数据科学、Web 开发、脚本 |

**总结:**

* **C++** 是一种功能强大且高效的语言，非常适合系统编程、游戏开发和高性能应用。

* **Java** 是一种通用语言，广泛用于 Web 应用、企业应用和 Android 开发。它提供了平台独立性和自动垃圾回收。

* **Python** 是一种流行的数据科学、Web 开发和脚本语言。它以其简洁性、可读性和丰富的库而闻名。

编程语言的选择取决于项目的具体需求和开发人员的偏好。每种语言都有其优缺点，在做出决定时务必考虑这些因素。

# Top 12 Tips for API Security
![image](https://github.com/user-attachments/assets/5a3bd2f6-6588-4a66-b9eb-9cb64413739d)
## API 安全的 12 个最佳实践

API（应用程序编程接口）是一种允许不同软件系统之间通信的工具。它们是构建现代 Web 应用程序和服务的关键要素。但是，API 也可能成为安全漏洞，如果未正确保护，可能会导致数据泄露和其他安全事件。

以下是在设计和部署 API 时要遵循的 12 个最佳实践，以帮助确保其安全：

1. **使用 HTTPS**：HTTPS 是使用 SSL/TLS 加密保护的 HTTP 协议。这将确保在客户端和服务器之间传输的所有数据都是加密的，防止窃听和中间人攻击。

2. **使用 OAuth 2**：OAuth 2 是一种授权协议，允许用户授予第三方应用程序访问其帐户或资源的权限，而无需共享其密码。这有助于减少 API 密钥被盗的风险。

3. **使用 WebAuthn**：WebAuthn 是一种 Web 身份验证标准，允许用户使用他们的设备（例如 YubiKey 或指纹扫描仪）进行身份验证。这比传统的用户名和密码更安全，因为它可以防止网络钓鱼和凭据填充攻击。

4. **实施速率限制**：速率限制可帮助防止滥用 API，例如拒绝服务攻击（DDoS）。通过限制每个用户或客户端在一定时间内可以进行的请求数量，您可以帮助确保 API 不被淹没。

5. **使用 API 密钥**：API 密钥是用于验证 API 请求的字符串。它们应该强壮且保密，并且应该定期轮换。

6. **验证所有输入**：永远不要相信用户提供的数据。验证所有输入以确保它们有效且安全，并防止注入攻击。

7. **使用 API 网关**：API 网关是一种代理服务器，可用于保护 API 免受各种威胁，例如 DDoS 攻击、注入攻击和数据泄露。

8. **使用错误处理**：API 应该以安全的方式处理错误和异常。不要向客户端公开敏感信息，例如堆栈跟踪。

9. **记录和监控**：记录 API 请求和响应可帮助您识别可疑活动并调查安全事件。

10. **进行定期安全测试**：定期对您的 API 进行渗透测试和其他安全评估，以识别和修复漏洞。

11. **保持您的软件更新**：确保您的 API 依赖项（例如 Web 服务器、框架和库）是最新的，以修复已知的安全漏洞。

12. **遵循最佳实践**：遵循 OWASP API 安全 Top 10 等行业最佳实践，以确保您的 API 受到良好保护。

通过遵循这些最佳实践，您可以帮助确保您的 API 安全并免受攻击。

以下是一些有关如何使用 Gemini 实践这些提示的附加说明：

* **使用 HTTPS：**
    * 使用 `设置安全首选项` 命令启用 HTTPS。
    * 指定您的 SSL/TLS 证书。

* **使用 OAuth 2：**
    * 使用 `创建 OAuth 2 客户端` 命令创建 OAuth 2 客户端。
    * 将客户端 ID 和客户端密钥提供给您的应用程序。

* **使用 WebAuthn：**
    * 使用 `启用 WebAuthn` 命令启用 WebAuthn。
    * 配置您的应用程序以使用 WebAuthn 进行身份验证。

* **实施速率限制：**
    * 使用 `设置速率限制` 命令设置速率限制规则。
    * 指定每个用户或客户端的允许请求数。

* **使用 API 密钥：**
    * 使用 `创建 API 密钥` 命令创建 API 密钥。
    * 将 API 密钥提供给您的应用程序。

* **验证所有输入：**
    * 使用 Gemini 的验证功能验证用户提供的数据。
    * 确保所有数据都经过正确格式化和验证。

* **使用 API 网关：**
    * 使用 `创建 API 网关` 命令创建 API 网关。
    * 将您的 API 路由到 API 网关。

* **使用错误处理：**
    * 使用 Gemini 的错误处理功能处理错误和异常。
    * 不要向客户端公开敏感信息。

* **记录和监控：**
    * 使用 `启用日志记录` 命令启用日志记录。
    * 使用 `监控 API` 命令监控您的 API。

* **进行定期安全测试：**
    * 使用 Gemini 的安全扫描功能扫描您的 API 以查找漏洞。
    * 手动测试您的 API 以识别任何潜在的安全风险。

* **保持您的软件更新：**
    * 使用 `更新 Gemini` 命令更新 Gemini 到最新版本。
    * 更新您的 API 依赖项以修复已知的安全漏洞。

* **遵循最佳实践：**
    * 阅读 OWASP API 安全 Top 10 等行业最佳实践

# Our recommended materials to crack your next tech interview
![image](https://github.com/user-attachments/assets/85fdac8e-b77b-48e2-9245-45124e861178)

# How To Release A Mobile App
![image](https://github.com/user-attachments/assets/5b364e14-cb45-4405-a396-d16782184efa)

Sure, here is a Chinese explanation of the image:

## 如何发布移动应用程序

这张图片展示了如何将移动应用程序发布到 iOS 和 Android 平台的过程。它概述了将应用程序从开发到应用商店分发的关键阶段。

**iOS 应用程序发布流程**

1. **注册和开发:**
    * **Apple 开发者帐户:** 注册 Apple 开发者计划以访问开发工具和资源。
    * **Xcode:** 使用 Xcode，适用于 macOS 的集成开发环境 (IDE)，开发您的 iOS 应用程序。

2. **构建和测试:**
    * **编译二进制文件:** 将您的应用程序源代码编译为可执行的机器代码，用于 iOS 设备。
    * **运行单元测试:** 执行单元测试以确保您的应用程序的各个组件功能正常。
    * **创建发布候选人 (RC) 构建:** 生成应用程序的发布候选人构建，这是用于测试的近最终版本。

3. **批准:**
    * **利益相关者:** 与利益相关者一起审查 RC 构建以收集反馈并解决任何问题。
    * **合规性:** 确保您的应用程序符合 Apple 的 App Store 审核指南。
    * **安全:** 实施安全措施来保护用户数据并符合应用商店的要求。

4. **提交:**
    * **元数据:** 准备应用程序元数据，包括描述、屏幕截图和发行说明。
    * **ASO:** 优化您的应用程序的应用商店优化 (ASO) 以提高搜索结果中的可见性。
    * **上传 IPA:** 将最终打包的应用程序 (IPA) 上传到 Apple 的 App Store Connect 进行审查。

5. **应用程序提交:**
    * **App Store 审核:** Apple 会审核您的应用程序是否符合其指南和技术要求。
    * **批准/拒绝:** 如果获得批准，您的应用程序将发布到 App Store。如果被拒绝，请解决反馈并重新提交。

6. **发布:**
    * **设置发布日期:** 安排您的应用程序的发布日期，使其可供用户使用。
    * **监控性能:** 跟踪应用程序下载、使用情况和用户评论后发布。

**Android 应用程序发布流程**

1. **注册和开发:**
    * **Google Play 控制台:** 创建 Google Play 开发者帐户以在 Google Play 商店上发布应用程序。
    * **Android Studio:** 使用 Android Studio，官方的 Android 应用程序开发 IDE，创建您的应用程序。

2. **构建和测试:**
    * **创建发布构建:** 生成应用程序的发布构建，针对 Android 设备进行优化。
    * **运行单元测试:** 进行单元测试以验证应用程序组件的功能。
    * **错误测试:** 在发布之前进行彻底的错误测试以识别并修复任何问题。

3. **质量保证:**
    * **Beta 测试:** 将您的应用程序分发给有限的 Beta 测试人员以获取反馈和错误检测。
    * **回归测试:** 确保新的更改或修复不会引入新错误。

4. **提交:**
    * **元数据:** 准备应用程序元数据，包括描述、屏幕截图和发行说明。
    * **ASO:** 优化您的应用程序的 ASO 以提高其在 Google Play 搜索结果中的可见性。
    * **上传 APK:** 将最终打包的应用程序 (APK) 上传到 Google Play 控制台。

5. **应用程序提交:**
    * **Google Play 审核:** Google 会审核您的应用程序是否符合其政策和技术标准。
    * **批准/拒绝:** 如果获得批准，您的应用程序将发布在 Google Play 商店上。如果被拒绝，请解决反馈并重新提交。

6. **发布:**
    * **设置发布日期:** 安排您的应用程序的发布日期，使其可供用户使用。
    * **监控性能:** 跟踪应用程序下载、使用情况和用户评论后发布。

**关键点:**

* **遵循平台特定指南:** 每个平台都有自己的应用程序提交指南和要求。
* **彻底测试:** 严格的测试对于确保高质量且无错误的应用程序至关重要。
* **ASO 优化:** 优化您的应用程序的元数据和描述以提高其在应用商店中的可见性。
* **监控和迭代:** 不断监控应用程序性能、用户反馈和市场趋势以进行改进。

# A handy cheat sheet for the most popular cloud services
![image](https://github.com/user-attachments/assets/29d83f18-db04-455f-b8ad-dd94cfe1b993)

## 云计算服务比较

您提供的图片比较了不同公司提供的各种云计算服务。它突出显示了每项服务的关键功能和功能，使用户能够根据其云计算需求做出明智的决策。

**云计算服务比较**

| 功能 | AWS | Azure | Google Cloud | 阿里巴巴云 |
|---|---|---|---|---|
| **弹性计算云 (EC2)** | 虚拟机 | 虚拟机实例 | 计算引擎 | 弹性计算 |
| **弹性 Kubernetes 服务 (EKS)** | Azure Kubernetes 服务 (AKS) | Google Kubernetes Engine (GKE) | Oracle Container Engine | 阿里巴巴云 Kubernetes 服务 |
| **Lambda** | Azure Functions | Cloud Functions | OCI Functions | 函数计算 |
| **简单存储服务 (S3)** | Blob 存储 | 云存储 | 40 对象存储 | 对象存储 |
| **弹性块存储** | 托管磁盘 | 永久磁盘 | 永久卷 | 块存储 |
| **弹性文件系统** | 文件存储 | 文件存储 | 文件存储 | 网络附加存储 |
| **虚拟私有云** | 虚拟网络 | 虚拟私有云 | 虚拟网络 | 虚拟私有云 |
| **Route 53** | DNS | DNS | 云 DNS | DNS |
| **弹性负载均衡** | 负载均衡器 | 负载均衡 | 云负载均衡 | 负载均衡器 |
| **Web 应用程序防火墙** | Web 应用程序防火墙 | Web 应用程序防火墙 | Web 应用程序防火墙 | Web 应用程序防火墙 |
| **RDS** | SQL SQL 数据库 | Cloud SQL | ATP | ApsaraDB RDS |
| **DynamoDB** | Cosmos DB | Firebase 实时数据库 | NoSQL 数据库 | 表存储 |
| **Redshift** | Synapse Analytics | BigQuery | 自主数据仓库 | AnalyticDB |
| **Elastic MapReduce** | HDInsight | Dataproc | 大数据 | Elastic MapReduce |
| **Kinesis** | 流分析 | Dataflow | 流 | 数据中心 |
| **SageMaker** | 机器学习 | Vertex AI | 人工智能数据科学平台 | 数据工作 |
| **Glue** | 数据工厂 | 数据融合 | 数据集成 | 数据工作 |
| **EventBridge** | 事件网格 | Eventarc | 400 事件 | 事件桥 |
| **简单队列服务** | 存储队列 | Pub/Sub | 流 | 消息队列 |
| **简单通知服务** | Service Bus | Firebase Cloud Messaging | 通知 | 消息服务 |
| **CloudWatch** | 监控器 | 云监控 | 监控 | 云监控器 |
| **CloudFormation** | 资源管理器 | 部署管理器 | 资源管理器 | 资源管理器 |
| **IAM** | Active Directory | 云身份 | IAM | 编排资源访问管理 |
| **KMS** | 密钥保管库 | Cloud KMS | 保管库 | KMS |

**关键点:**

* **选择适合您需求的服务:** 每个云提供商都提供各种具有不同功能和定价的服务。做出决定时，请考虑您的具体要求。
* **比较价格:** 云计算成本可能因使用情况和提供商而异。比较定价计划和使用情况估计，以找到最具成本效益的解决方案。
* **考虑性能和可靠性:** 确保您选择的云服务能够满足您的性能和可靠性要求。
* **评估安全性:** 评估每个云提供商提供的安全措施以保护您的数据和应用程序。
* **探索免费试用和层级:** 许多云提供商提供免费试用或更低成本的层级，帮助您入门并评估其服务。

通过仔细比较这些因素，您可以选择最适合您的需求和预算的云计算服务。

# Best ways to test system functionality
![image](https://github.com/user-attachments/assets/b868f23e-eb39-4ce5-8be8-cd768863c856)

这张图片介绍了测试系统功能的最佳方法。我会将图片内容翻译成中文：

标题: 测试系统功能的最佳方法

表格包含三列：过程、图示和工具

1. 单元测试
   图示: 显示多个小方块
   工具: pytest, Mocha, JUnit, nunit

2. 集成测试
   图示: 显示组件A、B1、B2及其子组件的层级结构
   工具: Postman, Cucumber, SoapUI, Selenium

3. 系统测试
   图示: 显示系统及其四个模块的关系
   工具: Selenium, Robot Framework, Appium, Apache JMeter

4. 负载测试
   图示: 多个用户访问应用程序，测量性能指标（响应时间、吞吐量、错误率等）
   工具: Apache JMeter, Gatling, Locust, LoadRunner

5. 错误测试
   图示: 服务A和B与各种"攻击"类型的连接（延迟攻击、异常攻击、KillApp攻击）
   工具: Gremlin, Chaos Monkey

6. 测试自动化
   图示: 显示提交更改、触发构建、构建、运行测试、通知测试结果的流程
   工具: Jenkins, Travis CI, CircleCI, GitHub Actions

# Explaining JSON Web Token (JWT) to a 10 year old Kid
![image](https://github.com/user-attachments/assets/889f793a-cfb3-429d-a1fa-8b88b48d21fc)

这张图片解释了JWT（JSON Web Token）的概念和工作原理。我将为您详细解释每个部分：

1. JWT定义
   JWT是JSON Web Token的缩写，是一种以JSON格式存储数据的文件格式。它使用键值对的形式来存储信息。JSON可以包含简单的字符串值，也可以包含数组或嵌套的JSON对象。

2. JWT结构
   JWT由三部分组成：Header（头部）、Payload（数据）和Signature（签名）。这三部分分别用Base64编码，然后用点(.)连接起来形成完整的JWT。

3. JWT工作原理
   - 用户登录，提供用户名和密码。
   - 服务器验证凭据。
   - 服务器创建并签名JWT。
   - 服务器将JWT返回给客户端。
   - 客户端存储JWT（通常在本地存储中）。
   - 客户端在后续请求中携带JWT（通常在Authorization header中）。
   - 服务器验证JWT的签名。
   - 如果验证通过，服务器处理请求。

4. JWT签名算法
   - 公钥/私钥方式：使用私钥签名JWT，公钥验证JWT。常用算法有RS256、ES256等。
   - 对称密钥方式：使用同一个密钥进行签名和验证。常用算法有HMAC、HS256等。

JWT的主要优点是它是无状态的，服务器不需要存储会话信息，这使得它特别适合于分布式系统和微服务架构。然而，使用JWT时需要注意安全性，例如正确处理密钥、设置合适的过期时间等。

# **公司如何将代码发布到生产环境** How do companies ship code to production?
![image](https://github.com/user-attachments/assets/91a1e990-c9c9-48e3-9818-b69b5daf21c0)

**1. 计划**

* **创建用户故事：** 首先，需要创建用户故事来定义将发布到生产环境的代码的功能和特性。用户故事通常采用以下格式：“作为 [角色]，我希望 [执行操作]，以便 [获得收益]。”
* **拆解用户故事：** 开发人员会将这些用户故事分解为更小、更易于管理的任务。然后将这些任务分配给开发人员，并使用项目管理工具（例如 Jira）进行跟踪。

**2. 开发**

* **将代码提交到 Git：** 开发人员编写代码并将其提交到版本控制系统（例如 Git）。这使他们可以跟踪代码更改并与其他开发人员协作。
* **获取反馈：** 开发人员会从产品所有者和其他利益相关者那里获得有关他们所写代码的反馈。此反馈用于提高代码质量。

**3. 构建和打包**

* **构建代码：** 将代码构建成可部署到生产环境的包。这包括编译代码、运行测试和创建文档。
* **存储构建结果：** 将构建好的包存储在存储库中，例如 Artifactory。部署团队可以访问此存储库。

**4. 发布**

* **质量保证测试：** 质量保证团队会测试构建好的包，以确保它们符合公司的质量标准。此测试可能包括回归测试、性能测试和安全测试。
* **部署代码：** 部署团队将构建好的包部署到生产环境。这包括将包部署到生产环境并确保它们正常运行。

**5. 监控**

* **SRE 团队监控：** SRE 团队会监控生产环境以确保代码运行顺利。这可能包括监控性能、发出错误警报并将关键问题升级到相应的团队。

# 容器化应用程序部署流程图 How does Docker Work? Is Docker still relevant?
![image](https://github.com/user-attachments/assets/6bff3de6-ae2c-4fa9-b58f-bc7a4a39e854)

您提供的图片展示了容器化应用程序部署的流程图，该流程可分为以下几个主要阶段：

**1. 开发**

在这个初始阶段，开发人员编写应用程序代码。他们通常使用容器来打包代码及其依赖项，以确保代码在不同环境中始终如一地运行。

**2. 构建镜像**

编写完代码后，将其用于构建容器镜像。这些镜像封装了应用程序代码、运行时环境以及它拥有的任何依赖项。可以将容器注册表（例如 Docker Hub）用于存储和共享这些镜像。

**3. 测试**

构建好的容器镜像会进行严格的测试以确保其按预期工作。这可能包括自动化测试、性能测试和安全测试。

**4. 部署**

成功测试后，容器镜像将部署到容器编排平台（例如 Kubernetes）。该平台可自动部署、扩展和管理容器化应用程序。

**5. 生产运行**

部署好的容器将在生产服务器上启动。容器编排平台管理这些容器的生命周期，确保它们平稳高效地运行。

**6. 监控**

对部署的容器性能进行持续监控。此监控有助于识别和解决生产中可能出现的问题。

**附加说明：**

该图片还强调了使用容器部署应用程序的优势。这些优势包括：

* **可移植性：** 容器化应用程序可以在任何具有兼容容器运行时的系统上运行，无论基础操作系统如何。
* **可扩展性：** 容器化应用程序可以通过添加或删除容器轻松扩展或缩减。
* **隔离性：** 容器将应用程序彼此隔离并与底层主机系统隔离，从而提高安全性和可靠性。

# **高可用性Web应用程序系统设计蓝图** System Design Blueprint: The Ultimate Guide
<img width="640" alt="image" src="https://github.com/user-attachments/assets/202b6617-c66f-4fbe-90da-6bd5fb81b0f5">

该蓝图概述了一个健壮的系统设计，用于构建高可用性Web应用程序，优先考虑故障容错和可扩展性，即使在潜在故障面前，也能确保用户始终可以访问和利用应用程序的功能。该设计包含了多个关键组件，协同工作以实现这一目标。

**实现高可用性的基本组成部分**

* **负载均衡器：** 在Web服务器池之间分配传入流量，防止任何单个服务器在流量高峰期过载。这确保了应用程序用户获得最佳性能和响应速度。流行的开源负载均衡器选项包括HAProxy和Nginx，而AWS提供其Application Load Balancer服务。

* **Web服务器：** 充当托管Web应用程序代码并向用户设备提供Web内容的基础。该蓝图在冗余配置中包含多个Web服务器，使用诸如Round Robin DNS或运行状况检查之类的技术来确保故障容错。如果Web服务器遇到问题，负载均衡器可以自动将流量重新路由到健康服务器，最大限度地减少应用程序的停机时间。常见的Web服务器选择包括Apache HTTP Server和Nginx，两者都以稳定性和性能而闻名。

* **API网关：** 充当中央入口点，通过充当所有来自客户端应用程序的API请求的单一访问点来简化通信。API网关根据预定义的规则将这些请求路由到适当的后端服务，从而增强了系统内的可管理性和可观察性。流行的API网关包括Google Cloud Platform的Apigee和Amazon API Gateway。

* **应用程序服务器：** 处理应用程序的核心业务逻辑并与数据库层交互。该设计在冗余配置中包含多个应用程序服务器，类似于Web服务器层。这确保即使应用程序服务器出现故障，健康服务器也可以接管其任务，确保不间断的服务交付。流行的应用程序服务器包括WildFly和Tomcat，两者都提供成熟的Java应用程序服务器功能。

* **高可用数据库集群：** 以容错方式持久存储应用程序的数据。数据库集群将数据复制到多个数据库服务器上，通常在地理上分散以增强弹性。这确保了在单个数据库服务器发生故障时数据可用性和完整性。数据库集群的常见选项包括MySQL Cluster，PostgreSQL集群和Amazon Aurora。

* **缓存：** 通过存储经常访问的数据来减少数据库负载的临时存储层。通过缓存经常请求的数据，该系统降低了数据库查询延迟并增强了用户体验的应用程序响应速度。流行的开源内存缓存是Redis，而AWS提供ElastiCache用于托管缓存部署。

* **内容交付网络（CDN）：** 在策略上位于边缘服务器上，在全球范围内分布静态内容。静态内容（例如图像，JavaScript文件和其他媒体文件）将从最接近用户的服务器上传送，从而显着改善网站加载时间和用户体验。AWS，Azure和Google Cloud Platform等云提供商都提供CDN服务。

* **DNS服务器：** 将域名转换为IP地址，使用户可以通过用户友好的URL访问Web应用程序。通常使用诸如Google Public DNS或OpenDNS之类的公共DNS解析器，而云提供商也提供自己的托管DNS服务。

* **监控系统：** 持续监控所有系统组件的健康状况和性能。监控系统在主动识别和提醒IT工作人员任何潜在问题或性能瓶颈方面起着关键作用。这使IT团队能够在问题影响用户体验之前解决问题并确保最佳的系统正常运行时间。流行的开源监控工具包括Prometheus和Grafana，而云提供商提供自己的托管监控服务。

**提高鲁棒性的其他注意事项**

* **故障容错机制：** 系统设计通过在整个架构中引入冗余组件来优先考虑故障容错。这确保即使单个组件发生故障，应用程序也可以通过利用替代组件来优雅地降低性能或继续运行。水平扩展等技术（可以在其中添加额外的服务器来处理增加的负载）可以进一步提高故障容错性。

* **异步通信：** 该设计应利用异步通信机制（例如消息队列）来促进系统组件之间的通信。这种方法使组件解耦，提高了可扩展性，并通过使各个组件能够按照自己的速度处理消息而无需等待彼此，从而增强了整体系统鲁棒性。流行的消息队列系统包括RabbitMQ和Apache Kafka。

* **安全措施：** 安全性是任何Web应用程序的关键方面，并且该设计应包含健壮的安全措施来防止未经授权的访问，数据泄露和其他恶意攻击。这些措施可能包括防火墙，入侵检测/防御系统（IDS / IPS）以及静态和传输中的数据加密。

* **灾难恢复计划：** 在发生重大中断或灾难时，确保可以快速恢复应用程序至关重要。该计划应概述数据恢复，

# 高可用性Web应用程序系统设计蓝图Key Concepts to Understand Database Sharding
![image](https://github.com/user-attachments/assets/6427df44-78ae-413a-950b-36cc1bd2ab7c)

该蓝图描述了一种健壮的系统设计，用于构建高可用性Web应用程序，该设计优先考虑故障容错和可扩展性，即使在潜在故障面前，也能确保用户始终可以访问和利用应用程序的功能。该设计包含了多个关键组件，协同工作以实现这一目标。

**关键组件**

* **负载均衡器:** 分配传入流量，防止任何单个服务器过载。流行的选择包括HAProxy、Nginx和AWS Application Load Balancer。

* **Web服务器:** 托管Web应用程序代码并提供Web内容。常见的Web服务器包括Apache HTTP Server和Nginx。

* **API网关:** 充当中央入口点，简化通信。流行的API网关包括Apigee和Amazon API Gateway。

* **应用程序服务器:** 处理应用程序逻辑并与数据库交互。流行的应用程序服务器包括WildFly和Tomcat。

* **高可用数据库集群:** 以容错方式存储数据。常见的数据库集群包括MySQL Cluster、PostgreSQL集群和Amazon Aurora。

* **缓存:** 减少数据库负载的临时存储层。流行的缓存包括Redis和ElastiCache。

* **内容交付网络（CDN）:** 全球范围内分布静态内容。流行的CDN包括AWS CloudFront、Azure CDN和Google Cloud CDN。

* **DNS服务器:** 将域名转换为IP地址。流行的DNS服务器包括Google Public DNS、OpenDNS和AWS Route 53。

* **监控系统:** 监视系统健康状况和性能。流行的监控系统包括Prometheus、Grafana和CloudWatch。

**附加考虑因素**

* **故障容错机制：** 通过冗余组件和水平扩展提高故障容错能力。

* **异步通信：** 使用消息队列等技术实现异步通信以提高可扩展性。

* **安全措施：** 实施防火墙、IDS/IPS、加密等安全措施。

* **灾难恢复计划：** 制定灾难恢复计划以确保快速恢复。

**专业术语**

* **负载均衡:** 将传入流量分配给多个服务器以提高性能和可用性。

* **故障容错:** 系统能够容忍组件故障而继续运行的能力。

* **可扩展性:** 系统能够处理增加的负载或用户数量的能力。

* **API网关:** 提供对后端服务的单一访问点并管理API流量。

* **数据库集群:** 多个数据库服务器协同工作以提供高可用性和可扩展性。

* **缓存:** 临时存储数据以减少数据库负载并提高性能。

* **内容交付网络:** 全球范围内分布静态内容以提高网站加载速度。

* **DNS服务器:** 将域名转换为IP地址以使用户可以访问网站。

* **监控系统:** 收集和分析系统数据以识别问题并确保系统正常运行。

**总结**

该蓝图提供了一个全面的框架，用于设计和构建高可用性、可扩展性和安全的Web应用程序。通过仔细考虑每个组件的功能和相互关系，可以创建能够满足苛刻需求的健壮系统。

# A nice cheat sheet of different monitoring infrastructure in cloud services
![image](https://github.com/user-attachments/assets/2983b5d0-4063-47fd-8df9-65eed7491a0e)

# 主要架构风格和设计模式 Top 5 Software Architectural Patterns
![image](https://github.com/user-attachments/assets/34f54d56-ee63-44e2-b2bb-11010a6c1b57)

您发送的图像是一个图表，描绘了各种软件架构风格和设计模式。它采用圆形格式，分为多个分区，代表不同的风格和模式。每个分区都被分配了唯一的颜色，以提高视觉吸引力和区分度。

该图表将这些风格分为两大类：架构模式和设计模式。架构模式涉及广泛的系统级结构，而设计模式则专注于特定的软件设计解决方案。

以下是图表中一些主要架构风格和设计模式的细分：

**架构模式：**

* **微服务架构：** 这种模式将软件应用程序构建为一组独立可部署的细粒度服务。每个服务都拥有特定的业务功能，并通过定义良好的接口进行通信。这种方法促进了松耦合、可扩展性和弹性。

* **事件驱动架构 (EDA)：** 这种架构风格强调事件的产生、检测、消费和相应的反应。它促进了组件之间的松耦合，并促进了异步通信。EDA 非常适合实时或响应式系统。

* **分层（n 层）架构：** 这种成熟的方法将软件分为不同的层，例如表示层、业务逻辑层和数据访问层。每个层都提供特定的功能，并通过定义的接口与相邻层交互。这促进了模块化、可维护性和可重用性。

**设计模式：**

* **模型-视图-控制器 (MVC) 架构：** MVC 模式的衍生版本，这种风格倡导分离与数据管理、用户界面和应用程序控制流相关的关注点。通过将这些关注点分离成不同的组件，它促进了代码的可维护性和可重用性。

* **命令查询责任分离 (CQRS) 架构：** 这种方法分离了数据存储的读写操作。读操作由“读模型”处理，而写操作由“写模型”管理。这使得读写工作负载能够独立扩展和优化，从而提高性能和效率。

* **领域驱动设计 (DDD)：** 这种方法专注于建模软件应用程序的核心领域。它强调理解域的概念和过程，以创建与业务域一致的软件设计。

该图表还包含许多其他软件架构风格和设计模式，包括：

* 表示层
* 数据库层
* 微内核架构
* 编排架构
* MVP 架构
* 无数据成本
* 解释器
* 软件架构风格
* API 网关
* 集成层
* 业务逻辑层
* UI 框架
* 数据库
* 适配器
* 端口
* 客户
* 服务器
* 分发
* 存储库
* 工厂
* 总线
* 工作者
* 消息传递
* API
* 云
* 容器
* 微服务
* 事件源
* Kappa 架构
* CRUD（创建、读取、更新、删除）
* REST（表示性状态转移）
* SOAP（简单对象访问协议）
* SOA（面向服务的架构）
* 客户端服务器
* 点对点

每种风格或模式都具有独特的优势和劣势，最佳选择取决于特定应用程序的具体要求。软件架构师需要仔细评估这些方法，以确定最合适的解决方案来有效地满足应用程序的需求。


# OAuth 2.0 授权代码流 OAuth 2.0 Flows
![image](https://github.com/user-attachments/assets/4e8ca6ac-5ec2-4650-b896-0d7cc1d3d7ac)


您发送的图像是一个流程图，说明了 OAuth 2.0 授权代码流。它概述了资源所有者（用户）、客户端应用程序和资源服务器（API）在保护对用户数据访问时的交互。授权代码流是最常见的 OAuth 2.0 流。

以下是授权代码流中涉及的步骤细分：

1. **客户端请求用户数据：** 过程始于客户端应用程序向资源服务器请求用户数据。

2. **用户重定向到授权服务器：** 资源服务器将用户重定向到授权服务器进行身份验证并授予访问权限。

3. **授权服务器提示用户：** 授权服务器提示用户允许客户端应用程序访问其位于资源服务器上的数据。

4. **用户授予或拒绝许可：** 用户审查请求并选择授予或拒绝客户端应用程序访问其数据的权限。

5. **颁发授权代码（如果授予）：** 在授予许可后，授权服务器向客户端应用程序颁发临时授权代码并将用户重定向回客户端应用程序。

6. **客户端交换代码以获取访问令牌：** 然后，客户端应用程序使用授权代码向授权服务器请求访问令牌。客户端还必须提供其客户端标识和密钥进行授权。

7. **授权服务器验证请求：** 授权服务器验证客户端标识、密钥和授权代码。

8. **授予访问令牌（如果有效）：** 如果有效，授权服务器将授予客户端应用程序访问令牌和可能刷新令牌。

9. **客户端请求用户数据（重试）：** 现在，客户端应用程序可以使用访问令牌向资源服务器重新请求用户数据。

10. **资源服务器验证令牌：** 资源服务器验证客户端应用程序提供的访问令牌。

11. **提供数据（如果令牌有效）：** 如果有效，资源服务器将请求的用户数据提供给客户端应用程序。

授权代码流通过确保客户端应用程序永远不会直接处理用户的凭据来增强安全性。授权代码充当临时授权，而不是直接暴露敏感令牌。


# 2006 年至 2022 年 AWS 服务的演变 How did AWS grow from just a few services in 2006 to over 200 fully-featured services?
![image](https://github.com/user-attachments/assets/d053c8e2-ab97-4ec7-9cee-d500b64018b1)

您发送的图像是一个时间线信息图表，描绘了 2006 年至 2022 年 AWS 服务的演变。它展示了近二十年来 Amazon Web Services (AWS) 提供的不断扩大的云计算产品范围。

时间线始于 2006 年，推出了单一服务 Simple Queue Service (SQS)。在随后的几年中，AWS 战略性地推出了跨越各种功能类别的众多其他服务。以下是时间线中的一些重要亮点：

* **2006 年：** 推出 Simple Queue Service (SQS)。
* **2007 年：** 推出 SimpleDB，一个键值数据存储。
* **2008 年：** 推出 Amazon Elastic Compute Cloud (EC2) 和 Elastic Block Store (EBS)，标志着云计算的核心基础设施服务。
* **2009 年：** 推出 Management Console、Elastic Load Balancing、Auto Scaling、CloudFront、Route 53 和 Simple Notification Service (SNS)，扩展了 AWS 产品的广度和功能。
* **2010-2012 年：** 继续扩展服务，重点关注存储、数据库、安全和应用程序管理，包括 Elastic Transcoder、DynamoDB、CloudSearch、IAM、Elastic Beanstalk、VPC、CloudFormation。
* **2013-2014 年：** 推出专注于大数据、成本管理和移动应用程序开发的服务，包括 Redshift、RDS、Kinesis、CloudTrail、WorkSpaces 和移动 SDK。
* **2015-2016 年：** 随着 Lambda、API Gateway、Amazon Kinesis Data Streams、Amazon S3 Glacier、Amazon Rekognition 和 AWS IoT Core 的推出，无服务器计算、机器学习和物联网 (IoT) 服务得到发展。
* **2017-2018 年：** 随着 Amazon SageMaker、Amazon Comprehend、AWS Elemental 系列和 AWS Greengrass 的推出，人工智能、无服务器和管理服务继续多元化。
* **2019-2022 年：** 致力于分析、安全和机器学习，推出了 Amazon Braket、Amazon AppFlow、Amazon Transcribe、Amazon Lookout for Metrics 和 Amazon Lookout for Vision。

到 2022 年，AWS 已发展成为一个综合的云计算平台，提供广泛的服务组合，可满足不同的业务需求。时间线信息图表突出了 AWS 的持续增长和创新，巩固了其作为领先云服务提供商的地位。

# What is GraphQL? Is it a replacement for the REST API?
![image](https://github.com/user-attachments/assets/3fd61b84-a519-4163-a7d5-81b341566edb)

您发送的图像是一个图表，描绘了各种软件架构风格和设计模式。它采用圆形格式，分为多个分区，代表不同的风格和模式。每个分区都被分配了唯一的颜色，以提高视觉吸引力和区分度。

该图表将这些风格分为两大类：架构模式和设计模式。架构模式涉及广泛的系统级结构，而设计模式则专注于特定的软件设计解决方案。

以下是图表中一些主要架构风格和设计模式的细分：

**架构模式：**

* **微服务架构：** 这种模式将软件应用程序构建为一组独立可部署的细粒度服务。每个服务都拥有特定的业务功能，并通过定义良好的接口进行通信。这种方法促进了松耦合、可扩展性和弹性。

* **事件驱动架构 (EDA)：** 这种架构风格强调事件的产生、检测、消费和相应的反应。它促进了组件之间的松耦合，并促进了异步通信。EDA 非常适合实时或响应式系统。

* **分层（n 层）架构：** 这种成熟的方法将软件分为不同的层，例如表示层、业务逻辑层和数据访问层。每个层都提供特定的功能，并通过定义的接口与相邻层交互。这促进了模块化、可维护性和可重用性。

**设计模式：**

* **模型-视图-控制器 (MVC) 架构：** MVC 模式的衍生版本，这种风格倡导分离与数据管理、用户界面和应用程序控制流相关的关注点。通过将这些关注点分离成不同的组件，它促进了代码的可维护性和可重用性。

* **命令查询责任分离 (CQRS) 架构：** 这种方法分离了数据存储的读写操作。读操作由“读模型”处理，而写操作由“写模型”管理。这使得读写工作负载能够独立扩展和优化，从而提高性能和效率。

* **领域驱动设计 (DDD)：** 这种方法专注于建模软件应用程序的核心领域。它强调理解域的概念和过程，以创建与业务域一致的软件设计。

该图表还包含许多其他软件架构风格和设计模式，包括：

* 表示层
* 数据库层
* 微内核架构
* 编排架构
* MVP 架构
* 无数据成本
* 解释器
* 软件架构风格
* API 网关
* 集成层
* 业务逻辑层
* UI 框架
* 数据库
* 适配器
* 端口
* 客户
* 服务器
* 分发
* 存储库
* 工厂
* 总线
* 工作者
* 消息传递
* API
* 云
* 容器
* 微服务
* 事件源
* Kappa 架构
* CRUD（创建、读取、更新、删除）
* REST（表示性状态转移）
* SOAP（简单对象访问协议）
* SOA（面向服务的架构）
* 客户端服务器
* 点对点

每种风格或模式都具有独特的优势和劣势，最佳选择取决于特定应用程序的具体要求。软件架构师需要仔细评估这些方法，以确定最合适的解决方案来有效地满足应用程序的需求。

# HTTPS 的工作原理 HTTPS, SSL Handshake, and Data Encryption Explained to Kids
![image](https://github.com/user-attachments/assets/ecd5bc1e-ef75-4d68-9eaf-617ba8dd5315)

您发送的图像是一张海报，解释了 HTTPS 的工作原理。它使用客户（网络浏览器）和服务器（网站）之间安全对话的隐喻来说明使用 HTTPS 加密数据的过程。

以下是通过 HTTPS 保护通信的关键步骤细分：

1. **客户端发起连接：** 过程始于客户端（Web 浏览器）使用 HTTPS 向服务器（网站）发起连接。

2. **服务器发送证书：** 收到连接请求后，服务器会将其 SSL 证书发送给客户端。该证书包含服务器的公钥，并由受信任的证书颁发机构 (CA) 进行数字签名。

3. **客户端验证证书：** 客户端的 Web 浏览器会验证服务器 SSL 证书的有效性。它会检查证书是否由受信任的 CA 签名以及证书是否仍在有效期内。

4. **安全密钥交换：** 如果证书有效，客户端和服务器将进行安全密钥交换。他们使用加密协议 (例如 TLS（传输层安全）) 建立临时会话密钥。此会话密钥用于加密通信会话期间传输的数据。

5. **加密通信：** 建立会话密钥后，客户端和服务器之间的所有通信都将使用商定的会话密钥进行加密。这种加密会对数据进行混淆，使其对于任何截取它的人来说都无法读取。

6. **目的地解密：** 加密数据仅由收件人（服务器或客户端）使用其各自的私钥解密。

使用 HTTPS 可确保客户端和服务器之间传输的数据的机密性和完整性。使用 HTTPS，窃听者无法拦截和读取数据，并且可以减轻中间人攻击。

总之，HTTPS 是一种关键的安全协议，可保护互联网上的通信。通过加密数据传输，HTTPS 可以保护敏感信息，例如登录凭据、财务数据和个人详细信息，以免遭到未经授权的访问。

# A nice cheat sheet of different databases in cloud services
![image](https://github.com/user-attachments/assets/5b9d21d5-53cc-4e86-94d0-a2dcc1e931fb)

您发送的图像是一张云数据库速查表，总结了不同云提供商和开源/第三方数据库提供的各种云数据库服务。它提供了一个快速参考指南，可帮助用户选择最适合他们需求的数据库解决方案。

速查表采用表格格式组织，包含以下列：

* **数据库类型：** 此列标识数据库类型，例如关系型、文档型或键值型。
* **AWS：** 此列列出了亚马逊网络服务 (AWS) 提供的相应云数据库服务。
* **Azure：** 此列列出了 Microsoft Azure 提供的相应云数据库服务。
* **Google Cloud：** 此列列出了 Google Cloud Platform (GCP) 提供的相应云数据库服务。
* **开源/第三方：** 此列列出了每种类型流行的开源或第三方数据库选项。

以下是速查表中提到的云数据库服务及其相应开源/第三方替代方案的一些示例：

* **关系型数据库：** 对于关系型数据库，AWS 提供关系数据库服务 (RDS)，而 Azure 和 GCP 分别提供类似的 Azure SQL 数据库和 Cloud SQL 服务。MySQL、PostgreSQL 和 Oracle 列为开源关系型数据库的替代方案。

* **列式数据库：** 列式数据库针对数据仓库和分析工作负载进行了优化，AWS 提供 Redshift，而 Azure 和 GCP 分别提供 Synapse Analytics 和 BigQuery。ClickHouse 和 Apache Cassandra 列为开源列式数据库的替代方案。

* **键值数据库：** 键值数据库适用于基于唯一键存储和检索数据，AWS 提供 DynamoDB，而 Azure 和 GCP 分别提供 Cosmos DB 和 Bigtable。Redis 和 ScyllaDB 列为开源键值数据库的替代方案。

* **文档数据库：** 文档数据库非常适合存储和管理半结构化数据，AWS 中的 DocumentDB、Azure 中的 Cosmos DB 和 GCP 中的 Firestore 代表了这类数据库。MongoDB 和 Couchbase 列为开源文档数据库的替代方案。

* **其他数据库类型：** 速查表还包括其他数据库类别，例如时间序列数据库（例如 AWS 中的 Timestream）、图数据库（例如 AWS 中的 Neptune）和地理空间数据库（例如 AWS 中的 Keyspaces）。每个类别也提到了开源替代方案。

总体而言，这张云数据库速查表可作为开发人员和数据库管理员的宝贵资源，因为它提供了对各种云数据库服务产品进行简洁比较。在根据特定需求和功能选择最合适的数据库解决方案时，它可以促进明智的决策。

# 软件开发生命周期 (SDLC) 瀑布模型 CI/CD Pipeline Explained in Simple Terms
![image](https://github.com/user-attachments/assets/46f1c57d-1506-42af-8d7b-6e6920726d28)

您发送的图像是一张图表，描述了软件开发生命周期 (SDLC) 瀑布模型。 SDLC 瀑布模型是一种顺序的、线性的软件开发方法，其中每个阶段都按特定顺序完成，然后再进行下一个阶段。 瀑布模型中的阶段像瀑布一样向下流动，在完成之后几乎没有机会重新访问或修订早期阶段。

以下是 SDLC 瀑布模型中的顺序阶段细分：

**1. 需求收集：** 在初始阶段，项目需求被仔细记录。 这涉及从利益相关者（例如用户、客户和业务分析师）处收集输入，以定义软件项目的特征、功能和目标。

**2. 系统设计：** 在需求收集之后，系统设计开始。 在这里，软件架构师设计了总体系统架构，包括系统规格、硬件和软件需求以及不同软件组件之间的交互方式。

**3. 开发：** 在开发阶段，程序员将系统设计规范转换为功能代码。 此阶段涉及编码、单元测试单个软件组件以及集成测试以确保不同组件协同工作。

**4. 测试：** 在开发之后，进行彻底的测试以识别和纠正软件中的任何错误或缺陷。 测试人员会仔细检查软件以确保它符合指定的要求并按预期执行。

**5. 部署：** 一旦完成足够的测试并且软件被认为功能稳定，它就会部署到生产环境中。 这可能涉及将软件发布给最终用户或将其集成到目标环境中。

**6. 维护：** 部署后，软件进入维护阶段。 这个持续的过程涉及解决错误修复、根据用户反馈或不断变化的需求实施新功能以及为用户提供技术支持。

SDLC 瀑布模型提供了一种结构化且可预测的软件开发方法。 但是，它可能缺乏灵活性，无法适应开发过程后期引入的更改。 这种刚性在敏捷软件开发环境中可能带来挑战，因为敏捷软件开发环境更喜欢持续适应和迭代开发周期。

# What does API gateway do?
![image](https://github.com/user-attachments/assets/bc6c5468-40e2-4e50-b2eb-3bd0904f70ca)

您发送的图像是一张网络示意图，展示了具有灾难恢复功能的云文件存储系统。 它展示了主存储站点和灾难恢复 (DR) 站点，它们都位于云环境中。

以下是此云灾难恢复文件存储解决方案的关键组件和功能的细分：

**1. 主存储站点：** 主存储站点表示生产文件服务器所在的 location。 这是大多数文件访问和存储操作发生的地方。 数据会同步或异步复制到 DR 站点，以在主站点和 DR 站点之间保持数据一致性。

**2. 云存储：** 主站点和 DR 站点都利用云存储，该存储为文件数据提供可扩展性、可靠性和耐久性。 云存储消除了对本地物理存储基础架构的需求，简化了灾难恢复流程。

**3. 复制：** 数据复制是此灾难恢复解决方案的核心方面。 数据会不断从主存储站点复制到 DR 站点，确保始终可用最新副本的数据。 复制可以是同步或异步的，同步复制提供更强的数据一致性保证，但可能影响性能，而异步复制优先考虑性能，但可能会在主站点和 DR 站点之间引入一些数据延迟。

**4. 灾难恢复 (DR) 站点：** DR 站点用作文件存储系统的备份 location。 如果主站点发生灾难或中断，则可以激活 DR 站点以恢复对文件数据的访问并尽量减少停机时间。

**5. 互联网连接：** 主存储站点和 DR 站点都需要互联网连接以促进站点之间的通信和数据复制。

**6. 网络连接：** 为了提高可靠性，主站点和 DR 站点之间的网络连接可能利用地理上不同的路径来降低单点故障的风险。

**7. 故障转移：** 如果主站点发生灾难，将启动故障转移程序以激活 DR 站点。 这可能涉及将用户访问切换到 DR 站点并确保文件存储操作继续进行。

**8. 回滚（可选）：** 一旦主站点恢复，可能会执行回滚过程，具体取决于特定的灾难恢复计划。 此回滚将涉及将数据从 DR 站点迁移回主站点。

通过实施具有数据复制的云灾难恢复解决方案，组织可以确保业务连续性并在主存储站点中断的情况下最大限度地减少数据丢失。 云存储为灾难恢复解决方案提供可扩展性和灵活性，使其成为许多组织的合适选择。

# The Code Review Pyramid
![image](https://github.com/user-attachments/assets/47759d8f-9ad2-4177-a94e-544bf7a9aab2)

您发送的图像是一张概念图，用于说明敏捷软件开发的概念。敏捷方法是迭代和增量的软件开发方法，强调灵活性、适应性和持续改进。

概念图直观地组织了敏捷开发的关键原则、实践和优势。以下是概念图中突出显示的关键元素细分：

**1. 原则：** 敏捷原则是在敏捷方法论的基础上的基本准则。 一些核心原则包括：

* **通过早期和持续交付实现客户满意度：** 敏捷方法论优先考虑早期和经常地向用户交付可工作的软件。 这可以实现持续反馈并确保软件符合用户需求。
* **拥抱变化：** 敏捷开发承认需求可能会在整个开发过程中不断发展。 敏捷团队具有适应性，并欢迎更改以改进软件。
* **专注于可工作的软件：** 敏捷方法论强调生成可演示和测试的功能软件增量，而不是冗长的文档。
* **协作：** 敏捷促进开发团队、利益相关者和最终用户之间的密切协作。 这促进了透明度并确保每个人都与项目目标保持一致。
* **响应变化而不是遵循计划：** 虽然敏捷强调规划，但它也承认可能会出现不可预见的变化。 敏捷团队优先考虑响应变化以交付最大的价值。

**2. 实践：** 敏捷方法论包含各种指导软件开发过程的实践。 一些常见的敏捷实践包括：

* **用户故事：** 用户故事是从用户角度简要描述的功能。 它们帮助开发团队了解用户需求并优先考虑功能。
* **冲刺：** 冲刺是短暂的时间限定开发周期，团队在其中处理一组重点用户故事。 这种迭代方法促进了更快的反馈和交付。
* **Scrum 会议：** Scrum 会议是整个冲刺期间定期举行的会议，用于讨论进度、识别障碍并计划下一步。 典型的 Scrum 会议有三种：冲刺规划、每日站立会议和冲刺评审会议。
* **看板：** 看板是开发工作流程的可视化表示，通常使用卡片来表示用户故事或任务。 看板展示了工作流程阶段（例如待办事项、正在进行中、已完成）并促进了进度可视化。

**3. 优点：** 实施敏捷方法论可以为软件开发项目带来许多优势。 一些好处包括：

* **提高灵活​​性：** 敏捷开发允许团队根据需要适应不断变化的需求并进行纠正。
* **提高客户满意度：** 通过早期和经常地交付可工作的软件，敏捷方法论可以实现持续反馈并确保软件符合客户需求。
* **增强团队生产力：** 敏捷实践促进协作和沟通，从而导致更有效的开发过程。
* **降低风险：** 敏捷开发的迭代方法有助于早期识别和缓解风险。
* **加快上市时间：** 敏捷方法论可以更快地交付可工作的软件功能，这可能会缩短上市时间。

总而言之，概念图有效地总结了敏捷软件开发的核心原则。 通过拥抱敏捷原则和实践并利用其优势，组织可以培养一种更迭代、更适应和以用户为中心的软件开发方法。

# 构建软件应用程序的微服务架构 A picture is worth a thousand words: 9 best practices for developing microservices
![image](https://github.com/user-attachments/assets/f34ec05d-e28f-4191-a384-946c8a8f8db8)

您发送的图像是一张图表，展示了用于构建软件应用程序的微服务架构。 微服务架构将软件应用程序构建为松散耦合的独立服务集合。 每个服务都是自包含的，这意味着它具有自己的功能和数据库。 微服务通过定义良好的 API（应用程序编程接口）相互通信。

以下是使用微服务架构进行软件开发的关键特征和优势：

**1. 服务分解：** 微服务架构的核心原则是将大型软件应用程序分解为更小、独立的服务。 每个服务都拥有特定的业务功能，并独立于其他服务运行。 这种模块化设计促进了松散耦合，并简化了开发、测试和部署流程。

**2. 独立开发和部署：** 微服务架构支持独立开发、部署和扩展单个服务。 这意味着可以独立开发、测试和部署服务，而不会影响其他服务。 这促进了开发敏捷性和更快的发布周期。

**3. 可扩展性和容错性：** 微服务架构通过允许根据资源需求独立扩展单个服务来促进可扩展性。 此外，如果一个微服务失败，它不一定会导致整个应用程序失败，从而提高了容错性。

**4. 技术异构性：** 微服务架构允许使用不同的编程语言和技术来开发不同服务。 这种灵活性可以解决每个服务的特定需求并利用不同技术的优势。

**5. API 驱动的通信：** 服务使用定义良好的 API 相互通信。 API 封装了服务的功效，并提供与其他服务交互的标准化接口。 这促进了松散耦合，并即使服务使用不同的技术开发也能促进服务之间的通信。

总而言之，微服务架构为软件开发提供了一种模块化、可扩展且灵活的方法。 通过将复杂应用程序分解为更小、独立的服务，微服务架构可以提高敏捷性，促进独立开发和部署，并增强软件应用程序的整体可维护性和弹性。

# What are the greenest programming languages?
![image](https://github.com/user-attachments/assets/4ecfc82b-b259-4be4-ac67-8f7acbd51c97)

您发送的图像是一张表格，总结了不同编程语言的能耗。表格标题为“编程语言的能源效率”，并在底部引用了数据来源的研究。

以下是表格中信息の概要：

**1. 编程语言：** 此列列出了不同的编程语言，包括 C、C++、Java、Python 和 Ruby。

**2. 能量（焦耳）：** 此列显示了每种编程语言在焦耳中的相对能耗。较低的焦耳值表示较低的能耗。为了参考，表中显示 1 焦耳大约是将葡萄抬起一米所需的能量。

该表显示，一些语言的能效明显高于其他语言。例如，C 和 Rust 具有表中最低的能耗值，而 Ruby 和 JavaScript 等语言的值则明显更高。

以下是从表中获得的一些其他见解：

* **编译语言与解释语言：** 通常，编译语言比解释语言更节能。编译语言在执行之前会转换为机器代码，而解释语言会在运行时逐行翻译。解释语言的这种翻译过程可能会消耗更多能量。
* **范式：** 编程范式（例如面向对象、函数式）也可能影响能耗。但是，该表没有提供足够的信息来得出关于范式对能耗影响的明确结论。

总体而言，该表突出了不同编程语言的能耗水平差异。选择节能的编程语言可以促进更可持续的软件开发实践。

**重要说明：** 重要的是要承认，这张表仅代表了一项研究对能耗的发现。能耗受多种因素的影响，需要更多的研究来全面了解不同编程语言的能源效率。

# URL, URI, URN - Do you know the differences?
![image](https://github.com/user-attachments/assets/99f375f8-d35f-4991-a172-2e9f928430ce)



# What branching strategies does your team use?
![image](https://github.com/user-attachments/assets/6ece2459-e763-4d0f-b124-552a171f4a28)

您发送的图像是一张网络示意图，展示了部署在云环境中的 Web 应用防火墙 (WAF)。 WAF 充当安全层，过滤和监控进入 Web 应用程序的 HTTP 流量。 通过过滤恶意流量，WAF 有助于保护 Web 应用程序免受各种基于 Web 的攻击。

以下是云端 WAF 部署中的关键组件和功能概述：

* **基于云的 WAF 服务：** 基于云的 WAF 服务是云提供商提供的安全解决方案。 它会过滤和监控定向到云环境中托管的 Web 应用程序的传入 HTTP 流量。

* **Web 应用程序：** Web 应用程序位于云环境中，是传入 HTTP 流量的目标。

* **HTTP 流量：** HTTP（超文本传输协议）是 Web 服务器和浏览器之间通信的基础。 WAF 特别监控和过滤 HTTP 流量以识别和阻止恶意请求。

* **安全策略规则：** 安全策略规则定义了 WAF 用于允许或阻止传入流量的标准。 这些规则可以配置为根据各种属性过滤流量，例如源 IP 地址、请求方法（例如 GET、POST）以及请求有效负载（HTTP 请求的数据部分）中的模式。

* **允许的流量：** 符合定义的安全策略规则的合法 HTTP 流量被允许到达 Web 应用程序。

* **阻止的流量：** 违反安全策略规则的恶意 HTTP 流量被 WAF 阻止，阻止其到达 Web 应用程序并可能破坏其安全。

* **日志记录和监控：** 基于云的 WAF 服务通常提供日志记录和监控功能。 安全团队可以分析这些日志来识别潜在威胁并了解攻击模式。

云端 WAF 部署为组织提供诸多优势，包括：

* **可扩展性：** 基于云的 WAF 可以轻松扩展以处理波动大的 Web 流量。

* **降低成本：** 组织无需投资于本地 WAF 设备，这可能会降低硬件和维护成本。

* **简化管理：** 云提供商管理 WAF 基础设施，减轻了组织 IT 团队的负担。

* **提高安全性：** 基于云的 WAF 服务经常更新最新的安全规则，这可能会提供更好的保护，以抵御不断发展的威胁。

* **集中管理：** 基于云的 WAF 可以从单个位置集中管理和配置。

总而言之，部署基于云的 WAF 提供了一种可扩展且易于管理的安全解决方案，用于保护 Web 应用程序免受基于 Web 的攻击。 通过过滤和监控传入流量，基于云的 WAF 可以帮助组织降低安全风险并增强其 Web 应用程序的整体安全态势。

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





















































