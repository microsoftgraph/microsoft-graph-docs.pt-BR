---
title: Listar openShiftChangeRequests
description: Recupere uma lista de objetos openShiftChangeRequest em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9beb83beff4b2c80ee267f3e967fc12619017e42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071910"
---
# <a name="list-openshiftchangerequests"></a><span data-ttu-id="15411-103">Listar openShiftChangeRequests</span><span class="sxs-lookup"><span data-stu-id="15411-103">List openShiftChangeRequests</span></span>

<span data-ttu-id="15411-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15411-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15411-105">Recupere uma lista de objetos [openShiftChangeRequest](../resources/openshiftchangerequest.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="15411-105">Retrieve a list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="15411-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15411-106">Permissions</span></span>

<span data-ttu-id="15411-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15411-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15411-109">Permission type</span></span>                        | <span data-ttu-id="15411-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15411-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15411-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15411-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="15411-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="15411-112">Group.ReadWrite.All, Group.Read.All</span></span> |
| <span data-ttu-id="15411-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15411-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15411-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15411-114">Not supported.</span></span> |
| <span data-ttu-id="15411-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15411-115">Application</span></span>                            | <span data-ttu-id="15411-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15411-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15411-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15411-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15411-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15411-118">Optional query parameters</span></span>

<span data-ttu-id="15411-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15411-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="15411-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="15411-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="15411-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15411-121">Request headers</span></span>

| <span data-ttu-id="15411-122">Nome</span><span class="sxs-lookup"><span data-stu-id="15411-122">Name</span></span>      |<span data-ttu-id="15411-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="15411-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15411-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15411-124">Authorization</span></span> | <span data-ttu-id="15411-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15411-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15411-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15411-127">Request body</span></span>

<span data-ttu-id="15411-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15411-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15411-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="15411-129">Response</span></span>

<span data-ttu-id="15411-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a lista de objetos [openShiftChangeRequest](../resources/openshiftchangerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15411-130">If successful, this method returns a `200 OK` response code and the list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15411-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="15411-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15411-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15411-132">Request</span></span>

<span data-ttu-id="15411-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15411-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="15411-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="15411-134">Response</span></span>

<span data-ttu-id="15411-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15411-135">The following is an example of the response.</span></span>

> <span data-ttu-id="15411-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15411-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


