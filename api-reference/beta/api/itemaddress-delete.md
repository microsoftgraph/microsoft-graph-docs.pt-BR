---
title: Excluir endereço
description: Exclui um objeto myAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 00f531adb39ef55bc3ae48155a3de13434723cb9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812889"
---
# <a name="delete-itemaddress"></a><span data-ttu-id="a2096-103">Excluir endereço</span><span class="sxs-lookup"><span data-stu-id="a2096-103">Delete itemAddress</span></span>
<span data-ttu-id="a2096-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2096-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2096-105">Exclui um objeto [myAddress](../resources/itemaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="a2096-105">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2096-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2096-106">Permissions</span></span>

<span data-ttu-id="a2096-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2096-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2096-109">Permission type</span></span>                        | <span data-ttu-id="a2096-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2096-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a2096-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2096-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2096-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a2096-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a2096-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2096-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2096-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a2096-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a2096-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2096-115">Application</span></span>                            | <span data-ttu-id="a2096-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2096-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="a2096-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2096-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/addresses/{id}
DELETE /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a2096-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2096-118">Request headers</span></span>
|<span data-ttu-id="a2096-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a2096-119">Name</span></span>|<span data-ttu-id="a2096-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2096-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a2096-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2096-121">Authorization</span></span>|<span data-ttu-id="a2096-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2096-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2096-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2096-124">Request body</span></span>
<span data-ttu-id="a2096-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2096-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2096-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2096-126">Response</span></span>

<span data-ttu-id="a2096-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a2096-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a2096-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a2096-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2096-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2096-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="a2096-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2096-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemaddress"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="a2096-131">C#</span><span class="sxs-lookup"><span data-stu-id="a2096-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2096-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2096-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2096-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2096-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a2096-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2096-134">Response</span></span>
<span data-ttu-id="a2096-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a2096-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
