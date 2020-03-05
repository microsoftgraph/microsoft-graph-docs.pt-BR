---
title: Criar offerShiftRequest
description: Criar uma instância de um offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5532d9749e949d30b0a417908b7804606ead07af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456576"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="c7d06-103">Criar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="c7d06-103">Create offerShiftRequest</span></span>

<span data-ttu-id="c7d06-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7d06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7d06-105">Criar uma instância de um [offerShiftRequest](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c7d06-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7d06-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7d06-106">Permissions</span></span>

<span data-ttu-id="c7d06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7d06-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7d06-109">Permission type</span></span>                        | <span data-ttu-id="c7d06-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7d06-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7d06-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7d06-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7d06-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d06-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c7d06-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7d06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7d06-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7d06-114">Not supported.</span></span> |
| <span data-ttu-id="c7d06-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7d06-115">Application</span></span>                            | <span data-ttu-id="c7d06-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="c7d06-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="c7d06-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="c7d06-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7d06-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d06-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7d06-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7d06-119">Optional query parameters</span></span>

<span data-ttu-id="c7d06-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d06-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c7d06-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c7d06-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7d06-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d06-122">Request headers</span></span>

| <span data-ttu-id="c7d06-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c7d06-123">Name</span></span>      |<span data-ttu-id="c7d06-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7d06-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7d06-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7d06-125">Authorization</span></span> | <span data-ttu-id="c7d06-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7d06-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7d06-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d06-128">Request body</span></span>
<span data-ttu-id="c7d06-129">Forneça o novo objeto [offershiftrequest](../resources/offershiftrequest.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="c7d06-129">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7d06-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d06-130">Response</span></span>

<span data-ttu-id="c7d06-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d06-131">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7d06-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7d06-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7d06-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d06-133">Request</span></span>

<span data-ttu-id="c7d06-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d06-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7d06-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d06-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c7d06-136">C#</span><span class="sxs-lookup"><span data-stu-id="c7d06-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7d06-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7d06-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7d06-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7d06-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7d06-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d06-139">Response</span></span>

<span data-ttu-id="c7d06-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d06-140">The following is an example of the response.</span></span>

> <span data-ttu-id="c7d06-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d06-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
