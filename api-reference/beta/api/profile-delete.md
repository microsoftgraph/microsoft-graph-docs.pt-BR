---
title: Excluir perfil
description: Excluir perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ce087b6e03952985917c4b219ac6e49d3d90faf8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937823"
---
# <a name="delete-profile"></a><span data-ttu-id="3a72c-103">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="3a72c-103">Delete profile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a72c-104">Exclua o objeto de [perfil](../resources/profile.md) da conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3a72c-104">Delete [profile](../resources/profile.md) object from a user's account.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a72c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a72c-105">Permissions</span></span>

<span data-ttu-id="3a72c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a72c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a72c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a72c-108">Permission type</span></span>                        | <span data-ttu-id="3a72c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a72c-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="3a72c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a72c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a72c-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3a72c-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3a72c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a72c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a72c-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3a72c-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3a72c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a72c-114">Application</span></span>                            | <span data-ttu-id="3a72c-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3a72c-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="3a72c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a72c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile
```

## <a name="request-headers"></a><span data-ttu-id="3a72c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a72c-117">Request headers</span></span>

| <span data-ttu-id="3a72c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3a72c-118">Name</span></span>           |<span data-ttu-id="3a72c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a72c-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="3a72c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a72c-120">Authorization</span></span>  | <span data-ttu-id="3a72c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a72c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3a72c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a72c-123">Content-Type</span></span>   | <span data-ttu-id="3a72c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a72c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a72c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a72c-126">Request body</span></span>

<span data-ttu-id="3a72c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a72c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a72c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a72c-128">Response</span></span>

<span data-ttu-id="3a72c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a72c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a72c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a72c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a72c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a72c-132">Request</span></span>

<span data-ttu-id="3a72c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a72c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_profile"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile
```

### <a name="response"></a><span data-ttu-id="3a72c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a72c-134">Response</span></span>

<span data-ttu-id="3a72c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a72c-135">The following is an example of the response.</span></span>

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
  "description": "Delete profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->