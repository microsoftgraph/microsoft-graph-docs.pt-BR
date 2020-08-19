---
title: Excluir personCertification
description: Exclui um objeto personCertification.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: da30a5b3646dc5b72ccc726740d6ad7f076490d1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812893"
---
# <a name="delete-personcertification"></a><span data-ttu-id="eb8c7-103">Excluir personCertification</span><span class="sxs-lookup"><span data-stu-id="eb8c7-103">Delete personCertification</span></span>
<span data-ttu-id="eb8c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb8c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb8c7-105">Exclui um objeto [personCertification](../resources/personcertification.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-105">Deletes a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb8c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb8c7-106">Permissions</span></span>

<span data-ttu-id="eb8c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb8c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb8c7-109">Permission type</span></span>                        | <span data-ttu-id="eb8c7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb8c7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="eb8c7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb8c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb8c7-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb8c7-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="eb8c7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb8c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb8c7-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb8c7-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="eb8c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb8c7-115">Application</span></span>                            | <span data-ttu-id="eb8c7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb8c7-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="eb8c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb8c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/certifications/{id}
DELETE /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eb8c7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb8c7-118">Request headers</span></span>
|<span data-ttu-id="eb8c7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eb8c7-119">Name</span></span>|<span data-ttu-id="eb8c7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb8c7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eb8c7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb8c7-121">Authorization</span></span>|<span data-ttu-id="eb8c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb8c7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb8c7-124">Request body</span></span>
<span data-ttu-id="eb8c7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb8c7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb8c7-126">Response</span></span>

<span data-ttu-id="eb8c7-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eb8c7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb8c7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb8c7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb8c7-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="eb8c7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb8c7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personCertification"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="eb8c7-131">C#</span><span class="sxs-lookup"><span data-stu-id="eb8c7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb8c7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb8c7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb8c7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb8c7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="eb8c7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb8c7-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
