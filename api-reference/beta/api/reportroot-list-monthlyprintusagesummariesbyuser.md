---
title: Listar monthlyPrintUsageSummariesByUser
description: Recupere uma lista de resumos de uso de impressão mensal, agrupados pelo usuário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 92711998839e35e518b79b7685e0b3e1eab116ea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054900"
---
# <a name="list-monthlyprintusagesummariesbyuser"></a><span data-ttu-id="04470-103">Listar monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="04470-103">List monthlyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="04470-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04470-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04470-105">Recupere uma lista de resumos de uso de impressão mensal, agrupados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="04470-105">Retrieve a list of monthly print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="04470-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04470-106">Permissions</span></span>
<span data-ttu-id="04470-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="04470-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="04470-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="04470-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04470-110">Permission type</span></span> | <span data-ttu-id="04470-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04470-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="04470-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04470-112">Delegated (work or school account)</span></span>| <span data-ttu-id="04470-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04470-113">Reports.Read.All</span></span> |
|<span data-ttu-id="04470-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04470-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04470-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04470-115">Not Supported.</span></span>|
|<span data-ttu-id="04470-116">Application</span><span class="sxs-lookup"><span data-stu-id="04470-116">Application</span></span>|<span data-ttu-id="04470-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04470-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04470-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04470-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByUser
GET /print/reports/monthlyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04470-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04470-119">Optional query parameters</span></span>
<span data-ttu-id="04470-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04470-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="04470-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="04470-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="04470-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04470-122">Request headers</span></span>
| <span data-ttu-id="04470-123">Nome</span><span class="sxs-lookup"><span data-stu-id="04470-123">Name</span></span>      |<span data-ttu-id="04470-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="04470-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="04470-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="04470-125">Authorization</span></span> | <span data-ttu-id="04470-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04470-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04470-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04470-128">Request body</span></span>
<span data-ttu-id="04470-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04470-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="04470-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="04470-130">Response</span></span>
<span data-ttu-id="04470-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageSummaryByUser](../resources/printusagesummarybyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04470-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04470-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04470-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04470-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04470-133">Request</span></span>
<span data-ttu-id="04470-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04470-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04470-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="04470-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_6"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByUser
```
# <a name="c"></a>[<span data-ttu-id="04470-136">C#</span><span class="sxs-lookup"><span data-stu-id="04470-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04470-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04470-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04470-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04470-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04470-139">Java</span><span class="sxs-lookup"><span data-stu-id="04470-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="04470-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="04470-140">Response</span></span>
<span data-ttu-id="04470-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04470-141">The following is an example of the response.</span></span>
><span data-ttu-id="04470-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="04470-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List monthlyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


