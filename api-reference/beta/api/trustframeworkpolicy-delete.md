---
title: Excluir trustFrameworkPolicy
description: Essa operação exclui um objeto trustFrameworkPolicy existente de um locatário do Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0ebca87f50af1d4db6c4b6053bcabcaf9aa672d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444949"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="a4129-103">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="a4129-103">Delete trustFrameworkPolicy</span></span>

<span data-ttu-id="a4129-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4129-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4129-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4129-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4129-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4129-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4129-107">Excluir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)existente.</span><span class="sxs-lookup"><span data-stu-id="a4129-107">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4129-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4129-108">Permissions</span></span>

<span data-ttu-id="a4129-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4129-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="a4129-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4129-111">Permission type</span></span>      | <span data-ttu-id="a4129-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4129-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4129-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4129-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4129-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="a4129-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="a4129-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4129-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a4129-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4129-116">Not supported.</span></span>|
|<span data-ttu-id="a4129-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4129-117">Application</span></span>|<span data-ttu-id="a4129-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="a4129-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="a4129-119">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="a4129-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="a4129-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4129-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a4129-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4129-121">Request headers</span></span>

|<span data-ttu-id="a4129-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a4129-122">Name</span></span>|<span data-ttu-id="a4129-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4129-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a4129-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4129-124">Authorization</span></span>|<span data-ttu-id="a4129-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4129-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4129-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4129-127">Request body</span></span>

<span data-ttu-id="a4129-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4129-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4129-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4129-129">Response</span></span>

<span data-ttu-id="a4129-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4129-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4129-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4129-131">Example</span></span>

<span data-ttu-id="a4129-132">O exemplo a seguir exclui **um trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="a4129-132">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="a4129-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4129-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4129-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4129-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="c"></a>[<span data-ttu-id="a4129-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4129-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4129-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4129-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4129-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4129-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4129-138">Java</span><span class="sxs-lookup"><span data-stu-id="a4129-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4129-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4129-139">Response</span></span>

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


