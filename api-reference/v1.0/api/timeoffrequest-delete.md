---
title: Excluir timeOffRequest
description: Excluir um objeto timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e75bbd546189b5f409d274f5b858f8ce1757019
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154294"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="df31f-103">Excluir timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="df31f-103">Delete timeOffRequest</span></span>

<span data-ttu-id="df31f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df31f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df31f-105">Excluir um objeto [timeOffRequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="df31f-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df31f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df31f-106">Permissions</span></span>

<span data-ttu-id="df31f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df31f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df31f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df31f-109">Permission type</span></span>                        | <span data-ttu-id="df31f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df31f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="df31f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df31f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df31f-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="df31f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df31f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df31f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df31f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df31f-114">Not supported.</span></span>    |
|<span data-ttu-id="df31f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df31f-115">Application</span></span> | <span data-ttu-id="df31f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df31f-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="df31f-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="df31f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="df31f-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="df31f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="df31f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df31f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="df31f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df31f-120">Request headers</span></span>

| <span data-ttu-id="df31f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="df31f-121">Name</span></span>          | <span data-ttu-id="df31f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="df31f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="df31f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df31f-123">Authorization</span></span> | <span data-ttu-id="df31f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df31f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df31f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df31f-126">Request body</span></span>

<span data-ttu-id="df31f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df31f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df31f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df31f-128">Response</span></span>

<span data-ttu-id="df31f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df31f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df31f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df31f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df31f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df31f-132">Request</span></span>

<span data-ttu-id="df31f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df31f-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
---


### <a name="response"></a><span data-ttu-id="df31f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df31f-134">Response</span></span>

<span data-ttu-id="df31f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df31f-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
