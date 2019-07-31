---
title: Obter locatedRiskEvent
description: Recupere as propriedades e os relacionamentos de um objeto locatedriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a90ecf29119a74e3d102e61ca1f2987683d5c54d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984087"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="d91ae-103">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d91ae-103">Get locatedRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d91ae-104">Recupere as propriedades e os relacionamentos de um objeto locatedriskevent.</span><span class="sxs-lookup"><span data-stu-id="d91ae-104">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d91ae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d91ae-105">Permissions</span></span>
<span data-ttu-id="d91ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d91ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d91ae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d91ae-108">Permission type</span></span>      | <span data-ttu-id="d91ae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d91ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d91ae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d91ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d91ae-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d91ae-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="d91ae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d91ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d91ae-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d91ae-113">Not supported.</span></span>    |
|<span data-ttu-id="d91ae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d91ae-114">Application</span></span> | <span data-ttu-id="d91ae-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d91ae-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d91ae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d91ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d91ae-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d91ae-117">Request headers</span></span>
| <span data-ttu-id="d91ae-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d91ae-118">Name</span></span>      |<span data-ttu-id="d91ae-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d91ae-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d91ae-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d91ae-120">Authorization</span></span>  | <span data-ttu-id="d91ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d91ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d91ae-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d91ae-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d91ae-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d91ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d91ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d91ae-126">Request body</span></span>
<span data-ttu-id="d91ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d91ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d91ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d91ae-128">Response</span></span>

<span data-ttu-id="d91ae-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [locatedRiskEvent](../resources/locatedriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d91ae-129">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d91ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d91ae-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d91ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d91ae-131">Request</span></span>
<span data-ttu-id="d91ae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d91ae-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="d91ae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d91ae-133">Response</span></span>
<span data-ttu-id="d91ae-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d91ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
