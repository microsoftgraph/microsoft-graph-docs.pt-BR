---
title: Excluir a ispatente
description: Exclui um objeto ispatente.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1721797203410eab2fee7ff46970e1da36d8047f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089993"
---
# <a name="delete-itempatent"></a><span data-ttu-id="9663b-103">Excluir a ispatente</span><span class="sxs-lookup"><span data-stu-id="9663b-103">Delete itemPatent</span></span>

<span data-ttu-id="9663b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9663b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9663b-105">Exclui um objeto [ispatente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="9663b-105">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9663b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9663b-106">Permissions</span></span>

<span data-ttu-id="9663b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9663b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9663b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9663b-109">Permission type</span></span>                        | <span data-ttu-id="9663b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9663b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="9663b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9663b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9663b-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9663b-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9663b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9663b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9663b-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9663b-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9663b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9663b-115">Application</span></span>                            | <span data-ttu-id="9663b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9663b-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="9663b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9663b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/patents/{id}
DELETE /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9663b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9663b-118">Request headers</span></span>
|<span data-ttu-id="9663b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9663b-119">Name</span></span>|<span data-ttu-id="9663b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9663b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9663b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9663b-121">Authorization</span></span>|<span data-ttu-id="9663b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9663b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9663b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9663b-124">Request body</span></span>
<span data-ttu-id="9663b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9663b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9663b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9663b-126">Response</span></span>

<span data-ttu-id="9663b-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9663b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9663b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9663b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9663b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9663b-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="9663b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9663b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itempatent"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="9663b-131">C#</span><span class="sxs-lookup"><span data-stu-id="9663b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9663b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9663b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9663b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9663b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9663b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9663b-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


