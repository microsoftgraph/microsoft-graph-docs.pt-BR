---
title: Criar swapshiftRequest
description: Crie uma instância de um swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b1f873194d18f3ec34681f90942d5de2cbb089b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054830"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="6a8dd-103">Criar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="6a8dd-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="6a8dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a8dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a8dd-105">Crie uma instância de um [objeto swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6a8dd-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a8dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a8dd-106">Permissions</span></span>

<span data-ttu-id="6a8dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a8dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a8dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a8dd-109">Permission type</span></span>                        | <span data-ttu-id="6a8dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a8dd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a8dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a8dd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a8dd-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8dd-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a8dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a8dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-114">Not supported.</span></span> |
| <span data-ttu-id="6a8dd-115">Application</span><span class="sxs-lookup"><span data-stu-id="6a8dd-115">Application</span></span>                            | <span data-ttu-id="6a8dd-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="6a8dd-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="6a8dd-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a8dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a8dd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a8dd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a8dd-119">Optional query parameters</span></span>

<span data-ttu-id="6a8dd-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6a8dd-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6a8dd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a8dd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8dd-122">Request headers</span></span>

| <span data-ttu-id="6a8dd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6a8dd-123">Name</span></span>      |<span data-ttu-id="6a8dd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a8dd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a8dd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a8dd-125">Authorization</span></span> | <span data-ttu-id="6a8dd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a8dd-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="6a8dd-128">Content-type</span></span> | <span data-ttu-id="6a8dd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a8dd-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8dd-131">Request body</span></span>
<span data-ttu-id="6a8dd-132">No corpo da solicitação, forneça uma representação JSON de um novo [objeto swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6a8dd-132">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6a8dd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8dd-133">Response</span></span>

<span data-ttu-id="6a8dd-134">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-134">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a8dd-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a8dd-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a8dd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8dd-136">Request</span></span>

<span data-ttu-id="6a8dd-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a8dd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8dd-138">Response</span></span>

<span data-ttu-id="6a8dd-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6a8dd-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6a8dd-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


