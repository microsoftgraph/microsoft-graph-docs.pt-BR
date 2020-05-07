---
title: Criar offerShiftRequest
description: Criar uma instância de um offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 644d5a2fa0a93a100ecba0e1632c29eae6ad37e6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153552"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="d920f-103">Criar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="d920f-103">Create offerShiftRequest</span></span>

<span data-ttu-id="d920f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d920f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d920f-105">Criar uma instância de um [offerShiftRequest](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="d920f-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d920f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d920f-106">Permissions</span></span>

<span data-ttu-id="d920f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d920f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d920f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d920f-109">Permission type</span></span>                        | <span data-ttu-id="d920f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d920f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d920f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d920f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d920f-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d920f-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d920f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d920f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d920f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d920f-114">Not supported.</span></span> |
| <span data-ttu-id="d920f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d920f-115">Application</span></span>                            | <span data-ttu-id="d920f-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="d920f-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="d920f-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="d920f-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="d920f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d920f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="request-headers"></a><span data-ttu-id="d920f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d920f-119">Request headers</span></span>

| <span data-ttu-id="d920f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d920f-120">Name</span></span>      |<span data-ttu-id="d920f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d920f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d920f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d920f-122">Authorization</span></span> | <span data-ttu-id="d920f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d920f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d920f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d920f-125">Request body</span></span>
<span data-ttu-id="d920f-126">Forneça o novo objeto [offershiftrequest](../resources/offershiftrequest.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="d920f-126">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d920f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d920f-127">Response</span></span>

<span data-ttu-id="d920f-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d920f-128">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d920f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d920f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d920f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d920f-130">Request</span></span>

<span data-ttu-id="d920f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d920f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d920f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d920f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```
# <a name="c"></a>[<span data-ttu-id="d920f-133">C#</span><span class="sxs-lookup"><span data-stu-id="d920f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d920f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d920f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d920f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d920f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d920f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d920f-136">Response</span></span>

<span data-ttu-id="d920f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d920f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="d920f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d920f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
