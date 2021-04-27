---
title: Obter locatedRiskEvent
description: Recupere as propriedades e as relações de um objeto locatedriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-access
author: cloudhandler
ms.openlocfilehash: b0a62ba83d65dec634399bb7780f150aef92c5a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049300"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="55560-103">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="55560-103">Get locatedRiskEvent</span></span>

<span data-ttu-id="55560-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55560-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55560-105">Recupere as propriedades e as relações de um objeto locatedriskevent.</span><span class="sxs-lookup"><span data-stu-id="55560-105">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55560-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55560-106">Permissions</span></span>
<span data-ttu-id="55560-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55560-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55560-109">Permission type</span></span>      | <span data-ttu-id="55560-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55560-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55560-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55560-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55560-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="55560-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="55560-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55560-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55560-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55560-114">Not supported.</span></span>    |
|<span data-ttu-id="55560-115">Application</span><span class="sxs-lookup"><span data-stu-id="55560-115">Application</span></span> | <span data-ttu-id="55560-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="55560-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55560-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55560-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55560-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55560-118">Request headers</span></span>
| <span data-ttu-id="55560-119">Nome</span><span class="sxs-lookup"><span data-stu-id="55560-119">Name</span></span>      |<span data-ttu-id="55560-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55560-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55560-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55560-121">Authorization</span></span>  | <span data-ttu-id="55560-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55560-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55560-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="55560-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="55560-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="55560-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55560-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55560-127">Request body</span></span>
<span data-ttu-id="55560-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55560-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55560-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="55560-129">Response</span></span>

<span data-ttu-id="55560-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e [localizará o objetoRiskEvent](../resources/locatedriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55560-130">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55560-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55560-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55560-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55560-132">Request</span></span>
<span data-ttu-id="55560-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55560-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="55560-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="55560-134">Response</span></span>
<span data-ttu-id="55560-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55560-135">Here is an example of the response.</span></span> <span data-ttu-id="55560-136">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55560-136">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.locatedRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "a6653179-3c7b-4e99-bb4c-dddeb18adfc1",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


