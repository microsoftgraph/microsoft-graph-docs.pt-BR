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
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a><span data-ttu-id="c28bc-103">Usar os SDKs do Microsoft Graph com a API beta</span><span class="sxs-lookup"><span data-stu-id="c28bc-103">Use the Microsoft Graph SDKs with the beta API</span></span>

<span data-ttu-id="c28bc-104">Muitos dos SDKs do Microsoft Graph usam o ponto de extremidade do Microsoft Graph [v 1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) por padrão.</span><span class="sxs-lookup"><span data-stu-id="c28bc-104">Many of the Microsoft Graph SDKs use the [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph endpoint by default.</span></span> <span data-ttu-id="c28bc-105">Os SDKs podem ser usados com o ponto de extremidade [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) para aplicativos de não produção.</span><span class="sxs-lookup"><span data-stu-id="c28bc-105">The SDKs can be used with the [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) endpoint for non-production applications.</span></span> <span data-ttu-id="c28bc-106">O método para acessar o ponto de extremidade beta depende de qual SDK você está usando.</span><span class="sxs-lookup"><span data-stu-id="c28bc-106">The method for accessing the beta endpoint depends on which SDK you are using.</span></span>

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[<span data-ttu-id="c28bc-107">C#</span><span class="sxs-lookup"><span data-stu-id="c28bc-107">C#</span></span>](#tab/CS)

<span data-ttu-id="c28bc-108">Para chamar a API beta, você deve instalar o pacote [Microsoft. Graph. beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) .</span><span class="sxs-lookup"><span data-stu-id="c28bc-108">In order to call the beta API, you must install the [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) package.</span></span> <span data-ttu-id="c28bc-109">O uso é o mesmo do `Microsoft.Graph` pacote.</span><span class="sxs-lookup"><span data-stu-id="c28bc-109">Usage is the same as the `Microsoft.Graph` package.</span></span>

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[<span data-ttu-id="c28bc-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="c28bc-110">TypeScript</span></span>](#tab/typeScript)

<span data-ttu-id="c28bc-111">A [biblioteca de cliente JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) pode chamar a API beta de uma das duas maneiras.</span><span class="sxs-lookup"><span data-stu-id="c28bc-111">The [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) can call the beta API in one of two ways.</span></span>

- <span data-ttu-id="c28bc-112">Você pode definir a versão no `MicrosoftGraph.Client` ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="c28bc-112">You can set the version on the `MicrosoftGraph.Client` when you create it.</span></span> <span data-ttu-id="c28bc-113">Todas as solicitações feitas pelo cliente vão para a versão especificada.</span><span class="sxs-lookup"><span data-stu-id="c28bc-113">All requests made by the client will go to the specified version.</span></span>

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- <span data-ttu-id="c28bc-114">Você pode definir a versão em uma solicitação específica usando a `version` função no `GraphRequest` objeto.</span><span class="sxs-lookup"><span data-stu-id="c28bc-114">You can set the version on a specific request by using the `version` function on the `GraphRequest` object.</span></span>

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[<span data-ttu-id="c28bc-115">Java</span><span class="sxs-lookup"><span data-stu-id="c28bc-115">Java</span></span>](#tab/Java)

<span data-ttu-id="c28bc-116">Para chamar a API beta, você deve instalar o SDK do [Microsoft Graph beta java](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span><span class="sxs-lookup"><span data-stu-id="c28bc-116">In order to call the beta API, you must install the [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span></span> <span data-ttu-id="c28bc-117">O uso é o mesmo que o SDK não beta.</span><span class="sxs-lookup"><span data-stu-id="c28bc-117">Usage is the same as the non-beta SDK.</span></span>

```Java
IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="c28bc-118">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c28bc-118">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c28bc-119">O [SDK do Microsoft Graph para ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) exige a criação de uma cadeia de caracteres de URL para a API que você deseja chamar.</span><span class="sxs-lookup"><span data-stu-id="c28bc-119">The [Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) requires you to build a URL string to the API you want to call.</span></span> <span data-ttu-id="c28bc-120">Ele fornece uma constante `MSGraphBaseURL` para o ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="c28bc-120">It provides a constant `MSGraphBaseURL` for the v1.0 endpoint.</span></span> <span data-ttu-id="c28bc-121">Para usar a versão beta, basta substituir por `https://graph.microsoft.com/beta` .</span><span class="sxs-lookup"><span data-stu-id="c28bc-121">To use beta, you simply replace that with `https://graph.microsoft.com/beta`.</span></span>

<span data-ttu-id="c28bc-122">No entanto, os modelos no [SDK de modelos do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) são gerados de objetos na API v 1.0, de modo que eles podem não funcionar com objetos beta.</span><span class="sxs-lookup"><span data-stu-id="c28bc-122">However, the models in the [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) are generated from objects in the v1.0 API, so they may not work with beta objects.</span></span>

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[<span data-ttu-id="c28bc-123">PHP</span><span class="sxs-lookup"><span data-stu-id="c28bc-123">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c28bc-124">O [SDK do Microsoft Graph para php](https://github.com/microsoftgraph/msgraph-sdk-php) é compatível com os modelos e o ponto de extremidade beta.</span><span class="sxs-lookup"><span data-stu-id="c28bc-124">The [Microsoft Graph SDK for PHP](https://github.com/microsoftgraph/msgraph-sdk-php) supports the beta endpoint and models.</span></span> <span data-ttu-id="c28bc-125">Você define o ponto de extremidade beta com o `setApiVersion` método.</span><span class="sxs-lookup"><span data-stu-id="c28bc-125">You set the beta endpoint with the `setApiVersion` method.</span></span> <span data-ttu-id="c28bc-126">Você precisará remover a ambiguidade dos modelos v 1.0 e beta fornecendo um alias.</span><span class="sxs-lookup"><span data-stu-id="c28bc-126">You will need to disambiguate the v1.0 and beta models by providing an alias.</span></span>

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
