---
title: Obter timeOffRequest
description: Recupere as propriedades e os relacionamentos de um objeto timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7b1f20f71db24e39b5e129cc958f1e0ed182a570
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154287"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="41fc4-103">Obter timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="41fc4-103">Get timeOffRequest</span></span>

<span data-ttu-id="41fc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41fc4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41fc4-105">Recupere as propriedades e os relacionamentos de um objeto [timeoffrequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="41fc4-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41fc4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41fc4-106">Permissions</span></span>

<span data-ttu-id="41fc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41fc4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41fc4-109">Permission type</span></span>                        | <span data-ttu-id="41fc4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41fc4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="41fc4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41fc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="41fc4-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="41fc4-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="41fc4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41fc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41fc4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41fc4-114">Not supported.</span></span>    |
|<span data-ttu-id="41fc4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41fc4-115">Application</span></span> | <span data-ttu-id="41fc4-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="41fc4-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="41fc4-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="41fc4-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="41fc4-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="41fc4-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="41fc4-119">atualmente somente em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="41fc4-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="41fc4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41fc4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41fc4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41fc4-121">Optional query parameters</span></span>

<span data-ttu-id="41fc4-122">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc4-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41fc4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc4-123">Request headers</span></span>

| <span data-ttu-id="41fc4-124">Nome</span><span class="sxs-lookup"><span data-stu-id="41fc4-124">Name</span></span>      |<span data-ttu-id="41fc4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="41fc4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41fc4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="41fc4-126">Authorization</span></span> | <span data-ttu-id="41fc4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41fc4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41fc4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc4-129">Request body</span></span>

<span data-ttu-id="41fc4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41fc4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41fc4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="41fc4-131">Response</span></span>

<span data-ttu-id="41fc4-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [timeOffRequest](../resources/timeoffrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc4-132">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41fc4-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41fc4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41fc4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc4-134">Request</span></span>

<span data-ttu-id="41fc4-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41fc4-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
---


### <a name="response"></a><span data-ttu-id="41fc4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="41fc4-136">Response</span></span>

<span data-ttu-id="41fc4-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc4-137">The following is an example of the response.</span></span>

> <span data-ttu-id="41fc4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41fc4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
