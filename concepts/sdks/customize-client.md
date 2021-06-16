---
title: Personalizar o cliente de serviço do Microsoft Graph SDK
description: Fornece instruções sobre como alterar o comportamento padrão do cliente de serviço do Microsoft Graph SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d68a8c3b3d1dcd70026217bdbaf99f6a099862d5
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941540"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a>Personalizar o cliente de serviço do Microsoft Graph SDK

O cliente Graph SDK da Microsoft configura um conjunto padrão de middleware que permite que o SDK se comunique com os pontos de extremidade Graph Microsoft. Esse conjunto padrão é personalizável, permitindo que você altere o comportamento do cliente. Por exemplo, você pode inserir o registro em log personalizado ou adicionar um manipulador de teste para simular cenários específicos. Você pode adicionar e remover componentes de middleware. É importante observar que a ordem na qual os componentes de middleware são executados é significativa.

## <a name="c"></a>[C#](#tab/csharp)

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

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

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

### <a name="simpleauthproviderts"></a>SimpleAuthProvider.ts

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

### <a name="customlogginghandlerts"></a>CustomLoggingHandler.ts

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

## <a name="java"></a>[Java](#tab/java)

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

## <a name="configuring-the-http-proxy-for-the-client"></a>Configurando o proxy HTTP para o cliente

Alguns ambientes exigem que os aplicativos cliente usem um proxy HTTP antes que eles possam acessar a Internet pública. Esta seção mostra como configurar o proxy para os SDKs Graph Microsoft.

<!-- markdownlint-disable MD024 -->
## <a name="c"></a>[C#](#tab/csharp)

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

var scopes = new[] { "https://graph.microsoft.com/.default" };

// This example works with Microsoft.Graph 4+
var httpClient = GraphClientFactory.Create(new TokenCredentialAuthProvider(credential, scopes), proxy: new WebProxy(new Uri(proxyAddress)));

GraphServiceClient graphClient = new(httpClient);

/* For Microsoft.Graph version < 4, you'll need to implement an authHandler. Please note
/* that Microsoft.Graph.Auth is deemphasized and will not leave the preview state.

var httpProvider = new HttpProvider(handler, true);
GraphServiceClient graphClient = new(authHandler, httpProvider);

*/
```

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

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

## <a name="java"></a>[Java](#tab/java)

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
> Para obter mais informações sobre a configuração de proxy de Identidade do Azure, consulte [ProxyOptions](/java/api/com.azure.core.http.proxyoptions.proxyoptions).

---
