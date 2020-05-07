---
title: Listar openShiftChangeRequests
description: Recupere uma lista de objetos openShiftChangeRequest em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c203f9fab489844452eeb6cc341b18af7898eac
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153749"
---
# <a name="list-openshiftchangerequests"></a><span data-ttu-id="2e1cd-103">Listar openShiftChangeRequests</span><span class="sxs-lookup"><span data-stu-id="2e1cd-103">List openShiftChangeRequests</span></span>

<span data-ttu-id="2e1cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e1cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e1cd-105">Recupere uma lista de objetos [openShiftChangeRequest](../resources/openshiftchangerequest.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-105">Retrieve a list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e1cd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e1cd-106">Permissions</span></span>

<span data-ttu-id="2e1cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e1cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e1cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e1cd-109">Permission type</span></span>                        | <span data-ttu-id="2e1cd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e1cd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e1cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e1cd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e1cd-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2e1cd-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2e1cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e1cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e1cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-114">Not supported.</span></span> |
| <span data-ttu-id="2e1cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e1cd-115">Application</span></span>                            | <span data-ttu-id="2e1cd-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2e1cd-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="2e1cd-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2e1cd-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2e1cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e1cd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e1cd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e1cd-120">Optional query parameters</span></span>

<span data-ttu-id="2e1cd-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2e1cd-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2e1cd-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e1cd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e1cd-123">Request headers</span></span>

| <span data-ttu-id="2e1cd-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2e1cd-124">Name</span></span>      |<span data-ttu-id="2e1cd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e1cd-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e1cd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e1cd-126">Authorization</span></span> | <span data-ttu-id="2e1cd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e1cd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e1cd-129">Request body</span></span>

<span data-ttu-id="2e1cd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e1cd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e1cd-131">Response</span></span>

<span data-ttu-id="2e1cd-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e a lista de objetos [openShiftChangeRequest](../resources/openshiftchangerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-132">If successful, this method returns a `200 OK` response code and the list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e1cd-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e1cd-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e1cd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e1cd-134">Request</span></span>

<span data-ttu-id="2e1cd-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="2e1cd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e1cd-136">Response</span></span>

<span data-ttu-id="2e1cd-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-137">The following is an example of the response.</span></span>

> <span data-ttu-id="2e1cd-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e1cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
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
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
