---
title: Listar swapShiftsChangeRequest
description: Recupere uma lista de objetos swapShiftsChangeRequest na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c53e4466c52f73967bc0993171c3d4560a104928
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154889"
---
# <a name="list-swapshiftschangerequest"></a><span data-ttu-id="57918-103">Listar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="57918-103">List swapShiftsChangeRequest</span></span>

<span data-ttu-id="57918-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57918-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57918-105">Recupere uma lista de objetos [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) na equipe.</span><span class="sxs-lookup"><span data-stu-id="57918-105">Retrieve a list of [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="57918-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57918-106">Permissions</span></span>

<span data-ttu-id="57918-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57918-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57918-109">Permission type</span></span>                        | <span data-ttu-id="57918-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57918-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="57918-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57918-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57918-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57918-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="57918-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57918-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57918-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57918-114">Not supported.</span></span>    |
|<span data-ttu-id="57918-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57918-115">Application</span></span> | <span data-ttu-id="57918-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57918-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="57918-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="57918-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="57918-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="57918-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="57918-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57918-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57918-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57918-120">Optional query parameters</span></span>

<span data-ttu-id="57918-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57918-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="57918-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="57918-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="57918-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57918-123">Request headers</span></span>

| <span data-ttu-id="57918-124">Nome</span><span class="sxs-lookup"><span data-stu-id="57918-124">Name</span></span>      |<span data-ttu-id="57918-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="57918-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57918-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="57918-126">Authorization</span></span> | <span data-ttu-id="57918-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57918-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57918-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57918-129">Request body</span></span>

<span data-ttu-id="57918-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57918-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57918-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="57918-131">Response</span></span>

<span data-ttu-id="57918-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57918-132">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57918-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57918-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57918-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57918-134">Request</span></span>

<span data-ttu-id="57918-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57918-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests
```
---


### <a name="response"></a><span data-ttu-id="57918-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="57918-136">Response</span></span>

<span data-ttu-id="57918-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57918-137">The following is an example of the response.</span></span>

> <span data-ttu-id="57918-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57918-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
