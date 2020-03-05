---
title: Obter swapShiftsChangeRequest
description: Recupere as propriedades e os relacionamentos de um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e1418b83cc8e673afb1055a75849347bdab740d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453055"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="6f7fb-103">Obter swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="6f7fb-103">Get swapShiftsChangeRequest</span></span>

<span data-ttu-id="6f7fb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f7fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f7fb-105">Recupere as propriedades e os relacionamentos de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="6f7fb-105">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f7fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f7fb-106">Permissions</span></span>

<span data-ttu-id="6f7fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f7fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f7fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f7fb-109">Permission type</span></span>                        | <span data-ttu-id="6f7fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f7fb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6f7fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f7fb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f7fb-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7fb-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6f7fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f7fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f7fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-114">Not supported.</span></span> |
| <span data-ttu-id="6f7fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f7fb-115">Application</span></span> | <span data-ttu-id="6f7fb-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="6f7fb-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="6f7fb-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="6f7fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f7fb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f7fb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f7fb-119">Optional query parameters</span></span>

<span data-ttu-id="6f7fb-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6f7fb-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6f7fb-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f7fb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f7fb-122">Request headers</span></span>

| <span data-ttu-id="6f7fb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6f7fb-123">Name</span></span>      |<span data-ttu-id="6f7fb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7fb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f7fb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f7fb-125">Authorization</span></span> | <span data-ttu-id="6f7fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f7fb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f7fb-128">Request body</span></span>

<span data-ttu-id="6f7fb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f7fb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f7fb-130">Response</span></span>

<span data-ttu-id="6f7fb-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-131">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f7fb-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6f7fb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f7fb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f7fb-133">Request</span></span>

<span data-ttu-id="6f7fb-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f7fb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f7fb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```
# <a name="c"></a>[<span data-ttu-id="6f7fb-136">C#</span><span class="sxs-lookup"><span data-stu-id="6f7fb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f7fb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f7fb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f7fb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f7fb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6f7fb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f7fb-139">Response</span></span>

<span data-ttu-id="6f7fb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6f7fb-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
