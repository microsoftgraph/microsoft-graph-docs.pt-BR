---
title: Listar dailyPrintUsageByUser
description: Recupere uma lista de resumos diários de uso de impressão, agrupados pelo usuário.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: accf611304f83e7d3e245f09cbbde14749e84d67
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781206"
---
# <a name="list-dailyprintusagebyuser"></a><span data-ttu-id="0f711-103">Listar dailyPrintUsageByUser</span><span class="sxs-lookup"><span data-stu-id="0f711-103">List dailyPrintUsageByUser</span></span>

<span data-ttu-id="0f711-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f711-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f711-105">Recupere uma lista de resumos diários de uso de impressão, agrupados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="0f711-105">Retrieve a list of daily print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f711-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f711-106">Permissions</span></span>
<span data-ttu-id="0f711-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0f711-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="0f711-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0f711-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f711-110">Permission type</span></span> | <span data-ttu-id="0f711-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f711-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0f711-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f711-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0f711-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f711-113">Reports.Read.All</span></span> |
|<span data-ttu-id="0f711-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f711-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f711-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f711-115">Not Supported.</span></span>|
|<span data-ttu-id="0f711-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f711-116">Application</span></span>|<span data-ttu-id="0f711-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f711-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f711-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f711-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageByUser
GET /print/reports/dailyPrintUsageByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f711-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f711-119">Optional query parameters</span></span>
<span data-ttu-id="0f711-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f711-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0f711-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0f711-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f711-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f711-122">Request headers</span></span>
| <span data-ttu-id="0f711-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0f711-123">Name</span></span>      |<span data-ttu-id="0f711-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f711-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0f711-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f711-125">Authorization</span></span> | <span data-ttu-id="0f711-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f711-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f711-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f711-128">Request body</span></span>
<span data-ttu-id="0f711-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f711-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0f711-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f711-130">Response</span></span>
<span data-ttu-id="0f711-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageByUser](../resources/printUsageByUser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f711-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByUser](../resources/printUsageByUser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f711-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f711-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f711-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f711-133">Request</span></span>
<span data-ttu-id="0f711-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f711-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f711-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f711-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageByUser
```
# <a name="c"></a>[<span data-ttu-id="0f711-136">C#</span><span class="sxs-lookup"><span data-stu-id="0f711-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f711-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f711-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f711-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f711-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f711-139">Java</span><span class="sxs-lookup"><span data-stu-id="0f711-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0f711-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f711-140">Response</span></span>
<span data-ttu-id="0f711-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f711-141">The following is an example of the response.</span></span>
><span data-ttu-id="0f711-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f711-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 268

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "userPrincipalName": "username@contoso.com",
      "usageDate": "2020-02-04T00:00:00.0000000Z",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List dailyPrintUsageByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


