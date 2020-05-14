---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ffef189622621322fee15cdfc651531bd6a6d0c0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218226"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="94ef4-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="94ef4-103">Get offerShiftRequest</span></span>

<span data-ttu-id="94ef4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94ef4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94ef4-105">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="94ef4-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94ef4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94ef4-106">Permissions</span></span>

<span data-ttu-id="94ef4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94ef4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94ef4-109">Permission type</span></span>                        | <span data-ttu-id="94ef4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94ef4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94ef4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94ef4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94ef4-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="94ef4-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="94ef4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94ef4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ef4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94ef4-114">Not supported.</span></span> |
| <span data-ttu-id="94ef4-115">Application</span><span class="sxs-lookup"><span data-stu-id="94ef4-115">Application</span></span>                            | <span data-ttu-id="94ef4-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="94ef4-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="94ef4-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="94ef4-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="94ef4-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="94ef4-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="94ef4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94ef4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94ef4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94ef4-120">Optional query parameters</span></span>

<span data-ttu-id="94ef4-121">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94ef4-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94ef4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94ef4-122">Request headers</span></span>

| <span data-ttu-id="94ef4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="94ef4-123">Name</span></span>      |<span data-ttu-id="94ef4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="94ef4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94ef4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="94ef4-125">Authorization</span></span> | <span data-ttu-id="94ef4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94ef4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94ef4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94ef4-128">Request body</span></span>

<span data-ttu-id="94ef4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94ef4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94ef4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="94ef4-130">Response</span></span>

<span data-ttu-id="94ef4-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94ef4-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94ef4-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94ef4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94ef4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94ef4-133">Request</span></span>

<span data-ttu-id="94ef4-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94ef4-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94ef4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="94ef4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="94ef4-136">C#</span><span class="sxs-lookup"><span data-stu-id="94ef4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94ef4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ef4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94ef4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94ef4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94ef4-139">Java</span><span class="sxs-lookup"><span data-stu-id="94ef4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="94ef4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="94ef4-140">Response</span></span>

<span data-ttu-id="94ef4-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94ef4-141">The following is an example of the response.</span></span>

> <span data-ttu-id="94ef4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94ef4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
