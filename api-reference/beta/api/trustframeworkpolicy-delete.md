---
title: Excluir trustFrameworkPolicy
description: Esta operação exclui um objeto trustFrameworkPolicy existente de um locatário do Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d3d790126acab48b716694e281b94afa8228b9b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219001"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="5f426-103">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="5f426-103">Delete trustFrameworkPolicy</span></span>

<span data-ttu-id="5f426-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f426-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f426-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f426-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f426-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f426-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f426-107">Excluir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)existente.</span><span class="sxs-lookup"><span data-stu-id="5f426-107">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f426-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f426-108">Permissions</span></span>

<span data-ttu-id="5f426-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f426-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="5f426-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f426-111">Permission type</span></span>      | <span data-ttu-id="5f426-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f426-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f426-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f426-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f426-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="5f426-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="5f426-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f426-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5f426-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f426-116">Not supported.</span></span>|
|<span data-ttu-id="5f426-117">Application</span><span class="sxs-lookup"><span data-stu-id="5f426-117">Application</span></span>|<span data-ttu-id="5f426-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="5f426-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="5f426-119">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="5f426-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f426-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f426-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5f426-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f426-121">Request headers</span></span>

|<span data-ttu-id="5f426-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5f426-122">Name</span></span>|<span data-ttu-id="5f426-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f426-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5f426-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f426-124">Authorization</span></span>|<span data-ttu-id="5f426-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f426-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f426-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f426-127">Request body</span></span>

<span data-ttu-id="5f426-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f426-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f426-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f426-129">Response</span></span>

<span data-ttu-id="5f426-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5f426-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f426-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f426-131">Example</span></span>

<span data-ttu-id="5f426-132">O exemplo a seguir exclui um **trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="5f426-132">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="5f426-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f426-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5f426-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f426-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="c"></a>[<span data-ttu-id="5f426-135">C#</span><span class="sxs-lookup"><span data-stu-id="5f426-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f426-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f426-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f426-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f426-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5f426-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f426-138">Response</span></span>

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
