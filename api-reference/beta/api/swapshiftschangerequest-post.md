---
title: Criar swapshiftRequest
description: Criar uma instância de um swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1563837620e65c71ec834b8b877a795e5e0e5c22
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154392"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="a9ee4-103">Criar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="a9ee4-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="a9ee4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9ee4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ee4-105">Criar uma instância de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a9ee4-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9ee4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9ee4-106">Permissions</span></span>

<span data-ttu-id="a9ee4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9ee4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9ee4-109">Permission type</span></span>                        | <span data-ttu-id="a9ee4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9ee4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9ee4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9ee4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9ee4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9ee4-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a9ee4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9ee4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ee4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-114">Not supported.</span></span> |
| <span data-ttu-id="a9ee4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9ee4-115">Application</span></span>                            | <span data-ttu-id="a9ee4-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="a9ee4-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a9ee4-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9ee4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9ee4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9ee4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9ee4-119">Optional query parameters</span></span>

<span data-ttu-id="a9ee4-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a9ee4-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9ee4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9ee4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ee4-122">Request headers</span></span>

| <span data-ttu-id="a9ee4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a9ee4-123">Name</span></span>      |<span data-ttu-id="a9ee4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ee4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9ee4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9ee4-125">Authorization</span></span> | <span data-ttu-id="a9ee4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9ee4-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="a9ee4-128">Content-type</span></span> | <span data-ttu-id="a9ee4-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9ee4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ee4-131">Request body</span></span>
<span data-ttu-id="a9ee4-132">No corpo da solicitação, forneça uma representação JSON de um novo objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a9ee4-132">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a9ee4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9ee4-133">Response</span></span>

<span data-ttu-id="a9ee4-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-134">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9ee4-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9ee4-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9ee4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ee4-136">Request</span></span>

<span data-ttu-id="a9ee4-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/swapShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
  "senderMessage": "I can't make my shift, any chance we can swap?",
  "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
  "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
}
```

### <a name="response"></a><span data-ttu-id="a9ee4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9ee4-138">Response</span></span>

<span data-ttu-id="a9ee4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a9ee4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9ee4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
"assignedTo": "recipient",
"state": "pending",
"senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
"senderDateTime": "2019-05-01T10:00:00Z",
"senderMessage": "I can't make my shift, any chance we can swap?",
"recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
"recipientActionDateTime": null,
"recipientActionMessage": null,
"managerUserId": null,
"managerActionDateTime": null,
"managerActionMessage": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create swapShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
