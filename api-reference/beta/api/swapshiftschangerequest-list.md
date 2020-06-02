---
title: Listar swapShiftsChangeRequest
description: Recupere uma lista de objetos swapShiftsChangeRequest na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1c8fce3ac07c0ffbdb70deb09adfcc77f0a66a70
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154364"
---
# <a name="list-swapshiftschangerequest"></a><span data-ttu-id="9f18e-103">Listar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="9f18e-103">List swapShiftsChangeRequest</span></span>

<span data-ttu-id="9f18e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f18e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f18e-105">Recupere uma lista de objetos [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) na equipe.</span><span class="sxs-lookup"><span data-stu-id="9f18e-105">Retrieve a list of [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f18e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f18e-106">Permissions</span></span>

<span data-ttu-id="9f18e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f18e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f18e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f18e-109">Permission type</span></span>                        | <span data-ttu-id="9f18e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f18e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f18e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f18e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f18e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f18e-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9f18e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f18e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f18e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f18e-114">Not supported.</span></span> |
| <span data-ttu-id="9f18e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f18e-115">Application</span></span> | <span data-ttu-id="9f18e-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="9f18e-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="9f18e-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="9f18e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f18e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f18e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f18e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f18e-119">Optional query parameters</span></span>

<span data-ttu-id="9f18e-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f18e-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9f18e-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9f18e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f18e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f18e-122">Request headers</span></span>

| <span data-ttu-id="9f18e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9f18e-123">Name</span></span>      |<span data-ttu-id="9f18e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f18e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f18e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f18e-125">Authorization</span></span> | <span data-ttu-id="9f18e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f18e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f18e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f18e-128">Request body</span></span>

<span data-ttu-id="9f18e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f18e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f18e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f18e-130">Response</span></span>

<span data-ttu-id="9f18e-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f18e-131">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f18e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f18e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f18e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f18e-133">Request</span></span>

<span data-ttu-id="9f18e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f18e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f18e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f18e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests
```
# <a name="c"></a>[<span data-ttu-id="9f18e-136">C#</span><span class="sxs-lookup"><span data-stu-id="9f18e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f18e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f18e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f18e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f18e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f18e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f18e-139">Response</span></span>

<span data-ttu-id="9f18e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f18e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="9f18e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f18e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
