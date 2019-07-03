---
title: Excluir identityProvider
description: Excluir o identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: 74acf6b790ca9039944bc2d9bc687b74fced1d1b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442577"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="e7400-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="e7400-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7400-104">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="e7400-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7400-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7400-105">Permissions</span></span>

<span data-ttu-id="e7400-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7400-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7400-108">Permission type</span></span>      | <span data-ttu-id="e7400-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7400-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7400-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7400-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e7400-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7400-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e7400-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7400-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e7400-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7400-113">Not supported.</span></span>|
|<span data-ttu-id="e7400-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7400-114">Application</span></span>|<span data-ttu-id="e7400-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7400-115">Not supported.</span></span>|

<span data-ttu-id="e7400-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="e7400-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7400-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7400-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7400-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7400-118">Request headers</span></span>

|<span data-ttu-id="e7400-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e7400-119">Name</span></span>|<span data-ttu-id="e7400-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7400-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e7400-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7400-121">Authorization</span></span>|<span data-ttu-id="e7400-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7400-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7400-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7400-124">Request body</span></span>

<span data-ttu-id="e7400-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7400-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7400-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7400-126">Response</span></span>

<span data-ttu-id="e7400-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7400-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7400-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7400-128">Example</span></span>

<span data-ttu-id="e7400-129">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e7400-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e7400-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7400-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7400-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7400-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7400-132">C#</span><span class="sxs-lookup"><span data-stu-id="e7400-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7400-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7400-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7400-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e7400-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7400-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7400-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
