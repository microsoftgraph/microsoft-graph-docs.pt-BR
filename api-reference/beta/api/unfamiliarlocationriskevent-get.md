---
title: Obter unfamiliarLocationRiskEvent
description: Recupere as propriedades e os relacionamentos de um objeto unfamiliarlocationriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0f09a4b74c3203e92fada0a31e971b930f560276
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863495"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="fc03c-103">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fc03c-103">Get unfamiliarLocationRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="fc03c-104">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="fc03c-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="fc03c-105">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="fc03c-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="fc03c-106">Recupere as propriedades e os relacionamentos de um objeto unfamiliarlocationriskevent.</span><span class="sxs-lookup"><span data-stu-id="fc03c-106">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc03c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc03c-107">Permissions</span></span>
<span data-ttu-id="fc03c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc03c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc03c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc03c-110">Permission type</span></span>      | <span data-ttu-id="fc03c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc03c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc03c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc03c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc03c-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc03c-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="fc03c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc03c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc03c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc03c-115">Not supported.</span></span>    |
|<span data-ttu-id="fc03c-116">Application</span><span class="sxs-lookup"><span data-stu-id="fc03c-116">Application</span></span> | <span data-ttu-id="fc03c-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc03c-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc03c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc03c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc03c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc03c-119">Request headers</span></span>
| <span data-ttu-id="fc03c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fc03c-120">Name</span></span>      |<span data-ttu-id="fc03c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc03c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc03c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc03c-122">Authorization</span></span>  | <span data-ttu-id="fc03c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc03c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc03c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc03c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc03c-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fc03c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc03c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc03c-128">Request body</span></span>
<span data-ttu-id="fc03c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc03c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc03c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc03c-130">Response</span></span>

<span data-ttu-id="fc03c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc03c-131">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc03c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc03c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc03c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc03c-133">Request</span></span>
<span data-ttu-id="fc03c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc03c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="fc03c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc03c-135">Response</span></span>
<span data-ttu-id="fc03c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc03c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
