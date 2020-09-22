---
title: Obter suspiciousIpRiskEvent
description: Recupere as propriedades e os relacionamentos de um objeto suspiciousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: c1302d72a6ec8d55d694219a8fc9f27dc004ce85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013878"
---
# <a name="get-suspiciousipriskevent-deprecated"></a><span data-ttu-id="98af0-103">Obter suspiciousIpRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="98af0-103">Get suspiciousIpRiskEvent (deprecated)</span></span>

<span data-ttu-id="98af0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98af0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="98af0-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="98af0-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="98af0-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="98af0-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="98af0-107">Recupere as propriedades e os relacionamentos de um objeto suspiciousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="98af0-107">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="98af0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="98af0-108">Permissions</span></span>
<span data-ttu-id="98af0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98af0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98af0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98af0-111">Permission type</span></span>      | <span data-ttu-id="98af0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98af0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98af0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98af0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="98af0-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="98af0-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="98af0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98af0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98af0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98af0-116">Not supported.</span></span>    |
|<span data-ttu-id="98af0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98af0-117">Application</span></span> | <span data-ttu-id="98af0-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="98af0-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98af0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98af0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="98af0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98af0-120">Request headers</span></span>
| <span data-ttu-id="98af0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="98af0-121">Name</span></span>      |<span data-ttu-id="98af0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="98af0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98af0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="98af0-123">Authorization</span></span>  | <span data-ttu-id="98af0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98af0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98af0-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="98af0-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="98af0-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="98af0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98af0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98af0-129">Request body</span></span>
<span data-ttu-id="98af0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98af0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98af0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="98af0-131">Response</span></span>

<span data-ttu-id="98af0-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98af0-132">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98af0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98af0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98af0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98af0-134">Request</span></span>
<span data-ttu-id="98af0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98af0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="98af0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="98af0-136">Response</span></span>
<span data-ttu-id="98af0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98af0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


