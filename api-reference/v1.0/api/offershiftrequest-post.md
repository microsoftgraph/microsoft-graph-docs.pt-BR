---
title: Criar offerShiftRequest
description: Criar uma instância de um offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ef58e37eab376098a6aa2c7d77f7a009692f74b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217400"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="de1a4-103">Criar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="de1a4-103">Create offerShiftRequest</span></span>

<span data-ttu-id="de1a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de1a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de1a4-105">Criar uma instância de um [offerShiftRequest](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="de1a4-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="de1a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de1a4-106">Permissions</span></span>

<span data-ttu-id="de1a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de1a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de1a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de1a4-109">Permission type</span></span>                        | <span data-ttu-id="de1a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de1a4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de1a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de1a4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de1a4-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="de1a4-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="de1a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de1a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de1a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de1a4-114">Not supported.</span></span> |
| <span data-ttu-id="de1a4-115">Application</span><span class="sxs-lookup"><span data-stu-id="de1a4-115">Application</span></span>                            | <span data-ttu-id="de1a4-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de1a4-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="de1a4-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="de1a4-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="de1a4-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="de1a4-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="de1a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de1a4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="request-headers"></a><span data-ttu-id="de1a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de1a4-120">Request headers</span></span>

| <span data-ttu-id="de1a4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="de1a4-121">Name</span></span>      |<span data-ttu-id="de1a4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="de1a4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de1a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de1a4-123">Authorization</span></span> | <span data-ttu-id="de1a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de1a4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de1a4-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="de1a4-126">Content-type</span></span> | <span data-ttu-id="de1a4-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de1a4-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de1a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de1a4-129">Request body</span></span>
<span data-ttu-id="de1a4-130">Forneça o novo objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="de1a4-130">Provide the new [offerShiftRequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de1a4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="de1a4-131">Response</span></span>

<span data-ttu-id="de1a4-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de1a4-132">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de1a4-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de1a4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de1a4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de1a4-134">Request</span></span>

<span data-ttu-id="de1a4-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de1a4-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="de1a4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="de1a4-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="de1a4-137">C#</span><span class="sxs-lookup"><span data-stu-id="de1a4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de1a4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de1a4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de1a4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de1a4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de1a4-140">Java</span><span class="sxs-lookup"><span data-stu-id="de1a4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="de1a4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="de1a4-141">Response</span></span>

<span data-ttu-id="de1a4-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de1a4-142">The following is an example of the response.</span></span>

> <span data-ttu-id="de1a4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de1a4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
