---
title: Criar identityUserFlowAttribute
description: Crie um novo objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: ac068b6956c48f67245f6c93dca764cb575e3ba3
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920838"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="c135e-103">Criar identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="c135e-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="c135e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c135e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c135e-105">Crie um novo [objeto identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="c135e-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c135e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c135e-106">Permissions</span></span>

<span data-ttu-id="c135e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c135e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c135e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c135e-109">Permission type</span></span>      | <span data-ttu-id="c135e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c135e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c135e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c135e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c135e-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c135e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c135e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c135e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c135e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c135e-114">Not supported.</span></span>|
|<span data-ttu-id="c135e-115">Application</span><span class="sxs-lookup"><span data-stu-id="c135e-115">Application</span></span>|<span data-ttu-id="c135e-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c135e-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c135e-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c135e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c135e-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c135e-118">Global administrator</span></span>
* <span data-ttu-id="c135e-119">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="c135e-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c135e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c135e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="c135e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c135e-121">Request headers</span></span>

|<span data-ttu-id="c135e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c135e-122">Name</span></span>|<span data-ttu-id="c135e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c135e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c135e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c135e-124">Authorization</span></span>|<span data-ttu-id="c135e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c135e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c135e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c135e-127">Content-Type</span></span>|<span data-ttu-id="c135e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c135e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c135e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c135e-130">Request body</span></span>

<span data-ttu-id="c135e-131">No corpo da solicitação, forneça uma representação JSON de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="c135e-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="c135e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c135e-132">Property</span></span>|<span data-ttu-id="c135e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c135e-133">Type</span></span>|<span data-ttu-id="c135e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c135e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c135e-135">id</span><span class="sxs-lookup"><span data-stu-id="c135e-135">id</span></span>|<span data-ttu-id="c135e-136">String</span><span class="sxs-lookup"><span data-stu-id="c135e-136">String</span></span>|<span data-ttu-id="c135e-137">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c135e-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="c135e-138">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c135e-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="c135e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c135e-139">displayName</span></span>|<span data-ttu-id="c135e-140">String</span><span class="sxs-lookup"><span data-stu-id="c135e-140">String</span></span>|<span data-ttu-id="c135e-141">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c135e-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="c135e-142">descrição</span><span class="sxs-lookup"><span data-stu-id="c135e-142">description</span></span>|<span data-ttu-id="c135e-143">String</span><span class="sxs-lookup"><span data-stu-id="c135e-143">String</span></span>|<span data-ttu-id="c135e-144">A descrição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c135e-144">The description of the user flow attribute.</span></span> <span data-ttu-id="c135e-145">Ele é mostrado para o usuário no momento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="c135e-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="c135e-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="c135e-146">userFlowAttributeType</span></span>|<span data-ttu-id="c135e-147">String</span><span class="sxs-lookup"><span data-stu-id="c135e-147">String</span></span>|<span data-ttu-id="c135e-148">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c135e-148">The type of the user flow attribute.</span></span> <span data-ttu-id="c135e-149">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c135e-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="c135e-150">Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom`.</span><span class="sxs-lookup"><span data-stu-id="c135e-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="c135e-151">dataType</span><span class="sxs-lookup"><span data-stu-id="c135e-151">dataType</span></span>|<span data-ttu-id="c135e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c135e-152">String</span></span>|<span data-ttu-id="c135e-153">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c135e-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="c135e-154">Isso não pode ser modificado depois que o atributo de fluxo de usuário personalizado é criado.</span><span class="sxs-lookup"><span data-stu-id="c135e-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="c135e-155">Os valores com suporte para **tipo de dados** são:</span><span class="sxs-lookup"><span data-stu-id="c135e-155">The supported values for **dataType** are:</span></span><br/><ul><li>`string` </li><li>`boolean`</li><li>`int64`</li></ul>|

## <a name="response"></a><span data-ttu-id="c135e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c135e-156">Response</span></span>

<span data-ttu-id="c135e-157">Se tiver êxito, este método retornará um código de resposta e `201 Created` [um objeto identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c135e-157">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="c135e-158">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="c135e-158">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="c135e-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c135e-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c135e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c135e-160">Request</span></span>

<span data-ttu-id="c135e-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c135e-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c135e-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="c135e-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```
# <a name="c"></a>[<span data-ttu-id="c135e-163">C#</span><span class="sxs-lookup"><span data-stu-id="c135e-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c135e-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c135e-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c135e-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c135e-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c135e-166">Java</span><span class="sxs-lookup"><span data-stu-id="c135e-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c135e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="c135e-167">Response</span></span>

<span data-ttu-id="c135e-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c135e-168">The following is an example of the response.</span></span>

<span data-ttu-id="c135e-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c135e-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
