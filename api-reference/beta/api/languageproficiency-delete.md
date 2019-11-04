---
title: Excluir languageProficiency
description: Excluir um objeto languageProficiency do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fac3c223e51d77ee9369d505dc382eb530240b7a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938426"
---
# <a name="delete-languageproficiency"></a><span data-ttu-id="fa028-103">Excluir languageProficiency</span><span class="sxs-lookup"><span data-stu-id="fa028-103">Delete languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa028-104">Excluir um objeto [languageProficiency](../resources/languageproficiency.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fa028-104">Delete a [languageProficiency](../resources/languageproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa028-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa028-105">Permissions</span></span>

<span data-ttu-id="fa028-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa028-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa028-108">Permission type</span></span>                        | <span data-ttu-id="fa028-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa028-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa028-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa028-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa028-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa028-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fa028-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa028-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa028-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa028-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fa028-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa028-114">Application</span></span>                            | <span data-ttu-id="fa028-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa028-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="fa028-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa028-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa028-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa028-117">Request headers</span></span>

| <span data-ttu-id="fa028-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fa028-118">Name</span></span>           |<span data-ttu-id="fa028-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa028-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="fa028-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa028-120">Authorization</span></span>  | <span data-ttu-id="fa028-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa028-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="fa028-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa028-123">Content-Type</span></span>   | <span data-ttu-id="fa028-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa028-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa028-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa028-126">Request body</span></span>

<span data-ttu-id="fa028-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa028-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa028-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa028-128">Response</span></span>

<span data-ttu-id="fa028-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa028-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa028-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa028-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa028-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa028-132">Request</span></span>

<span data-ttu-id="fa028-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa028-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_languageproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/languages/{id}
```

### <a name="response"></a><span data-ttu-id="fa028-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa028-134">Response</span></span>

<span data-ttu-id="fa028-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa028-135">The following is an example of the response.</span></span>

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
  "description": "Delete languageProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->