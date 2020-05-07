---
title: Excluir openShift
description: Excluir um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bfd5af23293b82dbac18448ef7948057eb76db08
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155100"
---
# <a name="delete-openshift"></a><span data-ttu-id="90ca0-103">Excluir openShift</span><span class="sxs-lookup"><span data-stu-id="90ca0-103">Delete openShift</span></span>

<span data-ttu-id="90ca0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ca0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90ca0-105">Excluir um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="90ca0-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90ca0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90ca0-106">Permissions</span></span>

<span data-ttu-id="90ca0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90ca0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ca0-109">Permission type</span></span>                        | <span data-ttu-id="90ca0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90ca0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90ca0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ca0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90ca0-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="90ca0-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="90ca0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ca0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90ca0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ca0-114">Not supported.</span></span> |
| <span data-ttu-id="90ca0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90ca0-115">Application</span></span>                            | <span data-ttu-id="90ca0-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ca0-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="90ca0-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="90ca0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="90ca0-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="90ca0-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="90ca0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ca0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="90ca0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca0-120">Request headers</span></span>

| <span data-ttu-id="90ca0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="90ca0-121">Name</span></span>          | <span data-ttu-id="90ca0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ca0-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="90ca0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90ca0-123">Authorization</span></span> | <span data-ttu-id="90ca0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ca0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90ca0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca0-126">Request body</span></span>

<span data-ttu-id="90ca0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90ca0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ca0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca0-128">Response</span></span>

<span data-ttu-id="90ca0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca0-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90ca0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90ca0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90ca0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca0-132">Request</span></span>

<span data-ttu-id="90ca0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ca0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90ca0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="90ca0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
---


### <a name="response"></a><span data-ttu-id="90ca0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca0-135">Response</span></span>

<span data-ttu-id="90ca0-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca0-136">The following is an example of the response.</span></span>

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
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
