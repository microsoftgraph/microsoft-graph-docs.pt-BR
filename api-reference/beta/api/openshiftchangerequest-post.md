---
title: Criar openShiftChangeRequest
description: Criar uma instância de um objeto openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fb37f5c65ba04547aebd273df8ada78271a68108
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952206"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="2728e-103">Criar openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="2728e-103">Create openShiftChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2728e-104">Criar uma instância de um objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2728e-104">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2728e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2728e-105">Permissions</span></span>

<span data-ttu-id="2728e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2728e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2728e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2728e-108">Permission type</span></span>                        | <span data-ttu-id="2728e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2728e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2728e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2728e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2728e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2728e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2728e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2728e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2728e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2728e-113">Not supported.</span></span> |
| <span data-ttu-id="2728e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2728e-114">Application</span></span>                            | <span data-ttu-id="2728e-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="2728e-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="2728e-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="2728e-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="2728e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2728e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2728e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2728e-118">Optional query parameters</span></span>

<span data-ttu-id="2728e-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2728e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2728e-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2728e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2728e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2728e-121">Request headers</span></span>

| <span data-ttu-id="2728e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2728e-122">Name</span></span>      |<span data-ttu-id="2728e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2728e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2728e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2728e-124">Authorization</span></span> | <span data-ttu-id="2728e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2728e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2728e-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="2728e-127">Content-type</span></span> | <span data-ttu-id="2728e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2728e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2728e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2728e-130">Request body</span></span>
<span data-ttu-id="2728e-131">No corpo da solicitação, forneça uma representação JSON de um novo objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2728e-131">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2728e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2728e-132">Response</span></span>

<span data-ttu-id="2728e-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2728e-133">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2728e-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2728e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2728e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2728e-135">Request</span></span>

<span data-ttu-id="2728e-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2728e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="2728e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2728e-137">Response</span></span>

<span data-ttu-id="2728e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2728e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="2728e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2728e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
