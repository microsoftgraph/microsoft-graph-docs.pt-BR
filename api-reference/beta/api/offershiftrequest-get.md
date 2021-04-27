---
title: Obter offerShiftRequest
description: Recupere as propriedades e as relações de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e3e26ab6978e3af3d30a4d2a6fca038ac954949
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051134"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="4a2f9-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="4a2f9-103">Get offerShiftRequest</span></span>

<span data-ttu-id="4a2f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a2f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a2f9-105">Recupere as propriedades e as relações de um [objeto offerShiftRequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="4a2f9-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a2f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a2f9-106">Permissions</span></span>

<span data-ttu-id="4a2f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a2f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a2f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a2f9-109">Permission type</span></span>                        | <span data-ttu-id="4a2f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a2f9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a2f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a2f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a2f9-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2f9-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4a2f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a2f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a2f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-114">Not supported.</span></span> |
| <span data-ttu-id="4a2f9-115">Application</span><span class="sxs-lookup"><span data-stu-id="4a2f9-115">Application</span></span>                            | <span data-ttu-id="4a2f9-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2f9-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a2f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a2f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a2f9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4a2f9-118">Optional query parameters</span></span>

<span data-ttu-id="4a2f9-119">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a2f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2f9-120">Request headers</span></span>

| <span data-ttu-id="4a2f9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4a2f9-121">Name</span></span>      |<span data-ttu-id="4a2f9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a2f9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a2f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a2f9-123">Authorization</span></span> | <span data-ttu-id="4a2f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a2f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2f9-126">Request body</span></span>

<span data-ttu-id="4a2f9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a2f9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a2f9-128">Response</span></span>

<span data-ttu-id="4a2f9-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-129">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a2f9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4a2f9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a2f9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2f9-131">Request</span></span>

<span data-ttu-id="4a2f9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a2f9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a2f9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="4a2f9-134">C#</span><span class="sxs-lookup"><span data-stu-id="4a2f9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a2f9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a2f9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a2f9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a2f9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a2f9-137">Java</span><span class="sxs-lookup"><span data-stu-id="4a2f9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a2f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a2f9-138">Response</span></span>

<span data-ttu-id="4a2f9-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4a2f9-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a2f9-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


