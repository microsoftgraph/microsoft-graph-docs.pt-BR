---
title: Listar monthlyPrintUsageSummariesByUser
description: Recupere uma lista de resumos de uso de impressão mensal, agrupados por usuário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0d9246a6206e37600578cc836fe7f476c06e486b
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895522"
---
# <a name="list-monthlyprintusagesummariesbyuser"></a><span data-ttu-id="fbab4-103">Listar monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="fbab4-103">List monthlyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="fbab4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbab4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbab4-105">Recupere uma lista de resumos de uso de impressão mensal, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="fbab4-105">Retrieve a list of monthly print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbab4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fbab4-106">Permissions</span></span>
<span data-ttu-id="fbab4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fbab4-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="fbab4-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="fbab4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbab4-110">Permission type</span></span> | <span data-ttu-id="fbab4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbab4-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fbab4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbab4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="fbab4-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="fbab4-113">Users.Read.All</span></span> |
|<span data-ttu-id="fbab4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbab4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbab4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbab4-115">Not Supported.</span></span>|
|<span data-ttu-id="fbab4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbab4-116">Application</span></span>|<span data-ttu-id="fbab4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbab4-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbab4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbab4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByUser
GET /print/reports/monthlyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbab4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbab4-119">Optional query parameters</span></span>
<span data-ttu-id="fbab4-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbab4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fbab4-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fbab4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbab4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbab4-122">Request headers</span></span>
| <span data-ttu-id="fbab4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fbab4-123">Name</span></span>      |<span data-ttu-id="fbab4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbab4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fbab4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbab4-125">Authorization</span></span> | <span data-ttu-id="fbab4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbab4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbab4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbab4-128">Request body</span></span>
<span data-ttu-id="fbab4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbab4-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fbab4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbab4-130">Response</span></span>
<span data-ttu-id="fbab4-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbab4-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbab4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbab4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbab4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbab4-133">Request</span></span>
<span data-ttu-id="fbab4-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbab4-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByUser
```
##### <a name="response"></a><span data-ttu-id="fbab4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbab4-135">Response</span></span>
<span data-ttu-id="fbab4-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fbab4-136">The following is an example of the response.</span></span>
><span data-ttu-id="fbab4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbab4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "userPrincipalName": "username@microsoft.com",
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