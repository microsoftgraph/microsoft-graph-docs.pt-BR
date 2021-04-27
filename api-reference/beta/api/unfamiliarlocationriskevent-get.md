---
title: Obter unfamiliarLocationRiskEvent
description: Recupere as propriedades e as relações de um objeto unfamiliarlocationriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: aed2480df3792b76b9ebcd3b312eee2ddc4328c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049601"
---
# <a name="get-unfamiliarlocationriskevent-deprecated"></a><span data-ttu-id="3a87a-103">Obter unfamiliarLocationRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="3a87a-103">Get unfamiliarLocationRiskEvent (deprecated)</span></span>

<span data-ttu-id="3a87a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a87a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="3a87a-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="3a87a-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="3a87a-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="3a87a-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="3a87a-107">Recupere as propriedades e as relações de um objeto unfamiliarlocationriskevent.</span><span class="sxs-lookup"><span data-stu-id="3a87a-107">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a87a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a87a-108">Permissions</span></span>
<span data-ttu-id="3a87a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a87a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a87a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a87a-111">Permission type</span></span>      | <span data-ttu-id="3a87a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a87a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a87a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a87a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a87a-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a87a-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3a87a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a87a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a87a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a87a-116">Not supported.</span></span>    |
|<span data-ttu-id="3a87a-117">Application</span><span class="sxs-lookup"><span data-stu-id="3a87a-117">Application</span></span> | <span data-ttu-id="3a87a-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a87a-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a87a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a87a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3a87a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a87a-120">Request headers</span></span>
| <span data-ttu-id="3a87a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3a87a-121">Name</span></span>      |<span data-ttu-id="3a87a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a87a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a87a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a87a-123">Authorization</span></span>  | <span data-ttu-id="3a87a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a87a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a87a-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a87a-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a87a-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3a87a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a87a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a87a-129">Request body</span></span>
<span data-ttu-id="3a87a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a87a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a87a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a87a-131">Response</span></span>

<span data-ttu-id="3a87a-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a87a-132">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a87a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a87a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a87a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a87a-134">Request</span></span>
<span data-ttu-id="3a87a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a87a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="3a87a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a87a-136">Response</span></span>
<span data-ttu-id="3a87a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a87a-137">Here is an example of the response.</span></span> <span data-ttu-id="3a87a-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3a87a-138">Note: The response object shown here might be shortened for readability.</span></span>
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


