---
title: Excluir trustFrameworkPolicy
description: Esta operação exclui um objeto trustFrameworkPolicy existente de um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bc62bdcda19038a24441fccfe01fac9705d1344
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637434"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="0205e-103">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="0205e-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="0205e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0205e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0205e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0205e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0205e-106">Excluir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)existente.</span><span class="sxs-lookup"><span data-stu-id="0205e-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0205e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0205e-107">Permissions</span></span>

<span data-ttu-id="0205e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0205e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="0205e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0205e-110">Permission type</span></span>      | <span data-ttu-id="0205e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0205e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0205e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0205e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0205e-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="0205e-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="0205e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0205e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0205e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0205e-115">Not supported.</span></span>|
|<span data-ttu-id="0205e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0205e-116">Application</span></span>|<span data-ttu-id="0205e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0205e-117">Not supported.</span></span>|

<span data-ttu-id="0205e-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="0205e-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="0205e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0205e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0205e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0205e-120">Request headers</span></span>

|<span data-ttu-id="0205e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0205e-121">Name</span></span>|<span data-ttu-id="0205e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0205e-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0205e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0205e-123">Authorization</span></span>|<span data-ttu-id="0205e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0205e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0205e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0205e-126">Request body</span></span>

<span data-ttu-id="0205e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0205e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0205e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0205e-128">Response</span></span>

<span data-ttu-id="0205e-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0205e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0205e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0205e-130">Example</span></span>

<span data-ttu-id="0205e-131">O exemplo a seguir exclui um **trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="0205e-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="0205e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0205e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```

##### <a name="response"></a><span data-ttu-id="0205e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0205e-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0205e-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0205e-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0205e-135">Basic</span><span class="sxs-lookup"><span data-stu-id="0205e-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0205e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0205e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
