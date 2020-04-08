---
title: Obter identityRiskEvent
description: Recupere as propriedades e os relacionamentos do objeto identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a3d0beecec119076e753d4405d08b40f3885e33
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181088"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="7ba95-103">Obter identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7ba95-103">Get identityRiskEvent</span></span>

<span data-ttu-id="7ba95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ba95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="7ba95-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="7ba95-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="7ba95-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="7ba95-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="7ba95-107">Recupere as propriedades e os relacionamentos do objeto identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="7ba95-107">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ba95-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ba95-108">Permissions</span></span>
<span data-ttu-id="7ba95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ba95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ba95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ba95-111">Permission type</span></span>      | <span data-ttu-id="7ba95-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ba95-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ba95-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ba95-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7ba95-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba95-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="7ba95-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ba95-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ba95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ba95-116">Not supported.</span></span>    |
|<span data-ttu-id="7ba95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ba95-117">Application</span></span> | <span data-ttu-id="7ba95-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba95-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ba95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ba95-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7ba95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ba95-120">Request headers</span></span>
| <span data-ttu-id="7ba95-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7ba95-121">Name</span></span>      |<span data-ttu-id="7ba95-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ba95-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ba95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ba95-123">Authorization</span></span>  | <span data-ttu-id="7ba95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ba95-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ba95-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7ba95-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="7ba95-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7ba95-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ba95-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ba95-129">Request body</span></span>
<span data-ttu-id="7ba95-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ba95-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ba95-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ba95-131">Response</span></span>

<span data-ttu-id="7ba95-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ba95-132">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ba95-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ba95-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ba95-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ba95-134">Request</span></span>
<span data-ttu-id="7ba95-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ba95-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ba95-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ba95-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
# <a name="c"></a>[<span data-ttu-id="7ba95-137">C#</span><span class="sxs-lookup"><span data-stu-id="7ba95-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ba95-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ba95-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ba95-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ba95-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7ba95-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ba95-140">Response</span></span>
<span data-ttu-id="7ba95-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ba95-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
