---
title: Criar um cliente do Microsoft Graph
description: Descreve como criar um cliente para usar o para fazer chamadas para o Microsoft Graph. Inclui como configurar a autenticação e selecionar uma nuvem do soberana.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 3d120f626f3623545366a105aaf9c072c8501e1b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630185"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="0d444-104">Criar um cliente do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d444-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="0d444-105">O cliente do Microsoft Graph foi projetado para simplificar as chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d444-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="0d444-106">Você pode usar uma instância de cliente única para o tempo de vida do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d444-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="0d444-107">Para obter informações sobre como adicionar e instalar o pacote do cliente Microsoft Graph em seu projeto, consulte [install the SDK](sdk-installation.md).</span><span class="sxs-lookup"><span data-stu-id="0d444-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="0d444-108">Os exemplos de código a seguir mostram como criar uma instância de um cliente do Microsoft Graph com um provedor de autenticação nos idiomas com suporte.</span><span class="sxs-lookup"><span data-stu-id="0d444-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="0d444-109">O provedor de autenticação vai lidar com a aquisição de tokens de acesso para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d444-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="0d444-110">Vários provedores de autenticação diferentes estão disponíveis para cada idioma e plataforma.</span><span class="sxs-lookup"><span data-stu-id="0d444-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="0d444-111">Os diferentes provedores de aplicativos dão suporte a diferentes cenários de cliente.</span><span class="sxs-lookup"><span data-stu-id="0d444-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="0d444-112">Para obter detalhes sobre quais provedores e opções são apropriados para o seu cenário, consulte [escolher um provedor de autenticação](choose-authentication-providers.md).</span><span class="sxs-lookup"><span data-stu-id="0d444-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0d444-113">Basic</span><span class="sxs-lookup"><span data-stu-id="0d444-113">C#</span></span>](#tab/CS)

```csharp
var app = DeviceCodeProvider.CreateClientApplication("INSERT-CLIENT-APP-ID");
var authProvider = new DeviceCodeProvider(app);
var client = new GraphServiceClient(authProvider);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d444-114">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d444-114">Javascript</span></span>](#tab/Javascript)

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
const authProvider = new MSALAuthenticationProvider(userAgentApplication, scopes);
```

# <a name="javatabjava"></a>[<span data-ttu-id="0d444-115">Java</span><span class="sxs-lookup"><span data-stu-id="0d444-115">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(CLIENT_ID, SCOPES, CLIENT_SECRET, TENANT_GUID, NATIONAL_CLOUD);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="0d444-116">Android</span><span class="sxs-lookup"><span data-stu-id="0d444-116">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0d444-117">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0d444-117">Objective-C</span></span>](#tab/Objective-C)

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

# <a name="phptabphp"></a>[<span data-ttu-id="0d444-118">PHP</span><span class="sxs-lookup"><span data-stu-id="0d444-118">PHP</span></span>](#tab/PHP)

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
