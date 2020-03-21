---
title: Obter printUsageSummaryByUser
description: Recupere o resumo de uso de um usuário para um determinado período de tempo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: efeb9a9007fbe09636db266f145a294f12ab4d6e
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895530"
---
# <a name="get-printusagesummarybyuser"></a><span data-ttu-id="91df9-103">Obter printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="91df9-103">Get printUsageSummaryByUser</span></span>

<span data-ttu-id="91df9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91df9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91df9-105">Recupere o resumo de uso de um usuário para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="91df9-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="91df9-106">Consulte a documentação do [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) para obter descrições de cada ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="91df9-106">See the [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="91df9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="91df9-107">Permissions</span></span>
<span data-ttu-id="91df9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91df9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="91df9-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="91df9-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="91df9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91df9-111">Permission type</span></span> | <span data-ttu-id="91df9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91df9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="91df9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91df9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="91df9-114">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="91df9-114">Users.Read.All</span></span> |
|<span data-ttu-id="91df9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91df9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91df9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91df9-116">Not Supported.</span></span>|
|<span data-ttu-id="91df9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91df9-117">Application</span></span>|<span data-ttu-id="91df9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91df9-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91df9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91df9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser/{id}
GET /reports/monthlyPrintUsageSummariesByUser/{id}
GET /print/reports/dailyPrintUsageSummariesByUser/{id}
GET /print/reports/monthlyPrintUsageSummariesByUser/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91df9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91df9-120">Request headers</span></span>
| <span data-ttu-id="91df9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="91df9-121">Name</span></span>      |<span data-ttu-id="91df9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="91df9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91df9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="91df9-123">Authorization</span></span> | <span data-ttu-id="91df9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91df9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91df9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91df9-126">Request body</span></span>
<span data-ttu-id="91df9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91df9-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="91df9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="91df9-128">Response</span></span>
<span data-ttu-id="91df9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91df9-129">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91df9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91df9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91df9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91df9-131">Request</span></span>
<span data-ttu-id="91df9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91df9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByUser"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser/{id}
```
##### <a name="response"></a><span data-ttu-id="91df9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="91df9-133">Response</span></span>
<span data-ttu-id="91df9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91df9-134">The following is an example of the response.</span></span>
><span data-ttu-id="91df9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91df9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@microsoft.com",
  "usageDate": "2020-02-04T00:00:00.0000000Z",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageSummaryByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->