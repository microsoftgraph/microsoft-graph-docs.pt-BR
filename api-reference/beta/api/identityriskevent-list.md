---
title: Listar identityRiskEvents
description: Recupere uma lista de objetos identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7a645247b3ff251704010415711e84c805e936ca
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420445"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="331f4-103">Listar identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="331f4-103">List identityRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="331f4-104">Recupere uma lista de objetos identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="331f4-104">Retrieve a list of identityriskevent objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="331f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="331f4-105">Permissions</span></span>
<span data-ttu-id="331f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="331f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="331f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="331f4-108">Permission type</span></span>      | <span data-ttu-id="331f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="331f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="331f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="331f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="331f4-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="331f4-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="331f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="331f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="331f4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="331f4-113">Not supported.</span></span>    |
|<span data-ttu-id="331f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="331f4-114">Application</span></span> | <span data-ttu-id="331f4-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="331f4-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="331f4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="331f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="331f4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="331f4-117">Request headers</span></span>
| <span data-ttu-id="331f4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="331f4-118">Name</span></span>      |<span data-ttu-id="331f4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="331f4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="331f4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="331f4-120">Authorization</span></span>  | <span data-ttu-id="331f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="331f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="331f4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="331f4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="331f4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="331f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="331f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="331f4-126">Request body</span></span>
<span data-ttu-id="331f4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="331f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="331f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="331f4-128">Response</span></span>

<span data-ttu-id="331f4-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="331f4-129">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="331f4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="331f4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="331f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="331f4-131">Request</span></span>
<span data-ttu-id="331f4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="331f4-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="331f4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="331f4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="331f4-134">C#</span><span class="sxs-lookup"><span data-stu-id="331f4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="331f4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="331f4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="331f4-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="331f4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="331f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="331f4-137">Response</span></span>
<span data-ttu-id="331f4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="331f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
