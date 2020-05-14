---
title: Obter swapShiftsChangeRequest
description: Recupere as propriedades e os relacionamentos de um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d36bc14354e7782f54732d35b7c235ebb512152
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217442"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="36b94-103">Obter swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="36b94-103">Get swapShiftsChangeRequest</span></span>

<span data-ttu-id="36b94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36b94-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36b94-105">Recupere as propriedades e os relacionamentos de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="36b94-105">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36b94-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36b94-106">Permissions</span></span>

<span data-ttu-id="36b94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36b94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36b94-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36b94-109">Permission type</span></span>                        | <span data-ttu-id="36b94-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36b94-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="36b94-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36b94-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36b94-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36b94-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="36b94-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36b94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36b94-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36b94-114">Not supported.</span></span>    |
|<span data-ttu-id="36b94-115">Application</span><span class="sxs-lookup"><span data-stu-id="36b94-115">Application</span></span> | <span data-ttu-id="36b94-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36b94-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="36b94-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="36b94-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="36b94-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="36b94-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="36b94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36b94-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36b94-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36b94-120">Optional query parameters</span></span>

<span data-ttu-id="36b94-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36b94-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="36b94-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="36b94-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36b94-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36b94-123">Request headers</span></span>

| <span data-ttu-id="36b94-124">Nome</span><span class="sxs-lookup"><span data-stu-id="36b94-124">Name</span></span>      |<span data-ttu-id="36b94-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="36b94-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36b94-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="36b94-126">Authorization</span></span> | <span data-ttu-id="36b94-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36b94-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36b94-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36b94-129">Request body</span></span>

<span data-ttu-id="36b94-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36b94-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36b94-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="36b94-131">Response</span></span>

<span data-ttu-id="36b94-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36b94-132">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36b94-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36b94-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36b94-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36b94-134">Request</span></span>

<span data-ttu-id="36b94-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36b94-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36b94-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="36b94-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```
# <a name="c"></a>[<span data-ttu-id="36b94-137">C#</span><span class="sxs-lookup"><span data-stu-id="36b94-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36b94-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36b94-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36b94-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36b94-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36b94-140">Java</span><span class="sxs-lookup"><span data-stu-id="36b94-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-swapshiftschangerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="36b94-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="36b94-141">Response</span></span>

<span data-ttu-id="36b94-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36b94-142">The following is an example of the response.</span></span>

> <span data-ttu-id="36b94-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36b94-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
    "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
    "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c",
    "assignedTo": "manager",
    "state": "approved",
    "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
    "senderDateTime": "2019-05-01T10:00:00Z",
    "senderMessage": "I can't make my shift, any chance we can swap?",
    "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
    "recipientActionDateTime": "2019-05-01T11:00:00Z",
    "recipientActionMessage": "Sure!",
    "managerUserId": "fdcc8d43-7f83-438a-9ab1-098e8f2a95ff",
    "managerActionDateTime": "2019-05-01T12:00:00Z",
    "managerActionMessage": "Approved!"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
