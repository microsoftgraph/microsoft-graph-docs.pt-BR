---
title: Listar pontos de extremidade
description: Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 213e80aa3bea4f3eabb49720fce3b97da2972348
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947536"
---
# <a name="list-endpoints"></a><span data-ttu-id="02183-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="02183-103">List endpoints</span></span>

<span data-ttu-id="02183-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02183-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02183-105">Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="02183-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="02183-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02183-106">Permissions</span></span>
<span data-ttu-id="02183-107">Nenhuma permissão é necessária para chamar essa API, mas o locatário do usuário deve ter uma assinatura de impressão universal ativa.</span><span class="sxs-lookup"><span data-stu-id="02183-107">No permissions are needed to call this API, but the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="02183-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02183-108">Permission type</span></span> | <span data-ttu-id="02183-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02183-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="02183-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02183-110">Delegated (work or school account)</span></span>|<span data-ttu-id="02183-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02183-111">None.</span></span>|
|<span data-ttu-id="02183-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02183-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02183-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02183-113">None.</span></span>|
|<span data-ttu-id="02183-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02183-114">Application</span></span>|<span data-ttu-id="02183-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02183-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02183-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02183-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02183-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02183-117">Optional query parameters</span></span>
<span data-ttu-id="02183-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02183-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="02183-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="02183-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="02183-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02183-120">Request headers</span></span>
| <span data-ttu-id="02183-121">Nome</span><span class="sxs-lookup"><span data-stu-id="02183-121">Name</span></span>      |<span data-ttu-id="02183-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="02183-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02183-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02183-123">Authorization</span></span> | <span data-ttu-id="02183-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02183-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02183-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02183-126">Request body</span></span>
<span data-ttu-id="02183-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02183-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="02183-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02183-128">Response</span></span>
<span data-ttu-id="02183-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [AddServiceEndpoint](../resources/printserviceendpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02183-129">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02183-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02183-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02183-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02183-131">Request</span></span>
<span data-ttu-id="02183-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02183-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02183-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="02183-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="02183-134">C#</span><span class="sxs-lookup"><span data-stu-id="02183-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02183-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02183-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02183-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02183-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02183-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="02183-137">Response</span></span>
<span data-ttu-id="02183-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02183-138">The following is an example of the response.</span></span>
><span data-ttu-id="02183-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02183-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "value": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
