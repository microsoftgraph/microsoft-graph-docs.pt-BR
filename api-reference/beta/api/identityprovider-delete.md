---
title: Excluir identityProvider
description: Excluir o identityProvider existente.
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67559db80d23784f3641b953c950956f1afabf4c
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199575"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="4252e-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="4252e-103">Delete identityProvider</span></span>

<span data-ttu-id="4252e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4252e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4252e-105">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="4252e-105">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4252e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4252e-106">Permissions</span></span>

<span data-ttu-id="4252e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4252e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4252e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4252e-109">Permission type</span></span>      | <span data-ttu-id="4252e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4252e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4252e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4252e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4252e-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4252e-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="4252e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4252e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4252e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4252e-114">Not supported.</span></span>|
|<span data-ttu-id="4252e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4252e-115">Application</span></span>|<span data-ttu-id="4252e-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4252e-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="4252e-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="4252e-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="4252e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4252e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4252e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4252e-119">Request headers</span></span>

|<span data-ttu-id="4252e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4252e-120">Name</span></span>|<span data-ttu-id="4252e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4252e-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4252e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4252e-122">Authorization</span></span>|<span data-ttu-id="4252e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4252e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4252e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4252e-125">Request body</span></span>

<span data-ttu-id="4252e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4252e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4252e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4252e-127">Response</span></span>

<span data-ttu-id="4252e-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4252e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4252e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4252e-129">Example</span></span>

<span data-ttu-id="4252e-130">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="4252e-130">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="4252e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4252e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4252e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4252e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="4252e-133">C#</span><span class="sxs-lookup"><span data-stu-id="4252e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4252e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4252e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4252e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4252e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4252e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4252e-136">Response</span></span>

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
