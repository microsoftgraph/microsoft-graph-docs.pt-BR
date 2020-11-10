---
title: Criar b2cIdentityUserFlow
description: Criar um novo objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65c9508ee1a83ca807b53504869e4d10d5d27f8d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953526"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="8d45a-103">Criar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8d45a-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="8d45a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d45a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d45a-105">Criar um novo objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="8d45a-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d45a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d45a-106">Permissions</span></span>

<span data-ttu-id="8d45a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d45a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d45a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d45a-109">Permission type</span></span>      | <span data-ttu-id="8d45a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d45a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d45a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d45a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d45a-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d45a-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8d45a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d45a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8d45a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d45a-114">Not supported.</span></span>|
|<span data-ttu-id="8d45a-115">Application</span><span class="sxs-lookup"><span data-stu-id="8d45a-115">Application</span></span>|<span data-ttu-id="8d45a-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d45a-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8d45a-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="8d45a-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8d45a-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8d45a-118">Global administrator</span></span>
* <span data-ttu-id="8d45a-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="8d45a-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8d45a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d45a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="8d45a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d45a-121">Request headers</span></span>

|<span data-ttu-id="8d45a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8d45a-122">Name</span></span>|<span data-ttu-id="8d45a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d45a-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8d45a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d45a-124">Authorization</span></span>|<span data-ttu-id="8d45a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d45a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8d45a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d45a-127">Content-Type</span></span>|<span data-ttu-id="8d45a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d45a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d45a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d45a-130">Request body</span></span>

<span data-ttu-id="8d45a-131">No corpo da solicitação, forneça uma representação JSON de um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="8d45a-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="8d45a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d45a-132">Property</span></span>|<span data-ttu-id="8d45a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d45a-133">Type</span></span>|<span data-ttu-id="8d45a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d45a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d45a-135">id</span><span class="sxs-lookup"><span data-stu-id="8d45a-135">id</span></span>|<span data-ttu-id="8d45a-136">String</span><span class="sxs-lookup"><span data-stu-id="8d45a-136">String</span></span>|<span data-ttu-id="8d45a-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d45a-137">Required.</span></span> <span data-ttu-id="8d45a-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="8d45a-138">The name of the user flow.</span></span> <span data-ttu-id="8d45a-139">O nome será pré-instalado com `B2C_1` após a criação.</span><span class="sxs-lookup"><span data-stu-id="8d45a-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="8d45a-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="8d45a-140">userFlowType</span></span>|<span data-ttu-id="8d45a-141">String</span><span class="sxs-lookup"><span data-stu-id="8d45a-141">String</span></span>|<span data-ttu-id="8d45a-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d45a-142">Required.</span></span> <span data-ttu-id="8d45a-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="8d45a-143">The type of user flow you are creating.</span></span> <span data-ttu-id="8d45a-144">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="8d45a-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="8d45a-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8d45a-145">userFlowTypeVersion</span></span>|<span data-ttu-id="8d45a-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="8d45a-146">Float</span></span>|<span data-ttu-id="8d45a-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d45a-147">Required.</span></span> <span data-ttu-id="8d45a-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="8d45a-148">The version of the user flow.</span></span>|
|<span data-ttu-id="8d45a-149">identityProviders</span><span class="sxs-lookup"><span data-stu-id="8d45a-149">identityProviders</span></span>|<span data-ttu-id="8d45a-150">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="8d45a-150">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="8d45a-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8d45a-151">Optional.</span></span> <span data-ttu-id="8d45a-152">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d45a-152">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="8d45a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d45a-153">Response</span></span>

<span data-ttu-id="8d45a-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local com um URI para o objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) criado para essa solicitação, com o `B2C_1` prefixo adicionado ao nome.</span><span class="sxs-lookup"><span data-stu-id="8d45a-154">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="8d45a-155">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="8d45a-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="8d45a-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d45a-156">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="8d45a-157">Exemplo 1: criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="8d45a-157">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="8d45a-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d45a-158">Request</span></span>

<span data-ttu-id="8d45a-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d45a-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d45a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d45a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3
}
```
# <a name="c"></a>[<span data-ttu-id="8d45a-161">C#</span><span class="sxs-lookup"><span data-stu-id="8d45a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d45a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d45a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d45a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d45a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d45a-164">Java</span><span class="sxs-lookup"><span data-stu-id="8d45a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d45a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d45a-165">Response</span></span>

<span data-ttu-id="8d45a-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d45a-166">The following is an example of the response.</span></span>

<span data-ttu-id="8d45a-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d45a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer
Content-type: application/json

{
    "id": "B2C_1_Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="8d45a-168">Exemplo 2: criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="8d45a-168">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="8d45a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d45a-169">Request</span></span>

<span data-ttu-id="8d45a-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d45a-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d45a-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d45a-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows_identityProvider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "Name": "Facebook"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="8d45a-172">C#</span><span class="sxs-lookup"><span data-stu-id="8d45a-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d45a-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d45a-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d45a-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d45a-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d45a-175">Java</span><span class="sxs-lookup"><span data-stu-id="8d45a-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d45a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d45a-176">Response</span></span>

<span data-ttu-id="8d45a-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d45a-177">The following is an example of the response.</span></span>

<span data-ttu-id="8d45a-178">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d45a-178">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer
Content-type: application/json

{
    "id": "B2C_1_Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2cUserFlow_from_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '3'",
    "Error: create_b2cUserFlow_from_b2cUserFlows_identityProvider/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '3'"
  ]
}-->


