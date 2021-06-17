---
title: Criar um cliente microsoft Graph
description: Descreve como criar um cliente a ser usado para fazer chamadas para o Microsoft Graph. Inclui como configurar a autenticação e selecionar uma nuvem soberana.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 0256ad20b3078c081102221189a12e27432df058
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971357"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="9c37a-104">Criar um cliente microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9c37a-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="9c37a-105">O cliente Graph Microsoft foi projetado para facilitar as chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9c37a-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="9c37a-106">Você pode usar uma única instância do cliente durante o tempo de vida do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c37a-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="9c37a-107">Para obter informações sobre como adicionar e instalar o pacote de cliente microsoft Graph em seu projeto, consulte [Install the SDK](sdk-installation.md).</span><span class="sxs-lookup"><span data-stu-id="9c37a-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="9c37a-108">Os exemplos de código a seguir mostram como criar uma instância de um cliente microsoft Graph com um provedor de autenticação nos idiomas suportados.</span><span class="sxs-lookup"><span data-stu-id="9c37a-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="9c37a-109">O provedor de autenticação tratará da aquisição de tokens de acesso para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c37a-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="9c37a-110">Muitos provedores de autenticação diferentes estão disponíveis para cada idioma e plataforma.</span><span class="sxs-lookup"><span data-stu-id="9c37a-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="9c37a-111">Os diferentes provedores de aplicativos suportam diferentes cenários de cliente.</span><span class="sxs-lookup"><span data-stu-id="9c37a-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="9c37a-112">Para obter detalhes sobre quais provedores e opções são apropriados para seu cenário, consulte [Choose an Authentication Provider](choose-authentication-providers.md).</span><span class="sxs-lookup"><span data-stu-id="9c37a-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="c"></a>[<span data-ttu-id="9c37a-113">C#</span><span class="sxs-lookup"><span data-stu-id="9c37a-113">C#</span></span>](#tab/CS)

```csharp
// Build a client application.
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create("INSERT-CLIENT-APP-ID")
            .Build();
// Create an authentication provider by passing in a client application and graph scopes.
DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, graphScopes);
// Create a new instance of GraphServiceClient with the authentication provider.
GraphServiceClient graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[<span data-ttu-id="9c37a-114">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c37a-114">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "INSERT-CLIENT-APP-ID"; // Client Id of the registered application

/**
* Create an authProvider to authenticate againt the Microsoft Graph API.
* You can use the TokenCredentialAuthenticationProvider instance with @azure/identity library or
* you can authentication using any MSAL auth library with a custom authentication provider.
*/
const credential = new ClientSecretCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, { scopes: [scopes] });
const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider,
});
```

# <a name="java"></a>[<span data-ttu-id="9c37a-115">Java</span><span class="sxs-lookup"><span data-stu-id="9c37a-115">Java</span></span>](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        .build();

final TokenCredentialAuthProvider tokenCredAuthProvider = new TokenCredentialAuthProvider(SCOPES, clientSecretCredential);

final GraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(tokenCredAuthProvider)
                .buildClient();
```

# <a name="android"></a>[<span data-ttu-id="9c37a-116">Android</span><span class="sxs-lookup"><span data-stu-id="9c37a-116">Android</span></span>](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(CLIENT_ID)
                .redirectUrl("http://localhost:8765")
                .build();

final TokenCredentialAuthProvider tokenCredAuthProvider = new TokenCredentialAuthProvider(SCOPES, interactiveBrowserCredential);

GraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(tokenCredAuthProvider)
                .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="9c37a-117">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c37a-117">Objective-C</span></span>](#tab/Objective-C)

```objc
// Create the authenticationProvider.
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];
MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];
 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];

// Create the client with the authenticationProvider and create a request to the /me resource.
MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me"]]];

// Create the task to send the request and handle the response.
MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler:^(NSData *data, NSURLResponse *response, NSError *error) {

    //Do something

    }];

[meDataTask execute];
```

# <a name="php"></a>[<span data-ttu-id="9c37a-118">PHP</span><span class="sxs-lookup"><span data-stu-id="9c37a-118">PHP</span></span>](#tab/PHP)

```php
// PHP client currently doesn't have an authentication provider. You will need to handle
// getting an access token. The following example demonstrates the client credential
// OAuth flow and assumes that an administrator has consented to the application.
$guzzle = new \GuzzleHttp\Client();
$url = 'https://login.microsoftonline.com/' . $tenantId . '/oauth2/token?api-version=1.0';
$token = json_decode($guzzle->post($url, [
    'form_params' => [
        'client_id' => $clientId,
        'client_secret' => $clientSecret,
        'resource' => 'https://graph.microsoft.com/',
        'grant_type' => 'client_credentials',
    ],
])->getBody()->getContents());
$accessToken = $token->access_token;

// Create a new Graph client.
$graph = new Graph();
$graph->setAccessToken($accessToken);

// Make a call to /me Graph resource.
$user = $graph->createRequest("GET", "/me")
                ->setReturnType(Model\User::class)
                ->execute();
```
---
