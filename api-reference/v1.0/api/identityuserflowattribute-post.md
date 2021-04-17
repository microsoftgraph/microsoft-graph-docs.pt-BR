---
title: Criar identityUserFlowAttribute
description: Crie um novo objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3b5298d433e9ee79ff141f73b1081c7a72374feb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882748"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="0f6e0-103">Criar identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0f6e0-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="0f6e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f6e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f6e0-105">Crie um novo [objeto identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="0f6e0-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f6e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f6e0-106">Permissions</span></span>

<span data-ttu-id="0f6e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f6e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f6e0-109">Permission type</span></span>      | <span data-ttu-id="0f6e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f6e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f6e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f6e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f6e0-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f6e0-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0f6e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f6e0-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0f6e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-114">Not supported.</span></span>|
|<span data-ttu-id="0f6e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f6e0-115">Application</span></span>|<span data-ttu-id="0f6e0-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f6e0-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0f6e0-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="0f6e0-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0f6e0-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="0f6e0-118">Global administrator</span></span>
* <span data-ttu-id="0f6e0-119">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="0f6e0-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0f6e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f6e0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="0f6e0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6e0-121">Request headers</span></span>

|<span data-ttu-id="0f6e0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0f6e0-122">Name</span></span>|<span data-ttu-id="0f6e0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f6e0-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0f6e0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f6e0-124">Authorization</span></span>|<span data-ttu-id="0f6e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0f6e0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f6e0-127">Content-Type</span></span>|<span data-ttu-id="0f6e0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f6e0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6e0-130">Request body</span></span>

<span data-ttu-id="0f6e0-131">No corpo da solicitação, forneça uma representação JSON de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="0f6e0-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="0f6e0-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f6e0-132">Property</span></span>|<span data-ttu-id="0f6e0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f6e0-133">Type</span></span>|<span data-ttu-id="0f6e0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f6e0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f6e0-135">id</span><span class="sxs-lookup"><span data-stu-id="0f6e0-135">id</span></span>|<span data-ttu-id="0f6e0-136">String</span><span class="sxs-lookup"><span data-stu-id="0f6e0-136">String</span></span>|<span data-ttu-id="0f6e0-137">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="0f6e0-138">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="0f6e0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0f6e0-139">displayName</span></span>|<span data-ttu-id="0f6e0-140">String</span><span class="sxs-lookup"><span data-stu-id="0f6e0-140">String</span></span>|<span data-ttu-id="0f6e0-141">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="0f6e0-142">descrição</span><span class="sxs-lookup"><span data-stu-id="0f6e0-142">description</span></span>|<span data-ttu-id="0f6e0-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f6e0-143">String</span></span>|<span data-ttu-id="0f6e0-144">A descrição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-144">The description of the user flow attribute.</span></span> <span data-ttu-id="0f6e0-145">Ele é mostrado para o usuário no momento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="0f6e0-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="0f6e0-146">userFlowAttributeType</span></span>|<span data-ttu-id="0f6e0-147">String</span><span class="sxs-lookup"><span data-stu-id="0f6e0-147">String</span></span>|<span data-ttu-id="0f6e0-148">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-148">The type of the user flow attribute.</span></span> <span data-ttu-id="0f6e0-149">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="0f6e0-150">Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom`.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="0f6e0-151">dataType</span><span class="sxs-lookup"><span data-stu-id="0f6e0-151">dataType</span></span>|<span data-ttu-id="0f6e0-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f6e0-152">String</span></span>|<span data-ttu-id="0f6e0-153">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="0f6e0-154">Isso não pode ser modificado depois que o atributo de fluxo de usuário personalizado é criado.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="0f6e0-155">Os valores com suporte para **tipo de dados** são:</span><span class="sxs-lookup"><span data-stu-id="0f6e0-155">The supported values for **dataType** are:</span></span><br/><ul><li>`string` </li><li>`boolean`</li><li>`int64`</li></ul>|

## <a name="response"></a><span data-ttu-id="0f6e0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f6e0-156">Response</span></span>

<span data-ttu-id="0f6e0-157">Se tiver êxito, este método retornará um código de resposta e `201 Created` [um objeto identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-157">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="0f6e0-158">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-158">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="0f6e0-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f6e0-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f6e0-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f6e0-160">Request</span></span>

<span data-ttu-id="0f6e0-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-161">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="0f6e0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f6e0-162">Response</span></span>

<span data-ttu-id="0f6e0-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-163">The following is an example of the response.</span></span>

<span data-ttu-id="0f6e0-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f6e0-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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
