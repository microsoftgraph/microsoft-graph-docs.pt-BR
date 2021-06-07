---
title: Listar dailyPrintUsageSummariesByUser
description: Recupere uma lista de resumos diários de uso de impressão, agrupados pelo usuário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bc58cc3565e4d8f7d59c92c157865a2fc58a33fb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757742"
---
# <a name="list-dailyprintusagesummariesbyuser"></a><span data-ttu-id="67f94-103">Listar dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="67f94-103">List dailyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="67f94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67f94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67f94-105">Recupere uma lista de resumos diários de uso de impressão, agrupados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="67f94-105">Retrieve a list of daily print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f94-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67f94-106">Permissions</span></span>
<span data-ttu-id="67f94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="67f94-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="67f94-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="67f94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67f94-110">Permission type</span></span> | <span data-ttu-id="67f94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67f94-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="67f94-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67f94-112">Delegated (work or school account)</span></span>| <span data-ttu-id="67f94-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67f94-113">Reports.Read.All</span></span> |
|<span data-ttu-id="67f94-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67f94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67f94-115">Not Supported.</span></span>|
|<span data-ttu-id="67f94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67f94-116">Application</span></span>|<span data-ttu-id="67f94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67f94-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67f94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67f94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser
GET /print/reports/dailyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67f94-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="67f94-119">Optional query parameters</span></span>
<span data-ttu-id="67f94-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67f94-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="67f94-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="67f94-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="67f94-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67f94-122">Request headers</span></span>
| <span data-ttu-id="67f94-123">Nome</span><span class="sxs-lookup"><span data-stu-id="67f94-123">Name</span></span>      |<span data-ttu-id="67f94-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="67f94-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67f94-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="67f94-125">Authorization</span></span> | <span data-ttu-id="67f94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67f94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67f94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67f94-128">Request body</span></span>
<span data-ttu-id="67f94-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67f94-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67f94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f94-130">Response</span></span>
<span data-ttu-id="67f94-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageSummaryByUser](../resources/printusagesummarybyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67f94-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67f94-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67f94-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67f94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f94-133">Request</span></span>
<span data-ttu-id="67f94-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67f94-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67f94-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f94-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser
```
# <a name="c"></a>[<span data-ttu-id="67f94-136">C#</span><span class="sxs-lookup"><span data-stu-id="67f94-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67f94-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67f94-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67f94-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f94-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67f94-139">Java</span><span class="sxs-lookup"><span data-stu-id="67f94-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67f94-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f94-140">Response</span></span>
<span data-ttu-id="67f94-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67f94-141">The following is an example of the response.</span></span>
><span data-ttu-id="67f94-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="67f94-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser",
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
  "description": "List dailyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


