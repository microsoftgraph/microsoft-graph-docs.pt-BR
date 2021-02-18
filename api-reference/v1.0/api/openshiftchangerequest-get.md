---
title: Get openShiftChangeRequest
description: Recupere as propriedades e os relacionamentos de um objeto openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6cb69d55bf7a0197f2cb06f4a97776a035f58a03
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292592"
---
# <a name="get-openshiftchangerequest"></a><span data-ttu-id="ee7a5-103">Get openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="ee7a5-103">Get openShiftChangeRequest</span></span>

<span data-ttu-id="ee7a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee7a5-105">Recupere as propriedades e os relacionamentos de um [objeto openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ee7a5-105">Retrieve the properties and relationships of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee7a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee7a5-106">Permissions</span></span>

<span data-ttu-id="ee7a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee7a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee7a5-109">Permission type</span></span>                        | <span data-ttu-id="ee7a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee7a5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ee7a5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee7a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee7a5-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7a5-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ee7a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee7a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee7a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-114">Not supported.</span></span> |
| <span data-ttu-id="ee7a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee7a5-115">Application</span></span>                            | <span data-ttu-id="ee7a5-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7a5-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="ee7a5-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ee7a5-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ee7a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee7a5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftChangeRequests/{openShiftsChangeRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee7a5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee7a5-120">Optional query parameters</span></span>

<span data-ttu-id="ee7a5-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee7a5-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ee7a5-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee7a5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7a5-123">Request headers</span></span>

| <span data-ttu-id="ee7a5-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ee7a5-124">Name</span></span>      |<span data-ttu-id="ee7a5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee7a5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee7a5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee7a5-126">Authorization</span></span> | <span data-ttu-id="ee7a5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee7a5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7a5-129">Request body</span></span>

<span data-ttu-id="ee7a5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee7a5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee7a5-131">Response</span></span>

<span data-ttu-id="ee7a5-132">Se bem-sucedido, este método retorna um código de resposta e o objeto `200 OK` [openShiftChangeRequest](../resources/openshiftchangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-132">If successful, this method returns a `200 OK` response code and the requested [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee7a5-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ee7a5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee7a5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7a5-134">Request</span></span>

<span data-ttu-id="ee7a5-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09
```

### <a name="response"></a><span data-ttu-id="ee7a5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee7a5-136">Response</span></span>

<span data-ttu-id="ee7a5-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ee7a5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee7a5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
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
  "description": "Get openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

