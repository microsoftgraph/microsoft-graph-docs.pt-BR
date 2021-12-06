---
title: Criar um cliente microsoft Graph
description: Descreve como criar um cliente a ser usado para fazer chamadas para o Microsoft Graph. Inclui como configurar a autenticação e selecionar uma nuvem soberana.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 0daa9a27ff1a7c92fc39c1eb46c76f38fb34336a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020022"
---
# <a name="create-a-microsoft-graph-client"></a>Criar um cliente microsoft Graph

O cliente Graph Microsoft foi projetado para facilitar as chamadas para o Microsoft Graph. Você pode usar uma única instância do cliente durante o tempo de vida do aplicativo. Para obter informações sobre como adicionar e instalar o pacote de cliente microsoft Graph em seu projeto, consulte [Install the SDK](sdk-installation.md).

Os exemplos de código a seguir mostram como criar uma instância de um cliente microsoft Graph com um provedor de autenticação nos idiomas suportados. O provedor de autenticação tratará da aquisição de tokens de acesso para o aplicativo. Muitos provedores de autenticação diferentes estão disponíveis para cada idioma e plataforma. Os diferentes provedores de autenticação suportam diferentes cenários de cliente. Para obter detalhes sobre quais provedores e opções são apropriados para seu cenário, consulte [Choose an Authentication Provider](choose-authentication-providers.md).

<!-- markdownlint-disable MD025 -->
# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// Callback function that receives the user prompt
// Prompt contains the generated device code that use must
// enter during the auth process in the browser
Func<DeviceCodeInfo, CancellationToken, Task> callback = (code, cancellation) => {
    Console.WriteLine(code.Message);
    return Task.FromResult(0);
};

// https://docs.microsoft.com/dotnet/api/azure.identity.devicecodecredential
var deviceCodeCredential = new DeviceCodeCredential(
    callback, tenantId, clientId, options);

var graphClient = new GraphServiceClient(deviceCodeCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    DeviceCodeCredential
} = require("@azure/identity");

const credential = new DeviceCodeCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

# <a name="java"></a>[Java](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        .build();

final TokenCredentialAuthProvider tokenCredAuthProvider =
        new TokenCredentialAuthProvider(SCOPES, clientSecretCredential);

final GraphServiceClient graphClient = GraphServiceClient
        .builder()
        .authenticationProvider(tokenCredAuthProvider)
        .buildClient();
```

# <a name="android"></a>[Android](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
        .clientId(CLIENT_ID)
        .redirectUrl("http://localhost:8765")
        .build();

final TokenCredentialAuthProvider tokenCredAuthProvider =
        new TokenCredentialAuthProvider(SCOPES, interactiveBrowserCredential);

GraphServiceClient graphClient = GraphServiceClient
        .builder()
        .authenticationProvider(tokenCredAuthProvider)
        .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

```objectivec
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

# <a name="php"></a>[PHP](#tab/PHP)

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

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"
    "fmt"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota/authentication/go/azure"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewDeviceCodeCredential(&azidentity.DeviceCodeCredentialOptions{
    ClientID: "CLIENT_ID",
    UserPrompt: func(ctx context.Context, message azidentity.DeviceCodeMessage) error {
        fmt.Println(message.Message)
        return nil
    },
})

if err != nil {
    fmt.Printf("Error creating credentials: %v\n", err)
    return
}

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

if err != nil {
    fmt.Printf("Error authentication provider: %v\n", err)
    return
}

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)
if err != nil {
    fmt.Printf("Error creating adapter: %v\n", err)
    return
}
client := msgraphsdk.NewGraphServiceClient(adapter)
```

---
