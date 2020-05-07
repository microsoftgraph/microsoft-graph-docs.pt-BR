---
title: Excluir Shift
description: Excluir uma mudança do cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f3e08c9a8624787c0ce961dd4558bd3b21453667
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154112"
---
# <a name="delete-shift"></a><span data-ttu-id="b5966-103">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="b5966-103">Delete shift</span></span>

<span data-ttu-id="b5966-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5966-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5966-105">Excluir uma [mudança](../resources/shift.md) do cronograma.</span><span class="sxs-lookup"><span data-stu-id="b5966-105">Delete a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5966-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5966-106">Permissions</span></span>

<span data-ttu-id="b5966-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5966-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5966-109">Permission type</span></span>      | <span data-ttu-id="b5966-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5966-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5966-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5966-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5966-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b5966-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5966-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5966-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5966-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5966-114">Not supported.</span></span>    |
|<span data-ttu-id="b5966-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5966-115">Application</span></span> | <span data-ttu-id="b5966-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b5966-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="b5966-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="b5966-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b5966-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="b5966-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b5966-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5966-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b5966-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5966-120">Request headers</span></span>

| <span data-ttu-id="b5966-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5966-121">Header</span></span>       | <span data-ttu-id="b5966-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5966-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5966-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5966-123">Authorization</span></span>  | <span data-ttu-id="b5966-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5966-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5966-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5966-126">Request body</span></span>
<span data-ttu-id="b5966-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5966-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5966-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5966-128">Response</span></span>

<span data-ttu-id="b5966-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5966-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5966-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5966-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b5966-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5966-132">Request</span></span>

<span data-ttu-id="b5966-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5966-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
---


#### <a name="response"></a><span data-ttu-id="b5966-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5966-134">Response</span></span>

<span data-ttu-id="b5966-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5966-135">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
