---
title: Excluir personAward
description: Exclui um objeto personAward.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 83f1c3ee61d20edd25af9b66e40b91b62551efde
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576024"
---
# <a name="delete-personaward"></a><span data-ttu-id="49b45-103">Excluir personAward</span><span class="sxs-lookup"><span data-stu-id="49b45-103">Delete personAward</span></span>

<span data-ttu-id="49b45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49b45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49b45-105">Exclui um [objeto personAward](../resources/personaward.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="49b45-105">Deletes a [personAward](../resources/personaward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49b45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49b45-106">Permissions</span></span>

<span data-ttu-id="49b45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49b45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49b45-109">Permission type</span></span>                        | <span data-ttu-id="49b45-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49b45-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="49b45-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49b45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49b45-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b45-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="49b45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49b45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49b45-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b45-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="49b45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49b45-115">Application</span></span>                            | <span data-ttu-id="49b45-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b45-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="49b45-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49b45-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/awards/{id}
DELETE /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="49b45-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49b45-118">Request headers</span></span>
|<span data-ttu-id="49b45-119">Nome</span><span class="sxs-lookup"><span data-stu-id="49b45-119">Name</span></span>|<span data-ttu-id="49b45-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b45-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49b45-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49b45-121">Authorization</span></span>|<span data-ttu-id="49b45-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49b45-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49b45-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49b45-124">Request body</span></span>
<span data-ttu-id="49b45-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49b45-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49b45-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b45-126">Response</span></span>

<span data-ttu-id="49b45-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49b45-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="49b45-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="49b45-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49b45-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49b45-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="49b45-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="49b45-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personaward"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/awards/{personAwardId}
```
# <a name="c"></a>[<span data-ttu-id="49b45-131">C#</span><span class="sxs-lookup"><span data-stu-id="49b45-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49b45-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49b45-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49b45-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49b45-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="49b45-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b45-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


