---
title: Excluir userFlowLanguageConfiguration
description: Exclui um objeto userFlowLanguageConfiguration de um fluxo de usuário B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3d750145561adefd7532e23ab6cbfc9bff8efe59
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546949"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="08757-103">Excluir userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="08757-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="08757-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08757-105">Exclui um [objeto userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) de um fluxo de [usuário do Azure AD B2C.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="08757-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="08757-106">**Observação:** Não é possível excluir idiomas de um [fluxo Azure Active Directory usuário](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="08757-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08757-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08757-107">Permissions</span></span>

<span data-ttu-id="08757-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08757-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08757-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08757-110">Permission type</span></span>      | <span data-ttu-id="08757-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08757-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08757-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08757-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08757-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08757-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="08757-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08757-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="08757-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08757-115">Not supported.</span></span>|
|<span data-ttu-id="08757-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08757-116">Application</span></span>|<span data-ttu-id="08757-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08757-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="08757-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="08757-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="08757-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="08757-119">Global administrator</span></span>
* <span data-ttu-id="08757-120">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="08757-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="08757-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08757-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="08757-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08757-122">Request headers</span></span>

|<span data-ttu-id="08757-123">Nome</span><span class="sxs-lookup"><span data-stu-id="08757-123">Name</span></span>|<span data-ttu-id="08757-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="08757-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="08757-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="08757-125">Authorization</span></span>|<span data-ttu-id="08757-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08757-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08757-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08757-128">Request body</span></span>

<span data-ttu-id="08757-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08757-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08757-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="08757-130">Response</span></span>

<span data-ttu-id="08757-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="08757-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="08757-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="08757-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08757-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08757-133">Request</span></span>

<span data-ttu-id="08757-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08757-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08757-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="08757-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```
# <a name="c"></a>[<span data-ttu-id="08757-136">C#</span><span class="sxs-lookup"><span data-stu-id="08757-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08757-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08757-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08757-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08757-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08757-139">Java</span><span class="sxs-lookup"><span data-stu-id="08757-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08757-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="08757-140">Response</span></span>

<span data-ttu-id="08757-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08757-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
