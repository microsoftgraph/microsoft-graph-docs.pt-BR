---
title: Obter swapShiftsChangeRequest
description: Recupere as propriedades e os relacionamentos de um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5203f7902a5c25683e173c4647b7cb776655e05c
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951749"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="819e6-103">Obter swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="819e6-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="819e6-104">Recupere as propriedades e os relacionamentos de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="819e6-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="819e6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="819e6-105">Permissions</span></span>

<span data-ttu-id="819e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="819e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="819e6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="819e6-108">Permission type</span></span>                        | <span data-ttu-id="819e6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="819e6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="819e6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="819e6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="819e6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="819e6-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="819e6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="819e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="819e6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="819e6-113">Not supported.</span></span> |
| <span data-ttu-id="819e6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="819e6-114">Application</span></span> | <span data-ttu-id="819e6-115">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="819e6-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="819e6-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="819e6-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="819e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="819e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="819e6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="819e6-118">Optional query parameters</span></span>

<span data-ttu-id="819e6-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="819e6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="819e6-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="819e6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="819e6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="819e6-121">Request headers</span></span>

| <span data-ttu-id="819e6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="819e6-122">Name</span></span>      |<span data-ttu-id="819e6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="819e6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="819e6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="819e6-124">Authorization</span></span> | <span data-ttu-id="819e6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="819e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="819e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="819e6-127">Request body</span></span>

<span data-ttu-id="819e6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="819e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="819e6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="819e6-129">Response</span></span>

<span data-ttu-id="819e6-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="819e6-130">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="819e6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="819e6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="819e6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="819e6-132">Request</span></span>

<span data-ttu-id="819e6-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="819e6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```

### <a name="response"></a><span data-ttu-id="819e6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="819e6-134">Response</span></span>

<span data-ttu-id="819e6-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="819e6-135">The following is an example of the response.</span></span>

> <span data-ttu-id="819e6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="819e6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
