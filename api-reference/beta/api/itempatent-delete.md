---
title: Excluir a ispatente
description: Exclui um objeto ispatente.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a5d08e8a8478323f2563036a563eddee75a94a13
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809590"
---
# <a name="delete-itempatent"></a><span data-ttu-id="23f2a-103">Excluir a ispatente</span><span class="sxs-lookup"><span data-stu-id="23f2a-103">Delete itemPatent</span></span>

<span data-ttu-id="23f2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23f2a-105">Exclui um objeto [ispatente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="23f2a-105">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23f2a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23f2a-106">Permissions</span></span>

<span data-ttu-id="23f2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23f2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23f2a-109">Permission type</span></span>                        | <span data-ttu-id="23f2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23f2a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="23f2a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23f2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23f2a-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="23f2a-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="23f2a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23f2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f2a-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="23f2a-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="23f2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23f2a-115">Application</span></span>                            | <span data-ttu-id="23f2a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f2a-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="23f2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23f2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/patents/{id}
DELETE /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="23f2a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23f2a-118">Request headers</span></span>
|<span data-ttu-id="23f2a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="23f2a-119">Name</span></span>|<span data-ttu-id="23f2a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f2a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23f2a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="23f2a-121">Authorization</span></span>|<span data-ttu-id="23f2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23f2a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23f2a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23f2a-124">Request body</span></span>
<span data-ttu-id="23f2a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23f2a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f2a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f2a-126">Response</span></span>

<span data-ttu-id="23f2a-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23f2a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="23f2a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23f2a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23f2a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23f2a-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="23f2a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f2a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itempatent"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="23f2a-131">C#</span><span class="sxs-lookup"><span data-stu-id="23f2a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23f2a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23f2a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23f2a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23f2a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="23f2a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f2a-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
