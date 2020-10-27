---
title: Usar os SDKs do Microsoft Graph com a API beta
description: Descreve como usar os SDKs do Microsoft Graph com a versão beta da API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: fe0272ca46b4bdea1d36048296d1a702b9e1f469
ms.sourcegitcommit: 70e09ebbf67f49a0c64ab7a275e751f8a68b8696
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48771843"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Usar os SDKs do Microsoft Graph com a API beta

Muitos dos SDKs do Microsoft Graph usam o ponto de extremidade do Microsoft Graph [v 1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) por padrão. Os SDKs podem ser usados com o ponto de extremidade [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) para aplicativos de não produção. O método para acessar o ponto de extremidade beta depende de qual SDK você está usando.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

Para chamar a API beta, você deve instalar o pacote [Microsoft. Graph. beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) . O uso é o mesmo do `Microsoft.Graph` pacote.

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

A [biblioteca de cliente JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) pode chamar a API beta de uma das duas maneiras.

- Você pode definir a versão no `MicrosoftGraph.Client` ao criá-la. Todas as solicitações feitas pelo cliente vão para a versão especificada.

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

Para chamar a API beta, você deve instalar o SDK do [Microsoft Graph beta java](https://github.com/microsoftgraph/msgraph-beta-sdk-java). O uso é o mesmo que o SDK não beta.

```Java
IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

O [SDK do Microsoft Graph para ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) exige a criação de uma cadeia de caracteres de URL para a API que você deseja chamar. Ele fornece uma constante `MSGraphBaseURL` para o ponto de extremidade v 1.0. Para usar a versão beta, basta substituir por `https://graph.microsoft.com/beta` .

No entanto, os modelos no [SDK de modelos do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) são gerados de objetos na API v 1.0, de modo que eles podem não funcionar com objetos beta.

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

O [SDK do Microsoft Graph para php](https://github.com/microsoftgraph/msgraph-sdk-php) é compatível com os modelos e o ponto de extremidade beta. Você define o ponto de extremidade beta com o `setApiVersion` método. Você precisará remover a ambiguidade dos modelos v 1.0 e beta fornecendo um alias.

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

---
