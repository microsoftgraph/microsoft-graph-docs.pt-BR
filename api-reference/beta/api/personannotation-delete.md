---
title: Excluir personAnnotation
description: Exclui um objeto personAnnotation.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5f9bf692b7e386ca47042ee763fa0d9e57f86fea
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809582"
---
# <a name="delete-personannotation"></a><span data-ttu-id="dbb02-103">Excluir personAnnotation</span><span class="sxs-lookup"><span data-stu-id="dbb02-103">Delete personAnnotation</span></span>
<span data-ttu-id="dbb02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbb02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbb02-105">Exclui um objeto [personAnnotation](../resources/personannotation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dbb02-105">Deletes a [personAnnotation](../resources/personannotation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dbb02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbb02-106">Permissions</span></span>

<span data-ttu-id="dbb02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbb02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbb02-109">Permission type</span></span>                        | <span data-ttu-id="dbb02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbb02-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="dbb02-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbb02-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbb02-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbb02-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="dbb02-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbb02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbb02-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbb02-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="dbb02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbb02-115">Application</span></span>                            | <span data-ttu-id="dbb02-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbb02-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="dbb02-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbb02-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/notes/{id}
DELETE /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dbb02-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb02-118">Request headers</span></span>
|<span data-ttu-id="dbb02-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dbb02-119">Name</span></span>|<span data-ttu-id="dbb02-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb02-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dbb02-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbb02-121">Authorization</span></span>|<span data-ttu-id="dbb02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb02-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbb02-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb02-124">Request body</span></span>
<span data-ttu-id="dbb02-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbb02-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbb02-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb02-126">Response</span></span>

<span data-ttu-id="dbb02-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dbb02-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dbb02-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dbb02-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dbb02-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb02-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="dbb02-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbb02-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personannotation"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/notes/{id}
```
# <a name="c"></a>[<span data-ttu-id="dbb02-131">C#</span><span class="sxs-lookup"><span data-stu-id="dbb02-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbb02-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbb02-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbb02-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbb02-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dbb02-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb02-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
