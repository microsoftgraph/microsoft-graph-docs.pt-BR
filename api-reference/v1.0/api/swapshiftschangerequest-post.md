---
title: Criar swapshiftRequest
description: Criar uma instância de um swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fae65ef9812b68bea46960966af7caf694cb3b37
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155016"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="beee2-103">Criar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="beee2-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="beee2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beee2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="beee2-105">Criar uma instância de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="beee2-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="beee2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="beee2-106">Permissions</span></span>

<span data-ttu-id="beee2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="beee2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="beee2-109">Permission type</span></span>                        | <span data-ttu-id="beee2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="beee2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="beee2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="beee2-111">Delegated (work or school account)</span></span> |<span data-ttu-id="beee2-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="beee2-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="beee2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="beee2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beee2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="beee2-114">Not supported.</span></span>    |
|<span data-ttu-id="beee2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beee2-115">Application</span></span> | <span data-ttu-id="beee2-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beee2-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="beee2-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="beee2-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="beee2-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="beee2-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="beee2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="beee2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="beee2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="beee2-120">Optional query parameters</span></span>

<span data-ttu-id="beee2-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="beee2-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="beee2-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="beee2-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="beee2-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="beee2-123">Request headers</span></span>

| <span data-ttu-id="beee2-124">Nome</span><span class="sxs-lookup"><span data-stu-id="beee2-124">Name</span></span>      |<span data-ttu-id="beee2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="beee2-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="beee2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="beee2-126">Authorization</span></span> | <span data-ttu-id="beee2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beee2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="beee2-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="beee2-129">Content-type</span></span> | <span data-ttu-id="beee2-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beee2-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="beee2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="beee2-132">Request body</span></span>
<span data-ttu-id="beee2-133">No corpo da solicitação, forneça uma representação JSON de um novo objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="beee2-133">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="beee2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="beee2-134">Response</span></span>

<span data-ttu-id="beee2-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="beee2-135">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="beee2-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="beee2-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="beee2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="beee2-137">Request</span></span>

<span data-ttu-id="beee2-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="beee2-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/swapShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
  "senderMessage": "I can't make my shift, any chance we can swap?",
  "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
  "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
}
```

### <a name="response"></a><span data-ttu-id="beee2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="beee2-139">Response</span></span>

<span data-ttu-id="beee2-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="beee2-140">The following is an example of the response.</span></span>

> <span data-ttu-id="beee2-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="beee2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
