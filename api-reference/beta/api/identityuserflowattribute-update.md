---
title: Atualizar identityUserFlowAttribute
description: Atualizar propriedades de uma identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: c53781dba635e583531682f755b5c76be6dfac5e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435235"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="433fa-103">Atualizar identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="433fa-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="433fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="433fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="433fa-105">Atualize as propriedades de [um objeto identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="433fa-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="433fa-106">Somente atributos de fluxo de usuário personalizados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="433fa-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="433fa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="433fa-107">Permissions</span></span>

<span data-ttu-id="433fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="433fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="433fa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="433fa-110">Permission type</span></span>      | <span data-ttu-id="433fa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="433fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="433fa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="433fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="433fa-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="433fa-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="433fa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="433fa-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="433fa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="433fa-115">Not supported.</span></span>|
|<span data-ttu-id="433fa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="433fa-116">Application</span></span>| <span data-ttu-id="433fa-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="433fa-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="433fa-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="433fa-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="433fa-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="433fa-119">Global administrator</span></span>
* <span data-ttu-id="433fa-120">Administrador de Atributos de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="433fa-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="433fa-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="433fa-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="433fa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="433fa-122">Request headers</span></span>

|<span data-ttu-id="433fa-123">Nome</span><span class="sxs-lookup"><span data-stu-id="433fa-123">Name</span></span>|<span data-ttu-id="433fa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="433fa-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="433fa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="433fa-125">Authorization</span></span>|<span data-ttu-id="433fa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="433fa-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="433fa-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="433fa-128">Content-Type</span></span>|<span data-ttu-id="433fa-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="433fa-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="433fa-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="433fa-131">Request body</span></span>

<span data-ttu-id="433fa-132">No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um [objeto identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="433fa-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="433fa-133">**Observação:** Somente a **propriedade description** pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="433fa-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="433fa-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="433fa-134">Property</span></span>|<span data-ttu-id="433fa-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="433fa-135">Type</span></span>|<span data-ttu-id="433fa-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="433fa-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="433fa-137">description</span><span class="sxs-lookup"><span data-stu-id="433fa-137">description</span></span>|<span data-ttu-id="433fa-138">String</span><span class="sxs-lookup"><span data-stu-id="433fa-138">String</span></span>|<span data-ttu-id="433fa-139">A descrição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="433fa-139">The description of the user flow attribute.</span></span> <span data-ttu-id="433fa-140">Ele é mostrado ao usuário no momento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="433fa-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="433fa-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="433fa-141">Response</span></span>

<span data-ttu-id="433fa-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="433fa-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="433fa-143">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="433fa-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="433fa-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="433fa-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="433fa-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="433fa-145">Request</span></span>

<span data-ttu-id="433fa-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="433fa-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="433fa-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="433fa-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```
# <a name="c"></a>[<span data-ttu-id="433fa-148">C#</span><span class="sxs-lookup"><span data-stu-id="433fa-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="433fa-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="433fa-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="433fa-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="433fa-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="433fa-151">Java</span><span class="sxs-lookup"><span data-stu-id="433fa-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="433fa-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="433fa-152">Response</span></span>

<span data-ttu-id="433fa-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="433fa-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
