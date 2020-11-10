---
title: Criar identityUserFlowAttribute
description: Criar um novo objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 816b9e94ca95ec61f7a9628de7ede6617cebb7fd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953134"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="928b5-103">Criar identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="928b5-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="928b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="928b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="928b5-105">Criar um novo objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="928b5-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="928b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="928b5-106">Permissions</span></span>

<span data-ttu-id="928b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="928b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="928b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="928b5-109">Permission type</span></span>      | <span data-ttu-id="928b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="928b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="928b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="928b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="928b5-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="928b5-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="928b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="928b5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="928b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="928b5-114">Not supported.</span></span>|
|<span data-ttu-id="928b5-115">Application</span><span class="sxs-lookup"><span data-stu-id="928b5-115">Application</span></span>|<span data-ttu-id="928b5-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="928b5-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="928b5-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="928b5-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="928b5-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="928b5-118">Global administrator</span></span>
* <span data-ttu-id="928b5-119">Administrador do atributo de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="928b5-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="928b5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="928b5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="928b5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="928b5-121">Request headers</span></span>

|<span data-ttu-id="928b5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="928b5-122">Name</span></span>|<span data-ttu-id="928b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="928b5-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="928b5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="928b5-124">Authorization</span></span>|<span data-ttu-id="928b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="928b5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="928b5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="928b5-127">Content-Type</span></span>|<span data-ttu-id="928b5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="928b5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="928b5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="928b5-130">Request body</span></span>

<span data-ttu-id="928b5-131">No corpo da solicitação, forneça uma representação JSON de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="928b5-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="928b5-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="928b5-132">Property</span></span>|<span data-ttu-id="928b5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="928b5-133">Type</span></span>|<span data-ttu-id="928b5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="928b5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="928b5-135">id</span><span class="sxs-lookup"><span data-stu-id="928b5-135">id</span></span>|<span data-ttu-id="928b5-136">String</span><span class="sxs-lookup"><span data-stu-id="928b5-136">String</span></span>|<span data-ttu-id="928b5-137">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="928b5-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="928b5-138">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="928b5-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="928b5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="928b5-139">displayName</span></span>|<span data-ttu-id="928b5-140">String</span><span class="sxs-lookup"><span data-stu-id="928b5-140">String</span></span>|<span data-ttu-id="928b5-141">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="928b5-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="928b5-142">description</span><span class="sxs-lookup"><span data-stu-id="928b5-142">description</span></span>|<span data-ttu-id="928b5-143">String</span><span class="sxs-lookup"><span data-stu-id="928b5-143">String</span></span>|<span data-ttu-id="928b5-144">A descrição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="928b5-144">The description of the user flow attribute.</span></span> <span data-ttu-id="928b5-145">Ele é mostrado ao usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="928b5-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="928b5-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="928b5-146">userFlowAttributeType</span></span>|<span data-ttu-id="928b5-147">String</span><span class="sxs-lookup"><span data-stu-id="928b5-147">String</span></span>|<span data-ttu-id="928b5-148">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="928b5-148">The type of the user flow attribute.</span></span> <span data-ttu-id="928b5-149">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="928b5-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="928b5-150">Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom`.</span><span class="sxs-lookup"><span data-stu-id="928b5-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="928b5-151">dataType</span><span class="sxs-lookup"><span data-stu-id="928b5-151">dataType</span></span>|<span data-ttu-id="928b5-152">String</span><span class="sxs-lookup"><span data-stu-id="928b5-152">String</span></span>|<span data-ttu-id="928b5-153">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="928b5-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="928b5-154">Isso não pode ser modificado depois que o atributo de fluxo do usuário personalizado é criado.</span><span class="sxs-lookup"><span data-stu-id="928b5-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="928b5-155">Os valores com suporte para **tipo de dados** são:</span><span class="sxs-lookup"><span data-stu-id="928b5-155">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="928b5-156">`string` : indica que o tipo de dados de identityUserFlowAttribute é uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="928b5-156">`string` : denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="928b5-157">`boolean` : indica que o tipo de dados de identityUserFlowAttribute é um Boolean.</span><span class="sxs-lookup"><span data-stu-id="928b5-157">`boolean` : denotes that the dataType for the identityUserFlowAttribute is a boolean.</span></span></li><li><span data-ttu-id="928b5-158">`int64` : indica que o tipo de dados de identityUserFlowAttribute é um inteiro.</span><span class="sxs-lookup"><span data-stu-id="928b5-158">`int64` : denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="response"></a><span data-ttu-id="928b5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="928b5-159">Response</span></span>

<span data-ttu-id="928b5-160">Se bem-sucedido, este método retorna um `201 Created` código de resposta e um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="928b5-160">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="928b5-161">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="928b5-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="928b5-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="928b5-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="928b5-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="928b5-163">Request</span></span>

<span data-ttu-id="928b5-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="928b5-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="928b5-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="928b5-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```
# <a name="c"></a>[<span data-ttu-id="928b5-166">C#</span><span class="sxs-lookup"><span data-stu-id="928b5-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="928b5-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="928b5-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="928b5-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="928b5-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="928b5-169">Java</span><span class="sxs-lookup"><span data-stu-id="928b5-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="928b5-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="928b5-170">Response</span></span>

<span data-ttu-id="928b5-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="928b5-171">The following is an example of the response.</span></span>

<span data-ttu-id="928b5-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="928b5-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
