---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c997fb52a05a0debb30a89b99736a2ede8abcd19
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154932"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="f7768-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="f7768-103">Get offerShiftRequest</span></span>

<span data-ttu-id="f7768-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7768-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7768-105">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f7768-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7768-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7768-106">Permissions</span></span>

<span data-ttu-id="f7768-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7768-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7768-109">Permission type</span></span>                        | <span data-ttu-id="f7768-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7768-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7768-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7768-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7768-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7768-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f7768-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7768-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7768-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7768-114">Not supported.</span></span> |
| <span data-ttu-id="f7768-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7768-115">Application</span></span>                            | <span data-ttu-id="f7768-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7768-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="f7768-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="f7768-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f7768-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="f7768-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f7768-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7768-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7768-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7768-120">Optional query parameters</span></span>

<span data-ttu-id="f7768-121">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7768-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7768-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7768-122">Request headers</span></span>

| <span data-ttu-id="f7768-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f7768-123">Name</span></span>      |<span data-ttu-id="f7768-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7768-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7768-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7768-125">Authorization</span></span> | <span data-ttu-id="f7768-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7768-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7768-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7768-128">Request body</span></span>

<span data-ttu-id="f7768-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7768-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7768-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7768-130">Response</span></span>

<span data-ttu-id="f7768-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7768-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7768-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7768-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7768-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7768-133">Request</span></span>

<span data-ttu-id="f7768-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7768-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
---


### <a name="response"></a><span data-ttu-id="f7768-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7768-135">Response</span></span>

<span data-ttu-id="f7768-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7768-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f7768-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7768-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
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
