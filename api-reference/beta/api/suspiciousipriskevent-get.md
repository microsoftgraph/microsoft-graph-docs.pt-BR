---
title: Obter suspiciousIpRiskEvent
description: Recupere as propriedades e relacionamentos de um objeto suspiciousipriskevent.
ms.openlocfilehash: 3fa7625e01beb6b847bde602c7ccfd0d42d80904
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037828"
---
# <a name="get-suspiciousipriskevent"></a><span data-ttu-id="14579-103">Obter suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="14579-103">Get suspiciousIpRiskEvent</span></span>

> <span data-ttu-id="14579-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="14579-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14579-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="14579-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14579-106">Recupere as propriedades e relacionamentos de um objeto suspiciousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="14579-106">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="14579-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="14579-107">Permissions</span></span>
<span data-ttu-id="14579-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14579-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14579-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14579-110">Permission type</span></span>      | <span data-ttu-id="14579-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14579-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14579-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14579-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14579-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="14579-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="14579-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14579-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14579-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14579-115">Not supported.</span></span>    |
|<span data-ttu-id="14579-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14579-116">Application</span></span> | <span data-ttu-id="14579-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="14579-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14579-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14579-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="14579-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14579-119">Request headers</span></span>
| <span data-ttu-id="14579-120">Nome</span><span class="sxs-lookup"><span data-stu-id="14579-120">Name</span></span>      |<span data-ttu-id="14579-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="14579-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14579-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14579-122">Authorization</span></span>  | <span data-ttu-id="14579-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14579-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14579-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="14579-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="14579-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="14579-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14579-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14579-128">Request body</span></span>
<span data-ttu-id="14579-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14579-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14579-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="14579-130">Response</span></span>

<span data-ttu-id="14579-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14579-131">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14579-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14579-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14579-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14579-133">Request</span></span>
<span data-ttu-id="14579-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14579-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="14579-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="14579-135">Response</span></span>
<span data-ttu-id="14579-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14579-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": null,
  "createdDateTime": "2016-02-03T06:08:35.123512Z",
  "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
  "ipAddress": "95.31.18.119",
  "location": "Moskva, Russia, RU",
  "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
  "riskEventStatus": "active",
  "riskLevel": "low",
  "riskType": "SuspiciousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
