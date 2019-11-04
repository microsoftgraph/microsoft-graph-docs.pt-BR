---
title: Excluir workPosition
description: Excluir um objeto workPosition do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 809552f0601e65e8478ab8e3a040821e9be09764
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938103"
---
# <a name="delete-workposition"></a><span data-ttu-id="1828b-103">Excluir workPosition</span><span class="sxs-lookup"><span data-stu-id="1828b-103">Delete workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1828b-104">Excluir um objeto [workPosition](../resources/workposition.md) específico do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1828b-104">Delete a specific [workPosition](../resources/workposition.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1828b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1828b-105">Permissions</span></span>

<span data-ttu-id="1828b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1828b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1828b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1828b-108">Permission type</span></span>                        | <span data-ttu-id="1828b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1828b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1828b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1828b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1828b-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1828b-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1828b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1828b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1828b-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1828b-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1828b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1828b-114">Application</span></span>                            | <span data-ttu-id="1828b-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1828b-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1828b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1828b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1828b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1828b-117">Request headers</span></span>

| <span data-ttu-id="1828b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1828b-118">Name</span></span>           |<span data-ttu-id="1828b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1828b-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1828b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1828b-120">Authorization</span></span>  | <span data-ttu-id="1828b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1828b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1828b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1828b-123">Content-Type</span></span>   | <span data-ttu-id="1828b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1828b-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1828b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1828b-126">Request body</span></span>

<span data-ttu-id="1828b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1828b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1828b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1828b-128">Response</span></span>

<span data-ttu-id="1828b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1828b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1828b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1828b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1828b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1828b-132">Request</span></span>

<span data-ttu-id="1828b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1828b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_workposition"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/positions/{id}
```

### <a name="response"></a><span data-ttu-id="1828b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1828b-134">Response</span></span>

<span data-ttu-id="1828b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1828b-135">The following is an example of the response.</span></span>

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
  "description": "Delete workPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->