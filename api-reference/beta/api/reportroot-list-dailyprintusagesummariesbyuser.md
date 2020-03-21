---
title: Listar dailyPrintUsageSummariesByUser
description: Recupere uma lista de resumos de uso de impressão diária, agrupados por usuário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 01733cd87ce59e752fb42a4d0cc0401fd4da1837
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895527"
---
# <a name="list-dailyprintusagesummariesbyuser"></a><span data-ttu-id="cc350-103">Listar dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="cc350-103">List dailyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="cc350-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc350-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc350-105">Recupere uma lista de resumos de uso de impressão diária, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="cc350-105">Retrieve a list of daily print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc350-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc350-106">Permissions</span></span>
<span data-ttu-id="cc350-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cc350-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="cc350-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="cc350-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc350-110">Permission type</span></span> | <span data-ttu-id="cc350-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc350-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cc350-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc350-112">Delegated (work or school account)</span></span>| <span data-ttu-id="cc350-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="cc350-113">Users.Read.All</span></span> |
|<span data-ttu-id="cc350-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc350-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc350-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc350-115">Not Supported.</span></span>|
|<span data-ttu-id="cc350-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc350-116">Application</span></span>|<span data-ttu-id="cc350-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc350-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc350-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc350-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser
GET /print/reports/dailyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc350-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc350-119">Optional query parameters</span></span>
<span data-ttu-id="cc350-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc350-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cc350-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cc350-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc350-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc350-122">Request headers</span></span>
| <span data-ttu-id="cc350-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cc350-123">Name</span></span>      |<span data-ttu-id="cc350-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc350-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cc350-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc350-125">Authorization</span></span> | <span data-ttu-id="cc350-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc350-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc350-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc350-128">Request body</span></span>
<span data-ttu-id="cc350-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc350-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cc350-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc350-130">Response</span></span>
<span data-ttu-id="cc350-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc350-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc350-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc350-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc350-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc350-133">Request</span></span>
<span data-ttu-id="cc350-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc350-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser
```
##### <a name="response"></a><span data-ttu-id="cc350-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc350-135">Response</span></span>
<span data-ttu-id="cc350-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc350-136">The following is an example of the response.</span></span>
><span data-ttu-id="cc350-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc350-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "List dailyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->