---
title: Excluir a multipúblico
description: Exclui um objeto dopublication.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a43629bdbd20859a3c311f8efadf264a9f84bab2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820103"
---
# <a name="delete-itempublication"></a><span data-ttu-id="11e9c-103">Excluir a multipúblico</span><span class="sxs-lookup"><span data-stu-id="11e9c-103">Delete itemPublication</span></span>

<span data-ttu-id="11e9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11e9c-105">Exclui um objeto [Dopublication](../resources/itempublication.md) .</span><span class="sxs-lookup"><span data-stu-id="11e9c-105">Deletes an [itemPublication](../resources/itempublication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11e9c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11e9c-106">Permissions</span></span>

<span data-ttu-id="11e9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11e9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11e9c-109">Permission type</span></span>                        | <span data-ttu-id="11e9c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11e9c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="11e9c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11e9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11e9c-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11e9c-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="11e9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11e9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11e9c-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11e9c-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="11e9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11e9c-115">Application</span></span>                            | <span data-ttu-id="11e9c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11e9c-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="11e9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11e9c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/publications/{id}
DELETE /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11e9c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11e9c-118">Request headers</span></span>
|<span data-ttu-id="11e9c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="11e9c-119">Name</span></span>|<span data-ttu-id="11e9c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e9c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="11e9c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11e9c-121">Authorization</span></span>|<span data-ttu-id="11e9c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e9c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11e9c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11e9c-124">Request body</span></span>
<span data-ttu-id="11e9c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11e9c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11e9c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e9c-126">Response</span></span>

<span data-ttu-id="11e9c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="11e9c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="11e9c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11e9c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11e9c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e9c-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="11e9c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e9c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemPublication"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/publications/{id}
```
# <a name="c"></a>[<span data-ttu-id="11e9c-131">C#</span><span class="sxs-lookup"><span data-stu-id="11e9c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itempublication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e9c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e9c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itempublication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e9c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itempublication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="11e9c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e9c-134">Response</span></span>
<span data-ttu-id="11e9c-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11e9c-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
