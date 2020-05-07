---
title: Criar openShiftChangeRequest
description: Criar uma instância de um objeto openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f8f6469b92a8d2fbc289cfa436f2ed97c2204c00
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155044"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="be41c-103">Criar openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="be41c-103">Create openShiftChangeRequest</span></span>

<span data-ttu-id="be41c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be41c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be41c-105">Criar uma instância de um objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="be41c-105">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be41c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be41c-106">Permissions</span></span>

<span data-ttu-id="be41c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be41c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be41c-109">Permission type</span></span>                        | <span data-ttu-id="be41c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be41c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be41c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be41c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be41c-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="be41c-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="be41c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be41c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be41c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be41c-114">Not supported.</span></span> |
| <span data-ttu-id="be41c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be41c-115">Application</span></span>                            | <span data-ttu-id="be41c-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be41c-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="be41c-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="be41c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="be41c-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="be41c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="be41c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be41c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="be41c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be41c-120">Request headers</span></span>

| <span data-ttu-id="be41c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="be41c-121">Name</span></span>      |<span data-ttu-id="be41c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="be41c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be41c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="be41c-123">Authorization</span></span> | <span data-ttu-id="be41c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be41c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be41c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="be41c-126">Content-type</span></span> | <span data-ttu-id="be41c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be41c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be41c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be41c-129">Request body</span></span>
<span data-ttu-id="be41c-130">No corpo da solicitação, forneça uma representação JSON de um novo objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="be41c-130">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="be41c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="be41c-131">Response</span></span>

<span data-ttu-id="be41c-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be41c-132">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be41c-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be41c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be41c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be41c-134">Request</span></span>

<span data-ttu-id="be41c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be41c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="be41c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="be41c-136">Response</span></span>

<span data-ttu-id="be41c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be41c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="be41c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be41c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "assignedTo": "manager",
  "state": "pending",
  "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
  "senderDateTime": "2019-05-01T10:00:00Z",
  "senderMessage": "Can I take this shift?",
  "managerUserId": null,
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create openShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
