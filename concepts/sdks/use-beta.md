---
title: Usar o Microsoft Graph SDKs com a API beta
description: Descreve como usar o Microsoft Graph SDKs com a versão beta da API.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 8d550c37c998098d07079551a3a4998e85491f9b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992259"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Usar o Microsoft Graph SDKs com a API beta

Muitos dos SDKs do Microsoft Graph usam o ponto de extremidade [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) microsoft Graph por padrão. Os SDKs podem ser usados com o [ponto de extremidade beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) para aplicativos que não são de produção. O método para acessar o ponto de extremidade beta depende de qual SDK você está usando.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD025 -->
# <a name="c"></a>[C#](#tab/CS)

Para chamar a API beta, você deve instalar o [Microsoft.Graph. Pacote Beta.](https://www.nuget.org/packages/Microsoft.Graph.Beta) O uso é igual ao `Microsoft.Graph` pacote.

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

O [Microsoft Graph Biblioteca de Cliente JavaScript](https://github.com/microsoftgraph/msgraph-sdk-javascript) pode chamar a API beta de duas maneiras.

- Você pode definir a versão no `MicrosoftGraph.Client` momento em que a criar. Todas as solicitações feitas pelo cliente irão para a versão especificada.

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- Você pode definir a versão em uma solicitação específica usando a `version` função no `GraphRequest` objeto.

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

Para chamar a API beta, você deve instalar o [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java). O uso é igual ao SDK não beta.

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

O [Microsoft Graph SDK para ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) exige que você crie uma cadeia de caracteres de URL para a API que você deseja chamar. Ele fornece uma constante para o ponto de extremidade `MSGraphBaseURL` v1.0. Para usar beta, você simplesmente substitui isso por `https://graph.microsoft.com/beta` .

No entanto, os modelos no [SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) de modelos do Microsoft Graph são gerados a partir de objetos na API v1.0, portanto, eles podem não funcionar com objetos beta.

```objectivec
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

O [Microsoft Graph SDK para PHP](https://github.com/microsoftgraph/msgraph-sdk-php) dá suporte ao ponto de extremidade beta e modelos. Você definirá o ponto de extremidade beta com o `setApiVersion` método. Você precisará desambiguar os modelos v1.0 e beta fornecendo um alias.

```php
use Microsoft\Graph\Graph;
use Beta\Microsoft\Graph\Model as BetaModel;

class UseBeta
{
    public function run()
    {
        $accessToken = 'xxx';

        $graph = new Graph();
        $graph->setAccessToken($accessToken);

        $user = $graph->setApiVersion("beta")
                      ->createRequest("GET", "/me")
                      ->setReturnType(BetaModel\User::class)
                      ->execute();

        echo "Hello, I am $user->getGivenName() ";
    }
}
```

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Para chamar a API beta, você deve instalar o [pacote do Microsoft Graph Beta SDK para Ir.](https://github.com/microsoftgraph/msgraph-beta-sdk-go)

```go
import (
    msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
    a "github.com/microsoft/kiota/authentication/go/azure"
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(...)

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)
```

---
