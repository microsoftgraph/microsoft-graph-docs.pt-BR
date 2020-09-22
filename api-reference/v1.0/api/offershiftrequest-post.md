---
title: Criar offerShiftRequest
description: Criar uma instância de um offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c9ceee24fc8534e0599382bd0bc0782327fd097e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087108"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="d1261-103">Criar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="d1261-103">Create offerShiftRequest</span></span>

<span data-ttu-id="d1261-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1261-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1261-105">Criar uma instância de um [offerShiftRequest](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="d1261-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1261-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1261-106">Permissions</span></span>

<span data-ttu-id="d1261-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1261-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1261-109">Permission type</span></span>                        | <span data-ttu-id="d1261-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1261-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1261-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1261-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1261-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d1261-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d1261-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1261-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1261-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1261-114">Not supported.</span></span> |
| <span data-ttu-id="d1261-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1261-115">Application</span></span>                            | <span data-ttu-id="d1261-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1261-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="d1261-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d1261-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d1261-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d1261-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d1261-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1261-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="request-headers"></a><span data-ttu-id="d1261-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1261-120">Request headers</span></span>

| <span data-ttu-id="d1261-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d1261-121">Name</span></span>      |<span data-ttu-id="d1261-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1261-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1261-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1261-123">Authorization</span></span> | <span data-ttu-id="d1261-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1261-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1261-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d1261-126">Content-type</span></span> | <span data-ttu-id="d1261-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1261-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1261-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1261-129">Request body</span></span>
<span data-ttu-id="d1261-130">Forneça o novo objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="d1261-130">Provide the new [offerShiftRequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1261-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1261-131">Response</span></span>

<span data-ttu-id="d1261-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1261-132">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1261-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1261-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1261-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1261-134">Request</span></span>

<span data-ttu-id="d1261-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1261-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d1261-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1261-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```
# <a name="c"></a>[<span data-ttu-id="d1261-137">C#</span><span class="sxs-lookup"><span data-stu-id="d1261-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1261-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1261-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1261-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1261-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1261-140">Java</span><span class="sxs-lookup"><span data-stu-id="d1261-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d1261-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1261-141">Response</span></span>

<span data-ttu-id="d1261-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1261-142">The following is an example of the response.</span></span>

> <span data-ttu-id="d1261-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1261-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.etag": "\"4000ee23-0000-0700-0000-5d1415f60000\"",
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "createdDateTime": "2019-09-27T01:01:04.566Z",
  "lastModifiedDateTime": "2019-09-28T01:03:48.874Z",
  "assignedTo": "recipient",
  "state": "pending",
  "senderDateTime": "2019-09-27T01:01:04.566",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "senderUserId": "a4704dd0-3f4c-4f2c-9bb5-8cc575703f30",
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "managerUserId": null,
  "recipientActionDateTime": null,
  "recipientActionMessage": null,
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
      "displayName": "Employee 1"
    }
  }
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

