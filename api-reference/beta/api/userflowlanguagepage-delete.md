---
title: Excluir userFlowLanguagePage
description: Exclui os valores em um objeto userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ce15fce0565a7e7fdeb704d645a177342c7ad17d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444613"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="435bb-103">Excluir userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="435bb-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="435bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="435bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="435bb-105">Exclui os valores em um [objeto userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="435bb-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="435bb-106">Você só pode excluir os valores em um overridesPage, que é usado para personalizar os valores mostrados a um usuário durante uma jornada do usuário definida por um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="435bb-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="435bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="435bb-107">Permissions</span></span>

<span data-ttu-id="435bb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="435bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="435bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="435bb-110">Permission type</span></span>      | <span data-ttu-id="435bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="435bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="435bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="435bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="435bb-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="435bb-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="435bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="435bb-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="435bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="435bb-115">Not supported.</span></span>|
|<span data-ttu-id="435bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="435bb-116">Application</span></span>|<span data-ttu-id="435bb-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="435bb-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="435bb-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="435bb-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="435bb-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="435bb-119">Global administrator</span></span>
* <span data-ttu-id="435bb-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="435bb-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="435bb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="435bb-121">HTTP request</span></span>

<span data-ttu-id="435bb-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="435bb-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="435bb-123">Isso retorna o conteúdo dentro do objeto e permite que você o referencia diretamente.</span><span class="sxs-lookup"><span data-stu-id="435bb-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/$value
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="435bb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="435bb-124">Request headers</span></span>

|<span data-ttu-id="435bb-125">Nome</span><span class="sxs-lookup"><span data-stu-id="435bb-125">Name</span></span>|<span data-ttu-id="435bb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="435bb-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="435bb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="435bb-127">Authorization</span></span>|<span data-ttu-id="435bb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="435bb-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="435bb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="435bb-130">Request body</span></span>

<span data-ttu-id="435bb-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="435bb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="435bb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="435bb-132">Response</span></span>

<span data-ttu-id="435bb-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="435bb-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="435bb-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="435bb-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="435bb-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="435bb-135">Request</span></span>

<span data-ttu-id="435bb-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="435bb-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="435bb-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="435bb-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
```
# <a name="c"></a>[<span data-ttu-id="435bb-138">C#</span><span class="sxs-lookup"><span data-stu-id="435bb-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="435bb-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="435bb-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="435bb-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="435bb-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="435bb-141">Java</span><span class="sxs-lookup"><span data-stu-id="435bb-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="435bb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="435bb-142">Response</span></span>

<span data-ttu-id="435bb-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="435bb-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
