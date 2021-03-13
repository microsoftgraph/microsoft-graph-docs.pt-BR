---
title: Excluir personCertification
description: Exclui um objeto personCertification.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6a6c1493496fdfca68c1282091ebe2092f0683be
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774072"
---
# <a name="delete-personcertification"></a><span data-ttu-id="0b09b-103">Excluir personCertification</span><span class="sxs-lookup"><span data-stu-id="0b09b-103">Delete personCertification</span></span>
<span data-ttu-id="0b09b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b09b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b09b-105">Exclui um [objeto personCertification](../resources/personcertification.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="0b09b-105">Deletes a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b09b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b09b-106">Permissions</span></span>

<span data-ttu-id="0b09b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b09b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b09b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b09b-109">Permission type</span></span>                        | <span data-ttu-id="0b09b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b09b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0b09b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b09b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b09b-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b09b-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0b09b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b09b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b09b-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b09b-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0b09b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b09b-115">Application</span></span>                            | <span data-ttu-id="0b09b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b09b-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="0b09b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b09b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/certifications/{id}
DELETE /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b09b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b09b-118">Request headers</span></span>
|<span data-ttu-id="0b09b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0b09b-119">Name</span></span>|<span data-ttu-id="0b09b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b09b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b09b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b09b-121">Authorization</span></span>|<span data-ttu-id="0b09b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b09b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b09b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b09b-124">Request body</span></span>
<span data-ttu-id="0b09b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b09b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b09b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b09b-126">Response</span></span>

<span data-ttu-id="0b09b-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b09b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0b09b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0b09b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b09b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b09b-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="0b09b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b09b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personCertification"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b09b-131">C#</span><span class="sxs-lookup"><span data-stu-id="0b09b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personcertification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b09b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b09b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personcertification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b09b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b09b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personcertification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b09b-134">Java</span><span class="sxs-lookup"><span data-stu-id="0b09b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personcertification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0b09b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b09b-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


