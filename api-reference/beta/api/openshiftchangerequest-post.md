---
title: Criar openShiftChangeRequest
description: Crie uma instância de um objeto openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c991a7b798f114df204c1731eba6a4a71bf29cf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052989"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="aa8bd-103">Criar openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="aa8bd-103">Create openShiftChangeRequest</span></span>

<span data-ttu-id="aa8bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa8bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa8bd-105">Crie instância de um [objeto openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="aa8bd-105">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa8bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa8bd-106">Permissions</span></span>

<span data-ttu-id="aa8bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa8bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa8bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa8bd-109">Permission type</span></span>                        | <span data-ttu-id="aa8bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa8bd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aa8bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa8bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa8bd-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa8bd-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="aa8bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa8bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa8bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-114">Not supported.</span></span> |
| <span data-ttu-id="aa8bd-115">Application</span><span class="sxs-lookup"><span data-stu-id="aa8bd-115">Application</span></span>                            | <span data-ttu-id="aa8bd-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="aa8bd-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="aa8bd-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa8bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa8bd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa8bd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa8bd-119">Optional query parameters</span></span>

<span data-ttu-id="aa8bd-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aa8bd-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aa8bd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa8bd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa8bd-122">Request headers</span></span>

| <span data-ttu-id="aa8bd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="aa8bd-123">Name</span></span>      |<span data-ttu-id="aa8bd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa8bd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa8bd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa8bd-125">Authorization</span></span> | <span data-ttu-id="aa8bd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa8bd-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="aa8bd-128">Content-type</span></span> | <span data-ttu-id="aa8bd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa8bd-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa8bd-131">Request body</span></span>
<span data-ttu-id="aa8bd-132">No corpo da solicitação, forneça uma representação JSON de um novo [objeto openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="aa8bd-132">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aa8bd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa8bd-133">Response</span></span>

<span data-ttu-id="aa8bd-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-134">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa8bd-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aa8bd-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa8bd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa8bd-136">Request</span></span>

<span data-ttu-id="aa8bd-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="aa8bd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa8bd-138">Response</span></span>

<span data-ttu-id="aa8bd-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-139">The following is an example of the response.</span></span>

> <span data-ttu-id="aa8bd-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa8bd-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


