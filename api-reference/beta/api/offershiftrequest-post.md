---
title: Criar offerShiftRequest
description: Criar uma instância de um offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3c7eeb1fbe68e41465b5a55150e72c694dad059d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952122"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="dcd5e-103">Criar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="dcd5e-103">Create offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcd5e-104">Criar uma instância de um [offerShiftRequest](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="dcd5e-104">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd5e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcd5e-105">Permissions</span></span>

<span data-ttu-id="dcd5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcd5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcd5e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcd5e-108">Permission type</span></span>                        | <span data-ttu-id="dcd5e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcd5e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcd5e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcd5e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcd5e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcd5e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="dcd5e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcd5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd5e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-113">Not supported.</span></span> |
| <span data-ttu-id="dcd5e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcd5e-114">Application</span></span>                            | <span data-ttu-id="dcd5e-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="dcd5e-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="dcd5e-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="dcd5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcd5e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcd5e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dcd5e-118">Optional query parameters</span></span>

<span data-ttu-id="dcd5e-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dcd5e-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dcd5e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcd5e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd5e-121">Request headers</span></span>

| <span data-ttu-id="dcd5e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dcd5e-122">Name</span></span>      |<span data-ttu-id="dcd5e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcd5e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcd5e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcd5e-124">Authorization</span></span> | <span data-ttu-id="dcd5e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcd5e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd5e-127">Request body</span></span>
<span data-ttu-id="dcd5e-128">Forneça o novo objeto [offershiftrequest](../resources/offershiftrequest.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-128">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcd5e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd5e-129">Response</span></span>

<span data-ttu-id="dcd5e-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [offerShiftRequest](../resources/offershiftrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-130">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcd5e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcd5e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcd5e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd5e-132">Request</span></span>

<span data-ttu-id="dcd5e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```

### <a name="response"></a><span data-ttu-id="dcd5e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd5e-134">Response</span></span>

<span data-ttu-id="dcd5e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-135">The following is an example of the response.</span></span>

> <span data-ttu-id="dcd5e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcd5e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.etag": "\"4000ee23-0000-0700-0000-5d1415f60000\"",
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "createdDateTime": "2019-09-27T01:01:04.566Z",
  "lastModifiedDateTime": "2019-09-28T01:03:48.874Z",
  "assignedTo": "recipient",
  "state": "pending",
  "senderDateTime": "2019-09-27T01:01:04.566",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "senderUserId": "a4704dd0-3f4c-4f2c-9bb5-8cc575703f30",
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "managerUserId": null,
  "recipientActionDateTime": null,
  "recipientActionMessage": null,
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
      "displayName": "Employee 1"
    }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
