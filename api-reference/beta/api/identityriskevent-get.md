---
title: Obter identityRiskEvent
description: Recupere as propriedades e relações do objeto identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: aaec2759ee3dd6b1e4b12a77124560c5b0985c42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818029"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="33871-103">Obter identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="33871-103">Get identityRiskEvent</span></span>

> <span data-ttu-id="33871-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33871-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33871-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33871-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33871-106">Recupere as propriedades e relações do objeto identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="33871-106">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="33871-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="33871-107">Permissions</span></span>
<span data-ttu-id="33871-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33871-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33871-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33871-110">Permission type</span></span>      | <span data-ttu-id="33871-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33871-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33871-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33871-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33871-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="33871-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="33871-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33871-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33871-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33871-115">Not supported.</span></span>    |
|<span data-ttu-id="33871-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33871-116">Application</span></span> | <span data-ttu-id="33871-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="33871-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33871-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33871-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="33871-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33871-119">Request headers</span></span>
| <span data-ttu-id="33871-120">Nome</span><span class="sxs-lookup"><span data-stu-id="33871-120">Name</span></span>      |<span data-ttu-id="33871-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="33871-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33871-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="33871-122">Authorization</span></span>  | <span data-ttu-id="33871-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33871-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33871-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="33871-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="33871-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="33871-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33871-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33871-128">Request body</span></span>
<span data-ttu-id="33871-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33871-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33871-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="33871-130">Response</span></span>

<span data-ttu-id="33871-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33871-131">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33871-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33871-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33871-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33871-133">Request</span></span>
<span data-ttu-id="33871-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33871-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="33871-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="33871-135">Response</span></span>
<span data-ttu-id="33871-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33871-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
