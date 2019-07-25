---
title: Excluir trustFrameworkPolicy
description: Esta operação exclui um objeto trustFrameworkPolicy existente de um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1d96ff0f8be03a9e32998e47307a7377ffd217e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867926"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="744c0-103">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="744c0-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="744c0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="744c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="744c0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="744c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="744c0-106">Excluir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)existente.</span><span class="sxs-lookup"><span data-stu-id="744c0-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="744c0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="744c0-107">Permissions</span></span>

<span data-ttu-id="744c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="744c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="744c0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="744c0-110">Permission type</span></span>      | <span data-ttu-id="744c0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="744c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="744c0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="744c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="744c0-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="744c0-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="744c0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="744c0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="744c0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="744c0-115">Not supported.</span></span>|
|<span data-ttu-id="744c0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="744c0-116">Application</span></span>|<span data-ttu-id="744c0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="744c0-117">Not supported.</span></span>|

<span data-ttu-id="744c0-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="744c0-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="744c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="744c0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="744c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="744c0-120">Request headers</span></span>

|<span data-ttu-id="744c0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="744c0-121">Name</span></span>|<span data-ttu-id="744c0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="744c0-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="744c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="744c0-123">Authorization</span></span>|<span data-ttu-id="744c0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="744c0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="744c0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="744c0-126">Request body</span></span>

<span data-ttu-id="744c0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="744c0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="744c0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="744c0-128">Response</span></span>

<span data-ttu-id="744c0-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="744c0-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="744c0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="744c0-130">Example</span></span>

<span data-ttu-id="744c0-131">O exemplo a seguir exclui um **trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="744c0-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="744c0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="744c0-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="744c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="744c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="744c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="744c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="744c0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="744c0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="744c0-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="744c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="744c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="744c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="744c0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="744c0-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
