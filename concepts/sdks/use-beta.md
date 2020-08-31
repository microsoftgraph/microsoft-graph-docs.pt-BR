---
title: Usar os SDKs do Microsoft Graph com a API beta
description: Descreve como usar os SDKs do Microsoft Graph com a versão beta da API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: a384384b4172a835160cf12b8e1fb0c06edc7fe7
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312191"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Usar os SDKs do Microsoft Graph com a API beta

Os SDKs do Microsoft Graph usam o ponto de extremidade do Microsoft Graph [v 1.0](/graph/api/overview?view=graph-rest-1.0) por padrão. Os SDKs podem ser usados com o ponto de extremidade [beta](/graph/api/overview?view=graph-rest-beta) para aplicativos de não produção. O método para acessar o ponto de extremidade beta depende de qual SDK você está usando.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

Para chamar a API beta, você deve instalar o pacote [Microsoft. Graph. beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) . O uso é o mesmo do `Microsoft.Graph` pacote.

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

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

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

O [SDK do Microsoft Graph para ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) exige a criação de uma cadeia de caracteres de URL para a API que você deseja chamar. Ele fornece uma constante `MSGraphBaseURL` para o ponto de extremidade v 1.0. Para usar a versão beta, basta substituir por `https://graph.microsoft.com/beta` .

No entanto, os modelos no [SDK de modelos do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) são gerados de objetos na API v 1.0, de modo que eles podem não funcionar com objetos beta.

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

---
