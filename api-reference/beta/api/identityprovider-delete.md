---
title: Excluir identityProvider
description: Exclua um identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2924b7b4174f1457d212f4905dd829a23d636296
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508854"
---
# <a name="delete-identityprovider-deprecated"></a><span data-ttu-id="92f28-103">Excluir identityProvider (preterido)</span><span class="sxs-lookup"><span data-stu-id="92f28-103">Delete identityProvider (deprecated)</span></span>
<span data-ttu-id="92f28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92f28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="92f28-105">Excluir um [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="92f28-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92f28-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="92f28-106">Permissions</span></span>

<span data-ttu-id="92f28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92f28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92f28-109">Permission type</span></span>      | <span data-ttu-id="92f28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92f28-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92f28-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92f28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92f28-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f28-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="92f28-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92f28-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="92f28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92f28-114">Not supported.</span></span>|
|<span data-ttu-id="92f28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92f28-115">Application</span></span>|<span data-ttu-id="92f28-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f28-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="92f28-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="92f28-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="92f28-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="92f28-118">Global Administrator</span></span>
* <span data-ttu-id="92f28-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="92f28-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="92f28-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92f28-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92f28-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92f28-121">Request headers</span></span>

|<span data-ttu-id="92f28-122">Nome</span><span class="sxs-lookup"><span data-stu-id="92f28-122">Name</span></span>|<span data-ttu-id="92f28-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="92f28-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="92f28-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="92f28-124">Authorization</span></span>|<span data-ttu-id="92f28-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92f28-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92f28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92f28-127">Request body</span></span>

<span data-ttu-id="92f28-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92f28-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92f28-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92f28-129">Response</span></span>

<span data-ttu-id="92f28-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92f28-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92f28-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92f28-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="92f28-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92f28-132">Request</span></span>

<span data-ttu-id="92f28-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92f28-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```

# <a name="java"></a>[<span data-ttu-id="92f28-134">Java</span><span class="sxs-lookup"><span data-stu-id="92f28-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="92f28-135">C#</span><span class="sxs-lookup"><span data-stu-id="92f28-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92f28-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92f28-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92f28-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92f28-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="92f28-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="92f28-138">Response</span></span>

<span data-ttu-id="92f28-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92f28-139">The following is an example of the response.</span></span>

<span data-ttu-id="92f28-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="92f28-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
