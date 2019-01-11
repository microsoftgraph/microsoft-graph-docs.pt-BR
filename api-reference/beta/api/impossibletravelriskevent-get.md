---
title: Obter impossibleTravelRiskEvent
description: Recupere as propriedades e relacionamentos de um objeto impossibletravelriskevent.
localization_priority: Normal
ms.openlocfilehash: 6f9c6913fe1bdcd5576814f170eb75d51b28da40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843943"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="4f83b-103">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4f83b-103">Get impossibleTravelRiskEvent</span></span>

> <span data-ttu-id="4f83b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4f83b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f83b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4f83b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f83b-106">Recupere as propriedades e relacionamentos de um objeto impossibletravelriskevent.</span><span class="sxs-lookup"><span data-stu-id="4f83b-106">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f83b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4f83b-107">Permissions</span></span>
<span data-ttu-id="4f83b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f83b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f83b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f83b-110">Permission type</span></span>      | <span data-ttu-id="4f83b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f83b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f83b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f83b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4f83b-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f83b-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="4f83b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f83b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f83b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f83b-115">Not supported.</span></span>    |
|<span data-ttu-id="4f83b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f83b-116">Application</span></span> | <span data-ttu-id="4f83b-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f83b-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f83b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f83b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4f83b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f83b-119">Request headers</span></span>
| <span data-ttu-id="4f83b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4f83b-120">Name</span></span>      |<span data-ttu-id="4f83b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f83b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f83b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f83b-122">Authorization</span></span>  | <span data-ttu-id="4f83b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f83b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f83b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f83b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f83b-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4f83b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f83b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f83b-128">Request body</span></span>
<span data-ttu-id="4f83b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f83b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f83b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f83b-130">Response</span></span>

<span data-ttu-id="4f83b-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f83b-131">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f83b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f83b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f83b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f83b-133">Request</span></span>
<span data-ttu-id="4f83b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f83b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="4f83b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f83b-135">Response</span></span>
<span data-ttu-id="4f83b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f83b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
