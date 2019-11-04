---
title: Excluir email
description: Exclua um objeto de email de um perfil de usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d9b6f87f181b0b5258579b4a3c8603a0b84849f5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938447"
---
# <a name="delete-itememail"></a><span data-ttu-id="be3b3-103">Excluir email</span><span class="sxs-lookup"><span data-stu-id="be3b3-103">Delete itemEmail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be3b3-104">Excluir um objeto de [email](../resources/itememail.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="be3b3-104">Delete an [itemEmail](../resources/itememail.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be3b3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="be3b3-105">Permissions</span></span>

<span data-ttu-id="be3b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be3b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be3b3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be3b3-108">Permission type</span></span>                        | <span data-ttu-id="be3b3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be3b3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be3b3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be3b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="be3b3-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="be3b3-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="be3b3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be3b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be3b3-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="be3b3-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="be3b3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be3b3-114">Application</span></span>                            | <span data-ttu-id="be3b3-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be3b3-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="be3b3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be3b3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/emails/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="be3b3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be3b3-117">Request headers</span></span>

| <span data-ttu-id="be3b3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="be3b3-118">Name</span></span>           |<span data-ttu-id="be3b3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="be3b3-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="be3b3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="be3b3-120">Authorization</span></span>  | <span data-ttu-id="be3b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be3b3-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="be3b3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be3b3-123">Request body</span></span>

<span data-ttu-id="be3b3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be3b3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be3b3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="be3b3-125">Response</span></span>

<span data-ttu-id="be3b3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be3b3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be3b3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be3b3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be3b3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be3b3-129">Request</span></span>

<span data-ttu-id="be3b3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be3b3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_itememail"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/emails/{id}
```

### <a name="response"></a><span data-ttu-id="be3b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="be3b3-131">Response</span></span>

<span data-ttu-id="be3b3-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be3b3-132">The following is an example of the response.</span></span>

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
  "description": "Delete itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
