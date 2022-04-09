---
title: Usar os SDKs Graph Microsoft com a API beta
description: Descreve como usar os SDKs do Microsoft Graph com a versão beta da API.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: aee313a4f4e5eb9efd68c9fd0877dcc96722633c
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733189"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Usar os SDKs Graph Microsoft com a API beta

Muitos dos SDKs do Microsoft Graph usam o ponto de [extremidade do Microsoft Graph v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) por padrão. Os SDKs podem ser usados com o ponto de extremidade [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) para aplicativos de não produção. O método para acessar o ponto de extremidade beta depende de qual SDK você está usando.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD025 -->
# <a name="c"></a>[C#](#tab/CS)

Para chamar a API beta, você deve instalar o [Microsoft.Graph. Pacote beta](https://www.nuget.org/packages/Microsoft.Graph.Beta). O uso é o mesmo que o `Microsoft.Graph` pacote.

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

A [Biblioteca Graph Cliente JavaScript da Microsoft](https://github.com/microsoftgraph/msgraph-sdk-javascript) pode chamar a API beta de uma das duas maneiras.

- Você pode definir a versão no momento `MicrosoftGraph.Client` em que a cria. Todas as solicitações feitas pelo cliente irão para a versão especificada.

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

Para chamar a API beta, você deve instalar o [SDK do Java Graph Beta da Microsoft](https://github.com/microsoftgraph/msgraph-beta-sdk-java). O uso é o mesmo que o SDK não beta.

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

O [Microsoft Graph SDK para ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) exige que você crie uma cadeia de caracteres de URL para a API que você deseja chamar. Ele fornece uma constante `MSGraphBaseURL` para o ponto de extremidade v1.0. Para usar beta, basta substituí-lo por `https://graph.microsoft.com/beta`.

No entanto, os modelos no [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) são gerados a partir de objetos na API v1.0, portanto, eles podem não funcionar com objetos beta.

```objectivec
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

O [Microsoft Graph SDK para PHP](https://github.com/microsoftgraph/msgraph-sdk-php) dá suporte ao ponto de extremidade beta e aos modelos. Você define o ponto de extremidade beta com o `setApiVersion` método. Você precisará desambiguar os modelos v1.0 e beta fornecendo um alias.

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

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Para chamar a API beta, você deve instalar o pacote do [SDK do Microsoft Graph Beta para Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go).

```go
import (
    msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
    a "github.com/microsoft/kiota-authentication-azure-go"
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(...)

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)
```

---
