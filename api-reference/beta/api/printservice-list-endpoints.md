---
title: Listar printServiceEndpoints
description: Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9441b8e704edb328afa2fe372204f0a2c1acc5ed
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053605"
---
# <a name="list-printserviceendpoints"></a><span data-ttu-id="d28d6-103">Listar printServiceEndpoints</span><span class="sxs-lookup"><span data-stu-id="d28d6-103">List printServiceEndpoints</span></span>

<span data-ttu-id="d28d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d28d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28d6-105">Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="d28d6-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="d28d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d28d6-106">Permissions</span></span>
<span data-ttu-id="d28d6-107">Nenhuma permissão é necessária para chamar essa API, mas para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura universal ativa.</span><span class="sxs-lookup"><span data-stu-id="d28d6-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d28d6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d28d6-108">Permission type</span></span> | <span data-ttu-id="d28d6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d28d6-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d28d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d28d6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d28d6-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d28d6-111">None.</span></span>|
|<span data-ttu-id="d28d6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d28d6-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d28d6-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d28d6-113">None.</span></span>|
|<span data-ttu-id="d28d6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d28d6-114">Application</span></span>|<span data-ttu-id="d28d6-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d28d6-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d28d6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d28d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d28d6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d28d6-117">Optional query parameters</span></span>
<span data-ttu-id="d28d6-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d28d6-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d28d6-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d28d6-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d28d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d28d6-120">Request headers</span></span>
| <span data-ttu-id="d28d6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d28d6-121">Name</span></span>      |<span data-ttu-id="d28d6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d28d6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d28d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d28d6-123">Authorization</span></span> | <span data-ttu-id="d28d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d28d6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d28d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d28d6-126">Request body</span></span>
<span data-ttu-id="d28d6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d28d6-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d28d6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d28d6-128">Response</span></span>
<span data-ttu-id="d28d6-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printServiceEndpoint](../resources/printserviceendpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d28d6-129">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d28d6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d28d6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d28d6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d28d6-131">Request</span></span>
<span data-ttu-id="d28d6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d28d6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d28d6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d28d6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="d28d6-134">C#</span><span class="sxs-lookup"><span data-stu-id="d28d6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d28d6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d28d6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d28d6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d28d6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d28d6-137">Java</span><span class="sxs-lookup"><span data-stu-id="d28d6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d28d6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d28d6-138">Response</span></span>
<span data-ttu-id="d28d6-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d28d6-139">The following is an example of the response.</span></span>
><span data-ttu-id="d28d6-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d28d6-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


