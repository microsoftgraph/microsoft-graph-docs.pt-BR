---
title: Criar um cliente do Microsoft Graph
description: Descreve como criar um cliente para usar o para fazer chamadas para o Microsoft Graph. Inclui como configurar a autenticação e selecionar uma nuvem do soberana.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: bbcf8a624253a8db0602a9eb8c818980cb9d05b5
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581107"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="2c5f0-104">Criar um cliente do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2c5f0-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="2c5f0-105">O cliente do Microsoft Graph foi projetado para simplificar as chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c5f0-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="2c5f0-106">Você pode usar uma instância de cliente única para o tempo de vida do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c5f0-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="2c5f0-107">Para obter informações sobre como adicionar e instalar o pacote do cliente Microsoft Graph em seu projeto, consulte  [install the SDK](sdk-installation.md).</span><span class="sxs-lookup"><span data-stu-id="2c5f0-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="2c5f0-108">Os exemplos de código a seguir mostram como criar uma instância de um cliente do Microsoft Graph com um provedor de autenticação nos idiomas com suporte.</span><span class="sxs-lookup"><span data-stu-id="2c5f0-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="2c5f0-109">O provedor de autenticação vai lidar com a aquisição de tokens de acesso para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c5f0-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="2c5f0-110">Vários provedores de autenticação diferentes estão disponíveis para cada idioma e plataforma.</span><span class="sxs-lookup"><span data-stu-id="2c5f0-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="2c5f0-111">Os diferentes provedores de aplicativos dão suporte a diferentes cenários de cliente.</span><span class="sxs-lookup"><span data-stu-id="2c5f0-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="2c5f0-112">Para obter detalhes sobre quais provedores e opções são apropriados para o seu cenário, consulte [escolher um provedor de autenticação](choose-authentication-providers.md).</span><span class="sxs-lookup"><span data-stu-id="2c5f0-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="c"></a>[<span data-ttu-id="2c5f0-113">C#</span><span class="sxs-lookup"><span data-stu-id="2c5f0-113">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="2c5f0-114">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c5f0-114">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "INSERT-CLIENT-APP-ID"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MSALAuthenticationProvider(userAgentApplication, graphScopes );
```

# <a name="java"></a>[<span data-ttu-id="2c5f0-115">Java</span><span class="sxs-lookup"><span data-stu-id="2c5f0-115">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(CLIENT_ID, SCOPES, CLIENT_SECRET, TENANT_GUID, NationalCloud.Global);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="android"></a>[<span data-ttu-id="2c5f0-116">Android</span><span class="sxs-lookup"><span data-stu-id="2c5f0-116">Android</span></span>](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "INSERT-CLIENT-APP-ID");

MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="2c5f0-117">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c5f0-117">Objective-C</span></span>](#tab/Objective-C)

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

# <a name="php"></a>[<span data-ttu-id="2c5f0-118">PHP</span><span class="sxs-lookup"><span data-stu-id="2c5f0-118">PHP</span></span>](#tab/PHP)

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
