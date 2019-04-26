---
title: Obter impossibleTravelRiskEvent
description: Recupere as propriedades e os relacionamentos de um objeto impossibletravelriskevent.
localization_priority: Normal
ms.openlocfilehash: 0889a14a9a7fd2654fb122963df5b1cc58d0f5c1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328466"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="e33fb-103">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e33fb-103">Get impossibleTravelRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e33fb-104">Recupere as propriedades e os relacionamentos de um objeto impossibletravelriskevent.</span><span class="sxs-lookup"><span data-stu-id="e33fb-104">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e33fb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e33fb-105">Permissions</span></span>
<span data-ttu-id="e33fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e33fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e33fb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e33fb-108">Permission type</span></span>      | <span data-ttu-id="e33fb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e33fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33fb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e33fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e33fb-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33fb-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e33fb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e33fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33fb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33fb-113">Not supported.</span></span>    |
|<span data-ttu-id="e33fb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e33fb-114">Application</span></span> | <span data-ttu-id="e33fb-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33fb-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e33fb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e33fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e33fb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e33fb-117">Request headers</span></span>
| <span data-ttu-id="e33fb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e33fb-118">Name</span></span>      |<span data-ttu-id="e33fb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e33fb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e33fb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e33fb-120">Authorization</span></span>  | <span data-ttu-id="e33fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e33fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e33fb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e33fb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e33fb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e33fb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e33fb-126">Request body</span></span>
<span data-ttu-id="e33fb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e33fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e33fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e33fb-128">Response</span></span>

<span data-ttu-id="e33fb-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e33fb-129">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e33fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e33fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e33fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e33fb-131">Request</span></span>
<span data-ttu-id="e33fb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e33fb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="e33fb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e33fb-133">Response</span></span>
<span data-ttu-id="e33fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e33fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
  "ipAddress": "176.10.104.240",
  "isAtypicalLocation": true,
  "location": "Bern, CH",
  "previousIPAddress": "95.31.18.119",
  "previousLocation": "Moskva, Russia, RU",
  "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "ImpossibleTravelRiskEvent",
  "userAgent": "Firefox 42.0.0.1",
  "userDisplayName": "Jon Doe",
  "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
