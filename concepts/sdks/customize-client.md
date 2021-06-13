---
title: Personalizar o cliente de serviço do Microsoft Graph SDK
description: Fornece instruções sobre como alterar o comportamento padrão do cliente de serviço do Microsoft Graph SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: a2750babd35f1e3fd5f361ae43009eaa25eefe87
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911652"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a><span data-ttu-id="f49fd-103">Personalizar o cliente de serviço do Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="f49fd-103">Customize the Microsoft Graph SDK service client</span></span>

<span data-ttu-id="f49fd-104">O cliente Graph SDK da Microsoft configura um conjunto padrão de middleware que permite que o SDK se comunique com os pontos de extremidade Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f49fd-104">The Microsoft Graph SDK client configures a default set of middleware that allows the SDK to communicate with the Microsoft Graph endpoints.</span></span> <span data-ttu-id="f49fd-105">Esse conjunto padrão é personalizável, permitindo que você altere o comportamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="f49fd-105">This default set is customizable, allowing you to change the behavior of the client.</span></span> <span data-ttu-id="f49fd-106">Por exemplo, você pode inserir o registro em log personalizado ou adicionar um manipulador de teste para simular cenários específicos.</span><span class="sxs-lookup"><span data-stu-id="f49fd-106">For example, you can insert customized logging, or add a test handler to simulate specific scenarios.</span></span> <span data-ttu-id="f49fd-107">Você pode adicionar e remover componentes de middleware.</span><span class="sxs-lookup"><span data-stu-id="f49fd-107">You can add and remove middleware components.</span></span> <span data-ttu-id="f49fd-108">É importante observar que a ordem na qual os componentes de middleware são executados é significativa.</span><span class="sxs-lookup"><span data-stu-id="f49fd-108">It is important to note that the order in which middleware components run is significant.</span></span>

## <a name="c"></a>[<span data-ttu-id="f49fd-109">C#</span><span class="sxs-lookup"><span data-stu-id="f49fd-109">C#</span></span>](#tab/csharp)

```csharp
var handlers = GraphClientFactory.CreateDefaultHandlers(authProvider);

// Remove a default handler
var compressionHandler =
    handlers.Where(h => h is CompressionHandler).FirstOrDefault();
handlers.Remove(compressionHandler);

// Add a new one
// ChaosHandler simulates random server failures
handlers.Add(new ChaosHandler());

var httpClient = GraphClientFactory.Create(handlers);

var customGraphClient = new GraphServiceClient(httpClient);

var messages = await customGraphClient.Me.Messages.Request()
    .Top(100)
    .Select(m => m.Subject)
    .GetAsync();
```

## <a name="typescript"></a>[<span data-ttu-id="f49fd-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="f49fd-110">TypeScript</span></span>](#tab/typeScript)

```typescript
// Create a custom auth provider
let authProvider = new SimpleAuthProvider(accessToken);
// Create an authentication handler that uses custom auth provider
let authHandler = new MicrosoftGraph.AuthenticationHandler(authProvider);

// Create a custom logging handler
let loggingHandler = new CustomLoggingHandler();

// Create a standard HTTP message handler
let httpHandler = new MicrosoftGraph.HTTPMessageHandler();

// Use setNext to chain handlers together
// auth -> logging -> http
authHandler.setNext(loggingHandler);
loggingHandler.setNext(httpHandler);

// Pass the first middleware in the chain in the middleWare property
const client = MicrosoftGraph.Client.initWithMiddleware({
  defaultVersion: 'v1.0',
  debugLogging: true,
  middleware: authHandler,
});

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();
```

### <a name="simpleauthproviderts"></a><span data-ttu-id="f49fd-111">SimpleAuthProvider.ts</span><span class="sxs-lookup"><span data-stu-id="f49fd-111">SimpleAuthProvider.ts</span></span>

```typescript
import { AuthenticationProvider } from "@microsoft/microsoft-graph-client";

export default class SimpleAuthProvider implements AuthenticationProvider {
  private accessToken: string;

  constructor(accessToken: string) {
    this.accessToken = accessToken;
  }

  getAccessToken = async (): Promise<string> => {
    return this.accessToken;
  }
}
```

### <a name="customlogginghandlerts"></a><span data-ttu-id="f49fd-112">CustomLoggingHandler.ts</span><span class="sxs-lookup"><span data-stu-id="f49fd-112">CustomLoggingHandler.ts</span></span>

```typescript
import { Context, Middleware } from "@microsoft/microsoft-graph-client";

export default class CustomLoggingHandler implements Middleware {
  private nextMiddleware: any = null;

  execute = async (context: Context): Promise<void> => {
    console.log(`Logging request: ${context.request.toString()}`);
    return await this.nextMiddleware.execute(context);
  }
  setNext = (middleware: Middleware): void => {
    this.nextMiddleware = middleware;
  }
}
```

## <a name="java"></a>[<span data-ttu-id="f49fd-113">Java</span><span class="sxs-lookup"><span data-stu-id="f49fd-113">Java</span></span>](#tab/java)

```java
// you can configure any OkHttpClient option and add interceptors
// Note: com.microsoft.graph:microsoft-graph:3.0 or above is required
// for a complete description of available configuration options https://square.github.io/okhttp/4.x/okhttp/okhttp3/-ok-http-client/-builder/
final OkHttpClient httpClient = HttpClients.createDefault(authenticationProvider)
                                .newBuilder()
                                .followSslRedirects(false) // sample configuration to apply to client
                                .build();

final GraphServiceClient graphServiceClient = GraphServiceClient
                .builder()
                .httpClient(httpClient)
                .buildClient();
```

---

## <a name="configuring-the-http-proxy-for-the-client"></a><span data-ttu-id="f49fd-114">Configurando o proxy HTTP para o cliente</span><span class="sxs-lookup"><span data-stu-id="f49fd-114">Configuring the HTTP proxy for the client</span></span>

<span data-ttu-id="f49fd-115">Alguns ambientes exigem que os aplicativos cliente usem um proxy HTTP antes que eles possam acessar a Internet pública.</span><span class="sxs-lookup"><span data-stu-id="f49fd-115">Some environments require client applications to use a HTTP proxy before they can access the public internet.</span></span> <span data-ttu-id="f49fd-116">Esta seção mostra como configurar o proxy para os SDKs Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f49fd-116">This section shows how to configure the proxy for the Microsoft Graph SDKs.</span></span>

<!-- markdownlint-disable MD024 -->
## <a name="c"></a>[<span data-ttu-id="f49fd-117">C#</span><span class="sxs-lookup"><span data-stu-id="f49fd-117">C#</span></span>](#tab/csharp)

```csharp
// URI to proxy
var proxyAddress = "http://localhost:8888";

// Create a new System.Net.Http.HttpClientHandler with the proxy
var handler = new HttpClientHandler
{
    // Create a new System.Net.WebProxy
    // See WebProxy documentation for scenarios requiring
    // authentication to the proxy
    Proxy = new WebProxy(new Uri(proxyAddress))
};

// Create an options object for the credential being used
// For example, here we're using a ClientSecretCredential so
// we create a ClientSecretCredentialOptions object
var options = new ClientSecretCredentialOptions
{
    // Create a new Azure.Core.HttpClientTransport
    Transport = new HttpClientTransport(handler)
};

var credential = new ClientSecretCredential(
    "YOUR_TENANT_ID",
    "YOUR_CLIENT_ID",
    "YOUR_CLIENT_SECRET",
    options
);

// Create a new Microsoft.Graph.HttpProvider using the
// proxied HttpClientHandler
var httpProvider = new HttpProvider(handler, true);

var scopes = new[] { "https://graph.microsoft.com/.default" };
var graphClient = new GraphServiceClient(credential, scopes, httpProvider);
```

## <a name="typescript"></a>[<span data-ttu-id="f49fd-118">TypeScript</span><span class="sxs-lookup"><span data-stu-id="f49fd-118">TypeScript</span></span>](#tab/typeScript)

```typescript
// Create a credential from @azure/identity package
const credential = new ClientSecretCredential(
  'YOUR_TENANT_ID',
  'YOUR_CLIENT_ID',
  'YOUR_CLIENT_SECRET',
  {
    proxyOptions: {
      host: 'localhost',
      port: 8888,
      // If proxy requires authentication
      //username: '',
      //password: ''
    },
  }
);

// Create a Graph token credential provider
const tokenAuthProvider = new TokenCredentialAuthenticationProvider(
  credential,
  {
    scopes: [ 'https://graph.microsoft.com/.default' ]
  });

const client = MicrosoftGraph.Client.initWithMiddleware({
  authProvider: tokenAuthProvider,
  // Configure proxy in fetchOptions
  fetchOptions: {
    agent: new HttpsProxyAgent('http://localhost:8888')
  }
});
```

## <a name="java"></a>[<span data-ttu-id="f49fd-119">Java</span><span class="sxs-lookup"><span data-stu-id="f49fd-119">Java</span></span>](#tab/java)

```Java
final int proxyPort = 8080;
final InetSocketAddress proxyInetAddress = new InetSocketAddress("proxy.ip.or.hostname", proxyPort);

// The section below configures the proxy for the Azure Identity client
// and is only needed if you rely on Azure Identity for authentication
final ProxyOptions pOptions = new ProxyOptions(ProxyOptions.Type.HTTP, proxyInetAddress);
final HttpClientOptions clientOptions = new HttpClientOptions();
clientOptions.setProxyOptions(pOptions);
final HttpClient azHttpClient = HttpClient.createDefault(clientOptions);

// Or any other credential the application is using
final ClientSecretCredential clientSecretCredential =
    new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        // don't forget that addition to use the configured client
        .httpClient(azHttpClient)
        .build();
final TokenCredentialAuthProvider authenticationProvider =
    new TokenCredentialAuthProvider(Arrays.asList(SCOPES), clientSecretCredential);

// The section below configures the proxy for the Microsoft Graph SDK client
final Proxy proxy = new Proxy(Proxy.Type.HTTP, proxyInetAddress);

// This block is only needed if the proxy requires authentication
final Authenticator proxyAuthenticator = new Authenticator() {
  @Override
  public Request authenticate(Route route, Response response) throws IOException {
    String credential = Credentials.basic("username", "password");
    return response.request().newBuilder()
        .header("Proxy-Authorization", credential)
        .build();
  }
};

final OkHttpClient graphHttpClient =
    HttpClients.createDefault(authenticationProvider)
        .newBuilder()
        .proxy(proxy)
        .proxyAuthenticator(proxyAuthenticator)
        .build();

final GraphServiceClient graphServiceClient =
    GraphServiceClient
        .builder()
        .httpClient(graphHttpClient)
        .buildClient();

```

> [!NOTE]
> <span data-ttu-id="f49fd-120">Para obter mais informações sobre a configuração de proxy de Identidade do Azure, consulte [ProxyOptions](/java/api/com.azure.core.http.proxyoptions.proxyoptions).</span><span class="sxs-lookup"><span data-stu-id="f49fd-120">For more information about Azure Identity proxy configuration, see [ProxyOptions](/java/api/com.azure.core.http.proxyoptions.proxyoptions).</span></span>

---
