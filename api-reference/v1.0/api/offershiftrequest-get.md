---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37ef0a62174ab2464993025ab170eedc42d904af
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313664"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="4770c-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="4770c-103">Get offerShiftRequest</span></span>

<span data-ttu-id="4770c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4770c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4770c-105">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4770c-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4770c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4770c-106">Permissions</span></span>

<span data-ttu-id="4770c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4770c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4770c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4770c-109">Permission type</span></span>                        | <span data-ttu-id="4770c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4770c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4770c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4770c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4770c-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4770c-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4770c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4770c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4770c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4770c-114">Not supported.</span></span> |
| <span data-ttu-id="4770c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4770c-115">Application</span></span>                            | <span data-ttu-id="4770c-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4770c-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4770c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4770c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4770c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4770c-118">Optional query parameters</span></span>

<span data-ttu-id="4770c-119">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4770c-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4770c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4770c-120">Request headers</span></span>

| <span data-ttu-id="4770c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4770c-121">Name</span></span>      |<span data-ttu-id="4770c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4770c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4770c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4770c-123">Authorization</span></span> | <span data-ttu-id="4770c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4770c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4770c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4770c-126">Request body</span></span>

<span data-ttu-id="4770c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4770c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4770c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4770c-128">Response</span></span>

<span data-ttu-id="4770c-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4770c-129">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4770c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4770c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4770c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4770c-131">Request</span></span>

<span data-ttu-id="4770c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4770c-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4770c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4770c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="4770c-134">C#</span><span class="sxs-lookup"><span data-stu-id="4770c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4770c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4770c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4770c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4770c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4770c-137">Java</span><span class="sxs-lookup"><span data-stu-id="4770c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="4770c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4770c-138">Response</span></span>

<span data-ttu-id="4770c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4770c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4770c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4770c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

