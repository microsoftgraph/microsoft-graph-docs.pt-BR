---
title: Obter identityRiskEvent
description: Recupere as propriedades e as relações do objeto identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2d03271d0b58b9384162290c3e10f8a7c62a963e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040858"
---
# <a name="get-identityriskevent-deprecated"></a><span data-ttu-id="8ec82-103">Obter identityRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="8ec82-103">Get identityRiskEvent (deprecated)</span></span>

<span data-ttu-id="8ec82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ec82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="8ec82-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="8ec82-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="8ec82-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="8ec82-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="8ec82-107">Recupere as propriedades e as relações do objeto identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="8ec82-107">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ec82-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ec82-108">Permissions</span></span>
<span data-ttu-id="8ec82-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec82-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ec82-111">Permission type</span></span>      | <span data-ttu-id="8ec82-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ec82-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ec82-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ec82-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8ec82-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ec82-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="8ec82-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ec82-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ec82-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ec82-116">Not supported.</span></span>    |
|<span data-ttu-id="8ec82-117">Application</span><span class="sxs-lookup"><span data-stu-id="8ec82-117">Application</span></span> | <span data-ttu-id="8ec82-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ec82-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ec82-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ec82-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8ec82-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec82-120">Request headers</span></span>
| <span data-ttu-id="8ec82-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8ec82-121">Name</span></span>      |<span data-ttu-id="8ec82-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec82-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ec82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ec82-123">Authorization</span></span>  | <span data-ttu-id="8ec82-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ec82-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ec82-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ec82-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ec82-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ec82-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ec82-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec82-129">Request body</span></span>
<span data-ttu-id="8ec82-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ec82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ec82-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ec82-131">Response</span></span>

<span data-ttu-id="8ec82-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ec82-132">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ec82-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ec82-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ec82-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec82-134">Request</span></span>
<span data-ttu-id="8ec82-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ec82-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ec82-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ec82-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
# <a name="c"></a>[<span data-ttu-id="8ec82-137">C#</span><span class="sxs-lookup"><span data-stu-id="8ec82-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ec82-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ec82-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ec82-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ec82-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8ec82-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ec82-140">Response</span></span>
<span data-ttu-id="8ec82-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ec82-141">Here is an example of the response.</span></span> <span data-ttu-id="8ec82-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ec82-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


