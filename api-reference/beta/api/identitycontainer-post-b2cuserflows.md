---
title: Criar b2cIdentityUserFlow
description: Crie um novo objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0537eaf5baea543ee4cf9dbbd24b8cb80fc4d48d
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844213"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="9e5c1-103">Criar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="9e5c1-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="9e5c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e5c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e5c1-105">Crie um novo [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="9e5c1-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e5c1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9e5c1-106">Permissions</span></span>

<span data-ttu-id="9e5c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e5c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e5c1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e5c1-109">Permission type</span></span>      | <span data-ttu-id="9e5c1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e5c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e5c1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e5c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e5c1-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e5c1-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9e5c1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e5c1-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9e5c1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-114">Not supported.</span></span>|
|<span data-ttu-id="9e5c1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e5c1-115">Application</span></span>|<span data-ttu-id="9e5c1-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e5c1-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9e5c1-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="9e5c1-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9e5c1-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9e5c1-118">Global administrator</span></span>
* <span data-ttu-id="9e5c1-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="9e5c1-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9e5c1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e5c1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="9e5c1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5c1-121">Request headers</span></span>

|<span data-ttu-id="9e5c1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9e5c1-122">Name</span></span>|<span data-ttu-id="9e5c1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e5c1-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9e5c1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e5c1-124">Authorization</span></span>|<span data-ttu-id="9e5c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9e5c1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e5c1-127">Content-Type</span></span>|<span data-ttu-id="9e5c1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e5c1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5c1-130">Request body</span></span>

<span data-ttu-id="9e5c1-131">No corpo da solicitação, forneça uma representação JSON de [um b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="9e5c1-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="9e5c1-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e5c1-132">Property</span></span>|<span data-ttu-id="9e5c1-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e5c1-133">Type</span></span>|<span data-ttu-id="9e5c1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e5c1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e5c1-135">id</span><span class="sxs-lookup"><span data-stu-id="9e5c1-135">id</span></span>|<span data-ttu-id="9e5c1-136">String</span><span class="sxs-lookup"><span data-stu-id="9e5c1-136">String</span></span>|<span data-ttu-id="9e5c1-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-137">Required.</span></span> <span data-ttu-id="9e5c1-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-138">The name of the user flow.</span></span> <span data-ttu-id="9e5c1-139">O nome será pré-canetado após `B2C_1` a criação.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="9e5c1-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="9e5c1-140">userFlowType</span></span>|<span data-ttu-id="9e5c1-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5c1-141">String</span></span>|<span data-ttu-id="9e5c1-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-142">Required.</span></span> <span data-ttu-id="9e5c1-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-143">The type of user flow you are creating.</span></span> <span data-ttu-id="9e5c1-144">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="9e5c1-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="9e5c1-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="9e5c1-145">userFlowTypeVersion</span></span>|<span data-ttu-id="9e5c1-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="9e5c1-146">Float</span></span>|<span data-ttu-id="9e5c1-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-147">Required.</span></span> <span data-ttu-id="9e5c1-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-148">The version of the user flow.</span></span>|
|<span data-ttu-id="9e5c1-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="9e5c1-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="9e5c1-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e5c1-150">Boolean</span></span>|<span data-ttu-id="9e5c1-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-151">Optional.</span></span> <span data-ttu-id="9e5c1-152">Determina se a personalização de idioma está habilitada no fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="9e5c1-153">A personalização de idioma não está habilitada por padrão para fluxos de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="9e5c1-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="9e5c1-154">defaultLanguageTag</span></span>|<span data-ttu-id="9e5c1-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5c1-155">String</span></span>|<span data-ttu-id="9e5c1-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-156">Optional.</span></span>  <span data-ttu-id="9e5c1-157">Especifica o idioma padrão do b2cIdentityUserFlow que é usado quando nenhuma `ui_locale` marca é especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="9e5c1-158">Esse campo é [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="9e5c1-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="9e5c1-159">identityProviders</span></span>|<span data-ttu-id="9e5c1-160">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="9e5c1-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="9e5c1-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-161">Optional.</span></span> <span data-ttu-id="9e5c1-162">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="9e5c1-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e5c1-163">Response</span></span>

<span data-ttu-id="9e5c1-164">Se tiver êxito, este método retornará um código de resposta e um título de local com um URI para o objeto `201 Created` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) criado para essa solicitação, com o prefixo adicionado ao `B2C_1` nome.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="9e5c1-165">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="9e5c1-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e5c1-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="9e5c1-167">Exemplo 1: Criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="9e5c1-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="9e5c1-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5c1-168">Request</span></span>

<span data-ttu-id="9e5c1-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e5c1-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e5c1-170">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="9e5c1-171">C#</span><span class="sxs-lookup"><span data-stu-id="9e5c1-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e5c1-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e5c1-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e5c1-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e5c1-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e5c1-174">Java</span><span class="sxs-lookup"><span data-stu-id="9e5c1-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9e5c1-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e5c1-175">Response</span></span>

<span data-ttu-id="9e5c1-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-176">The following is an example of the response.</span></span>

<span data-ttu-id="9e5c1-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "userFlowTypeVersion": 3,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": "en"
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="9e5c1-178">Exemplo 2: Criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="9e5c1-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="9e5c1-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5c1-179">Request</span></span>

<span data-ttu-id="9e5c1-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e5c1-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e5c1-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9e5c1-182">C#</span><span class="sxs-lookup"><span data-stu-id="9e5c1-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e5c1-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e5c1-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e5c1-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e5c1-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e5c1-185">Java</span><span class="sxs-lookup"><span data-stu-id="9e5c1-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e5c1-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e5c1-186">Response</span></span>

<span data-ttu-id="9e5c1-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-187">The following is an example of the response.</span></span>

<span data-ttu-id="9e5c1-188">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "userFlowTypeVersion": 3,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": "en"
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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="9e5c1-189">Exemplo 3: Criar um fluxo de usuário com os valores padrão e a configuração para conectores de API</span><span class="sxs-lookup"><span data-stu-id="9e5c1-189">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="9e5c1-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5c1-190">Request</span></span>

<span data-ttu-id="9e5c1-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e5c1-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e5c1-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration":{
        "postFederationSignup":{
            "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        },
        "postAttributeCollection":{
            "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="9e5c1-193">C#</span><span class="sxs-lookup"><span data-stu-id="9e5c1-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e5c1-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e5c1-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e5c1-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e5c1-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e5c1-196">Java</span><span class="sxs-lookup"><span data-stu-id="9e5c1-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e5c1-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e5c1-197">Response</span></span>

<span data-ttu-id="9e5c1-198">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-198">The following is an example of the response.</span></span>

<span data-ttu-id="9e5c1-199">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="9e5c1-200">**Observação:** A `apiConnectorConfiguration` propriedade sempre retorna um valor ' {} '.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-200">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="9e5c1-201">Para ver o valor completo com as propriedades de navegação, use [esta](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="9e5c1-201">To see full value with the navigation properties, use [this](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows/$entity",
    "id": "B2C_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2cUserFlow_from_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2cUserFlow_from_b2cUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2cUserFlow_from_b2cuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
