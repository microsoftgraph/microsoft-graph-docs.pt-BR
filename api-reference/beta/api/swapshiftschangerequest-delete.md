---
title: Excluir swapShiftsChangeRequest
description: Excluir um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09e7a6eaa03525d20479731fc07d691e8f70f093
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870846"
---
# <a name="delete-swapshiftschangerequest"></a><span data-ttu-id="44d0e-103">Excluir swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="44d0e-103">Delete swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44d0e-104">Excluir um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="44d0e-104">Delete a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44d0e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="44d0e-105">Permissions</span></span>

<span data-ttu-id="44d0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44d0e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44d0e-108">Permission type</span></span>                        | <span data-ttu-id="44d0e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44d0e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44d0e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44d0e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="44d0e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d0e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="44d0e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44d0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d0e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44d0e-113">Not supported.</span></span> |
|<span data-ttu-id="44d0e-114">Application</span><span class="sxs-lookup"><span data-stu-id="44d0e-114">Application</span></span> | <span data-ttu-id="44d0e-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="44d0e-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="44d0e-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="44d0e-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="44d0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44d0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="44d0e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44d0e-118">Request headers</span></span>

| <span data-ttu-id="44d0e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="44d0e-119">Name</span></span>          | <span data-ttu-id="44d0e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="44d0e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44d0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="44d0e-121">Authorization</span></span> | <span data-ttu-id="44d0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44d0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44d0e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44d0e-124">Request body</span></span>

<span data-ttu-id="44d0e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44d0e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44d0e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="44d0e-126">Response</span></span>

<span data-ttu-id="44d0e-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44d0e-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44d0e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="44d0e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44d0e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44d0e-130">Request</span></span>

<span data-ttu-id="44d0e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44d0e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44d0e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="44d0e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_swapshiftschangerequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44d0e-133">C#</span><span class="sxs-lookup"><span data-stu-id="44d0e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44d0e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44d0e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44d0e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44d0e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="44d0e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="44d0e-136">Response</span></span>

<span data-ttu-id="44d0e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44d0e-137">The following is an example of the response.</span></span>

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
