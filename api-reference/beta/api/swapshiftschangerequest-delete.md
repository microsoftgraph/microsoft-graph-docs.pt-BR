---
title: Excluir swapShiftsChangeRequest
description: Excluir um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 843226c6cd1109a87919790a004ad52b0351b753
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895540"
---
# <a name="delete-swapshiftschangerequest"></a><span data-ttu-id="484dc-103">Excluir swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="484dc-103">Delete swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="484dc-104">Excluir um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="484dc-104">Delete a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="484dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="484dc-105">Permissions</span></span>

<span data-ttu-id="484dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="484dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="484dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="484dc-108">Permission type</span></span>                        | <span data-ttu-id="484dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="484dc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="484dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="484dc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="484dc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="484dc-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="484dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="484dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="484dc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="484dc-113">Not supported.</span></span> |
| <span data-ttu-id="484dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="484dc-114">Application</span></span>                            | <span data-ttu-id="484dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="484dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="484dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="484dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="484dc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="484dc-117">Request headers</span></span>

| <span data-ttu-id="484dc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="484dc-118">Name</span></span>          | <span data-ttu-id="484dc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="484dc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="484dc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="484dc-120">Authorization</span></span> | <span data-ttu-id="484dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="484dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="484dc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="484dc-123">Request body</span></span>

<span data-ttu-id="484dc-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="484dc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="484dc-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="484dc-125">Response</span></span>

<span data-ttu-id="484dc-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="484dc-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="484dc-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="484dc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="484dc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="484dc-129">Request</span></span>

<span data-ttu-id="484dc-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="484dc-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_swapshiftschangerequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="484dc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="484dc-131">Response</span></span>

<span data-ttu-id="484dc-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="484dc-132">The following is an example of the response.</span></span>

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
  "description": "Delete swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
