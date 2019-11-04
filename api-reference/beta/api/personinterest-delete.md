---
title: Excluir personInterest
description: Exclua o objeto personInterest do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ede00cecfd7ecff638a4f29ccbb42835ccd73c1c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937893"
---
# <a name="delete-personinterest"></a><span data-ttu-id="9672f-103">Excluir personInterest</span><span class="sxs-lookup"><span data-stu-id="9672f-103">Delete personInterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9672f-104">Excluir um objeto [personInterest](../resources/personinterest.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="9672f-104">Delete a [personInterest](../resources/personinterest.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9672f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9672f-105">Permissions</span></span>

<span data-ttu-id="9672f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9672f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9672f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9672f-108">Permission type</span></span>                        | <span data-ttu-id="9672f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9672f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9672f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9672f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9672f-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9672f-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9672f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9672f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9672f-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9672f-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9672f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9672f-114">Application</span></span>                            | <span data-ttu-id="9672f-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9672f-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="9672f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9672f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9672f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9672f-117">Request headers</span></span>

| <span data-ttu-id="9672f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9672f-118">Name</span></span>           |<span data-ttu-id="9672f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9672f-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="9672f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9672f-120">Authorization</span></span>  | <span data-ttu-id="9672f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9672f-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="9672f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9672f-123">Request body</span></span>

<span data-ttu-id="9672f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9672f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9672f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9672f-125">Response</span></span>

<span data-ttu-id="9672f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9672f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9672f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9672f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9672f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9672f-129">Request</span></span>

<span data-ttu-id="9672f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9672f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```

### <a name="response"></a><span data-ttu-id="9672f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9672f-131">Response</span></span>

<span data-ttu-id="9672f-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9672f-132">The following is an example of the response.</span></span>

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
  "description": "Delete personInterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
