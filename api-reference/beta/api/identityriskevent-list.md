---
title: Listar identityRiskEvents
description: Recupere uma lista de objetos identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: eb99e6d9a701aa19c96e1123db4d8aa0bd8d8b51
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435396"
---
# <a name="list-identityriskevents-deprecated"></a><span data-ttu-id="3fdb3-103">Listar identityRiskEvents (preterido)</span><span class="sxs-lookup"><span data-stu-id="3fdb3-103">List identityRiskEvents (deprecated)</span></span>

<span data-ttu-id="3fdb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fdb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="3fdb3-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="3fdb3-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="3fdb3-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="3fdb3-107">Recupere uma lista de objetos identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-107">Retrieve a list of identityriskevent objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fdb3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fdb3-108">Permissions</span></span>
<span data-ttu-id="3fdb3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fdb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fdb3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fdb3-111">Permission type</span></span>      | <span data-ttu-id="3fdb3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fdb3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fdb3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fdb3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3fdb3-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fdb3-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3fdb3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fdb3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fdb3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-116">Not supported.</span></span>    |
|<span data-ttu-id="3fdb3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fdb3-117">Application</span></span> | <span data-ttu-id="3fdb3-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fdb3-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fdb3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fdb3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="3fdb3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdb3-120">Request headers</span></span>
| <span data-ttu-id="3fdb3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3fdb3-121">Name</span></span>      |<span data-ttu-id="3fdb3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fdb3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fdb3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fdb3-123">Authorization</span></span>  | <span data-ttu-id="3fdb3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fdb3-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3fdb3-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="3fdb3-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fdb3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdb3-129">Request body</span></span>
<span data-ttu-id="3fdb3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fdb3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fdb3-131">Response</span></span>

<span data-ttu-id="3fdb3-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-132">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fdb3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fdb3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fdb3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdb3-134">Request</span></span>
<span data-ttu-id="3fdb3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3fdb3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fdb3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents
```
# <a name="c"></a>[<span data-ttu-id="3fdb3-137">C#</span><span class="sxs-lookup"><span data-stu-id="3fdb3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fdb3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fdb3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fdb3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fdb3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3fdb3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fdb3-140">Response</span></span>
<span data-ttu-id="3fdb3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fdb3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


