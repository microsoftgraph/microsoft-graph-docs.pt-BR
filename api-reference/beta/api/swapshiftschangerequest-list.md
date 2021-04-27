---
title: Listar swapShiftsChangeRequest
description: Recupere uma lista de objetos swapShiftsChangeRequest na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4992950a05726dde407ea4bc344c5fe0f06e4d49
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054844"
---
# <a name="list-swapshiftschangerequest"></a><span data-ttu-id="fa96b-103">Listar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="fa96b-103">List swapShiftsChangeRequest</span></span>

<span data-ttu-id="fa96b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa96b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa96b-105">Recupere uma lista de [objetos swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) na equipe.</span><span class="sxs-lookup"><span data-stu-id="fa96b-105">Retrieve a list of [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa96b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa96b-106">Permissions</span></span>

<span data-ttu-id="fa96b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa96b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa96b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa96b-109">Permission type</span></span>                        | <span data-ttu-id="fa96b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa96b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa96b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa96b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa96b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa96b-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="fa96b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa96b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa96b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa96b-114">Not supported.</span></span> |
| <span data-ttu-id="fa96b-115">Application</span><span class="sxs-lookup"><span data-stu-id="fa96b-115">Application</span></span> | <span data-ttu-id="fa96b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="fa96b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="fa96b-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="fa96b-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="fa96b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa96b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa96b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa96b-119">Optional query parameters</span></span>

<span data-ttu-id="fa96b-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa96b-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fa96b-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fa96b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa96b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa96b-122">Request headers</span></span>

| <span data-ttu-id="fa96b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fa96b-123">Name</span></span>      |<span data-ttu-id="fa96b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa96b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa96b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa96b-125">Authorization</span></span> | <span data-ttu-id="fa96b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa96b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa96b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa96b-128">Request body</span></span>

<span data-ttu-id="fa96b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa96b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa96b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa96b-130">Response</span></span>

<span data-ttu-id="fa96b-131">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa96b-131">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa96b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa96b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa96b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa96b-133">Request</span></span>

<span data-ttu-id="fa96b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa96b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa96b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa96b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests
```
# <a name="c"></a>[<span data-ttu-id="fa96b-136">C#</span><span class="sxs-lookup"><span data-stu-id="fa96b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa96b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa96b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa96b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa96b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa96b-139">Java</span><span class="sxs-lookup"><span data-stu-id="fa96b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-swapshiftschangerequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa96b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa96b-140">Response</span></span>

<span data-ttu-id="fa96b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa96b-141">The following is an example of the response.</span></span>

> <span data-ttu-id="fa96b-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa96b-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
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
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List swapShiftsChangeRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


