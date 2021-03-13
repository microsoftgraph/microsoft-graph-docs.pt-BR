---
title: Excluir personAward
description: Exclui um objeto personAward.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 011db1b2bd748018ef2b85a060297e677297823d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774128"
---
# <a name="delete-personaward"></a><span data-ttu-id="223b2-103">Excluir personAward</span><span class="sxs-lookup"><span data-stu-id="223b2-103">Delete personAward</span></span>

<span data-ttu-id="223b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="223b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="223b2-105">Exclui um [objeto personAward](../resources/personaward.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="223b2-105">Deletes a [personAward](../resources/personaward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="223b2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="223b2-106">Permissions</span></span>

<span data-ttu-id="223b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="223b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="223b2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="223b2-109">Permission type</span></span>                        | <span data-ttu-id="223b2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="223b2-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="223b2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="223b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="223b2-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="223b2-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="223b2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="223b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="223b2-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="223b2-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="223b2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="223b2-115">Application</span></span>                            | <span data-ttu-id="223b2-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="223b2-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="223b2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="223b2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/awards/{id}
DELETE /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="223b2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="223b2-118">Request headers</span></span>
|<span data-ttu-id="223b2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="223b2-119">Name</span></span>|<span data-ttu-id="223b2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="223b2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="223b2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="223b2-121">Authorization</span></span>|<span data-ttu-id="223b2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="223b2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="223b2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="223b2-124">Request body</span></span>
<span data-ttu-id="223b2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="223b2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="223b2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="223b2-126">Response</span></span>

<span data-ttu-id="223b2-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="223b2-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="223b2-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="223b2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="223b2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="223b2-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="223b2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="223b2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personaward"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/awards/{personAwardId}
```
# <a name="c"></a>[<span data-ttu-id="223b2-131">C#</span><span class="sxs-lookup"><span data-stu-id="223b2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personaward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="223b2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="223b2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personaward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="223b2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="223b2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personaward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="223b2-134">Java</span><span class="sxs-lookup"><span data-stu-id="223b2-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personaward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="223b2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="223b2-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


