---
title: Listar openShiftChangeRequests
description: Recupere uma lista de objetos openShiftChangeRequest em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 465ec4ecc7f86483af7b4ae61f714c1aa40d09d5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952213"
---
# <a name="list-openshiftchangerequests"></a><span data-ttu-id="0d7a6-103">Listar openShiftChangeRequests</span><span class="sxs-lookup"><span data-stu-id="0d7a6-103">List openShiftChangeRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d7a6-104">Recupere uma lista de objetos [openShiftChangeRequest](../resources/openshiftchangerequest.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-104">Retrieve a list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d7a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d7a6-105">Permissions</span></span>

<span data-ttu-id="0d7a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d7a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d7a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d7a6-108">Permission type</span></span>                        | <span data-ttu-id="0d7a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d7a6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d7a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d7a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d7a6-111">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="0d7a6-111">Group.ReadWrite.All, Group.Read.All</span></span> |
| <span data-ttu-id="0d7a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d7a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d7a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-113">Not supported.</span></span> |
| <span data-ttu-id="0d7a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d7a6-114">Application</span></span>                            | <span data-ttu-id="0d7a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d7a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7a6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d7a6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d7a6-117">Optional query parameters</span></span>

<span data-ttu-id="0d7a6-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0d7a6-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0d7a6-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d7a6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7a6-120">Request headers</span></span>

| <span data-ttu-id="0d7a6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0d7a6-121">Name</span></span>      |<span data-ttu-id="0d7a6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d7a6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d7a6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d7a6-123">Authorization</span></span> | <span data-ttu-id="0d7a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d7a6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7a6-126">Request body</span></span>

<span data-ttu-id="0d7a6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d7a6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d7a6-128">Response</span></span>

<span data-ttu-id="0d7a6-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e a lista de objetos [openShiftChangeRequest](../resources/openshiftchangerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-129">If successful, this method returns a `200 OK` response code and the list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d7a6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d7a6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d7a6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7a6-131">Request</span></span>

<span data-ttu-id="0d7a6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="0d7a6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d7a6-133">Response</span></span>

<span data-ttu-id="0d7a6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0d7a6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d7a6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
