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
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a><span data-ttu-id="a26a9-103">Usar os SDKs do Microsoft Graph com a API beta</span><span class="sxs-lookup"><span data-stu-id="a26a9-103">Use the Microsoft Graph SDKs with the beta API</span></span>

<span data-ttu-id="a26a9-104">Os SDKs do Microsoft Graph usam o ponto de extremidade do Microsoft Graph [v 1.0](/graph/api/overview?view=graph-rest-1.0) por padrão.</span><span class="sxs-lookup"><span data-stu-id="a26a9-104">The Microsoft Graph SDKs use the [v1.0](/graph/api/overview?view=graph-rest-1.0) Microsoft Graph endpoint by default.</span></span> <span data-ttu-id="a26a9-105">Os SDKs podem ser usados com o ponto de extremidade [beta](/graph/api/overview?view=graph-rest-beta) para aplicativos de não produção.</span><span class="sxs-lookup"><span data-stu-id="a26a9-105">The SDKs can be used with the [beta](/graph/api/overview?view=graph-rest-beta) endpoint for non-production applications.</span></span> <span data-ttu-id="a26a9-106">O método para acessar o ponto de extremidade beta depende de qual SDK você está usando.</span><span class="sxs-lookup"><span data-stu-id="a26a9-106">The method for accessing the beta endpoint depends on which SDK you are using.</span></span>

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[<span data-ttu-id="a26a9-107">C#</span><span class="sxs-lookup"><span data-stu-id="a26a9-107">C#</span></span>](#tab/CS)

<span data-ttu-id="a26a9-108">Para chamar a API beta, você deve instalar o pacote [Microsoft. Graph. beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) .</span><span class="sxs-lookup"><span data-stu-id="a26a9-108">In order to call the beta API, you must install the [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) package.</span></span> <span data-ttu-id="a26a9-109">O uso é o mesmo do `Microsoft.Graph` pacote.</span><span class="sxs-lookup"><span data-stu-id="a26a9-109">Usage is the same as the `Microsoft.Graph` package.</span></span>

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

## <a name="typescript"></a>[<span data-ttu-id="a26a9-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a26a9-110">TypeScript</span></span>](#tab/typeScript)

<span data-ttu-id="a26a9-111">A [biblioteca de cliente JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) pode chamar a API beta de uma das duas maneiras.</span><span class="sxs-lookup"><span data-stu-id="a26a9-111">The [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) can call the beta API in one of two ways.</span></span>

- <span data-ttu-id="a26a9-112">Você pode definir a versão no `MicrosoftGraph.Client` ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="a26a9-112">You can set the version on the `MicrosoftGraph.Client` when you create it.</span></span> <span data-ttu-id="a26a9-113">Todas as solicitações feitas pelo cliente vão para a versão especificada.</span><span class="sxs-lookup"><span data-stu-id="a26a9-113">All requests made by the client will go to the specified version.</span></span>

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- <span data-ttu-id="a26a9-114">Você pode definir a versão em uma solicitação específica usando a `version` função no `GraphRequest` objeto.</span><span class="sxs-lookup"><span data-stu-id="a26a9-114">You can set the version on a specific request by using the `version` function on the `GraphRequest` object.</span></span>

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[<span data-ttu-id="a26a9-115">Java</span><span class="sxs-lookup"><span data-stu-id="a26a9-115">Java</span></span>](#tab/Java)

<span data-ttu-id="a26a9-116">Para chamar a API beta, você deve instalar o SDK do [Microsoft Graph beta java](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span><span class="sxs-lookup"><span data-stu-id="a26a9-116">In order to call the beta API, you must install the [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span></span> <span data-ttu-id="a26a9-117">O uso é o mesmo que o SDK não beta.</span><span class="sxs-lookup"><span data-stu-id="a26a9-117">Usage is the same as the non-beta SDK.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a26a9-118">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a26a9-118">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a26a9-119">O [SDK do Microsoft Graph para ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) exige a criação de uma cadeia de caracteres de URL para a API que você deseja chamar.</span><span class="sxs-lookup"><span data-stu-id="a26a9-119">The [Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) requires you to build a URL string to the API you want to call.</span></span> <span data-ttu-id="a26a9-120">Ele fornece uma constante `MSGraphBaseURL` para o ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="a26a9-120">It provides a constant `MSGraphBaseURL` for the v1.0 endpoint.</span></span> <span data-ttu-id="a26a9-121">Para usar a versão beta, basta substituir por `https://graph.microsoft.com/beta` .</span><span class="sxs-lookup"><span data-stu-id="a26a9-121">To use beta, you simply replace that with `https://graph.microsoft.com/beta`.</span></span>

<span data-ttu-id="a26a9-122">No entanto, os modelos no [SDK de modelos do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) são gerados de objetos na API v 1.0, de modo que eles podem não funcionar com objetos beta.</span><span class="sxs-lookup"><span data-stu-id="a26a9-122">However, the models in the [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) are generated from objects in the v1.0 API, so they may not work with beta objects.</span></span>

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

---
