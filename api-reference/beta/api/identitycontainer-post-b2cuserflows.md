---
title: Criar b2cIdentityUserFlow
description: Crie um novo objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 620d6a395c87c8507a9fd6c2bb9d5742a8b560da
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508873"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="768b9-103">Criar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="768b9-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="768b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="768b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="768b9-105">Crie um novo [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="768b9-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="768b9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="768b9-106">Permissions</span></span>

<span data-ttu-id="768b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="768b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="768b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="768b9-109">Permission type</span></span>      | <span data-ttu-id="768b9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="768b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="768b9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="768b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="768b9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="768b9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="768b9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="768b9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="768b9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="768b9-114">Not supported.</span></span>|
|<span data-ttu-id="768b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="768b9-115">Application</span></span>|<span data-ttu-id="768b9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="768b9-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="768b9-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="768b9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="768b9-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="768b9-118">Global administrator</span></span>
* <span data-ttu-id="768b9-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="768b9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="768b9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="768b9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="768b9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="768b9-121">Request headers</span></span>

|<span data-ttu-id="768b9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="768b9-122">Name</span></span>|<span data-ttu-id="768b9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="768b9-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="768b9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="768b9-124">Authorization</span></span>|<span data-ttu-id="768b9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="768b9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="768b9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="768b9-127">Content-Type</span></span>|<span data-ttu-id="768b9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="768b9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="768b9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="768b9-130">Request body</span></span>

<span data-ttu-id="768b9-131">No corpo da solicitação, forneça uma representação JSON de [um b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="768b9-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="768b9-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="768b9-132">Property</span></span>|<span data-ttu-id="768b9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="768b9-133">Type</span></span>|<span data-ttu-id="768b9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="768b9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="768b9-135">id</span><span class="sxs-lookup"><span data-stu-id="768b9-135">id</span></span>|<span data-ttu-id="768b9-136">String</span><span class="sxs-lookup"><span data-stu-id="768b9-136">String</span></span>|<span data-ttu-id="768b9-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="768b9-137">Required.</span></span> <span data-ttu-id="768b9-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="768b9-138">The name of the user flow.</span></span> <span data-ttu-id="768b9-139">O nome será pré-canetado após `B2C_1` a criação.</span><span class="sxs-lookup"><span data-stu-id="768b9-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="768b9-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="768b9-140">userFlowType</span></span>|<span data-ttu-id="768b9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="768b9-141">String</span></span>|<span data-ttu-id="768b9-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="768b9-142">Required.</span></span> <span data-ttu-id="768b9-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="768b9-143">The type of user flow you are creating.</span></span> <span data-ttu-id="768b9-144">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="768b9-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="768b9-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="768b9-145">userFlowTypeVersion</span></span>|<span data-ttu-id="768b9-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="768b9-146">Float</span></span>|<span data-ttu-id="768b9-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="768b9-147">Required.</span></span> <span data-ttu-id="768b9-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="768b9-148">The version of the user flow.</span></span>|
|<span data-ttu-id="768b9-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="768b9-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="768b9-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="768b9-150">Boolean</span></span>|<span data-ttu-id="768b9-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="768b9-151">Optional.</span></span> <span data-ttu-id="768b9-152">Determina se a personalização de idioma está habilitada no fluxo de usuários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="768b9-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="768b9-153">A personalização de idioma não está habilitada por padrão para fluxos de usuários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="768b9-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="768b9-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="768b9-154">defaultLanguageTag</span></span>|<span data-ttu-id="768b9-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="768b9-155">String</span></span>|<span data-ttu-id="768b9-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="768b9-156">Optional.</span></span>  <span data-ttu-id="768b9-157">Especifica o idioma padrão do b2cIdentityUserFlow que é usado quando nenhuma marca é `ui_locale` especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="768b9-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="768b9-158">Esse campo é [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível.</span><span class="sxs-lookup"><span data-stu-id="768b9-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="768b9-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="768b9-159">identityProviders</span></span>|<span data-ttu-id="768b9-160">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="768b9-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="768b9-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="768b9-161">Optional.</span></span> <span data-ttu-id="768b9-162">Os provedores de identidade que você deseja incluir no fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="768b9-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="768b9-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="768b9-163">Response</span></span>

<span data-ttu-id="768b9-164">Se tiver êxito, este método retornará um código de resposta e um header Location com um URI para o `201 Created` [objeto b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) criado para essa solicitação, com o prefixo adicionado ao `B2C_1` nome.</span><span class="sxs-lookup"><span data-stu-id="768b9-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="768b9-165">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="768b9-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="768b9-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="768b9-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="768b9-167">Exemplo 1: Criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="768b9-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="768b9-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="768b9-168">Request</span></span>

<span data-ttu-id="768b9-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="768b9-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="768b9-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="768b9-170">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="768b9-171">C#</span><span class="sxs-lookup"><span data-stu-id="768b9-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="768b9-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="768b9-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="768b9-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="768b9-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="768b9-174">Java</span><span class="sxs-lookup"><span data-stu-id="768b9-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="768b9-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="768b9-175">Response</span></span>

<span data-ttu-id="768b9-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="768b9-176">The following is an example of the response.</span></span>

<span data-ttu-id="768b9-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="768b9-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="768b9-178">Exemplo 2: Criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="768b9-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="768b9-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="768b9-179">Request</span></span>

<span data-ttu-id="768b9-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="768b9-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="768b9-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="768b9-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="768b9-182">C#</span><span class="sxs-lookup"><span data-stu-id="768b9-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="768b9-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="768b9-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="768b9-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="768b9-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="768b9-185">Java</span><span class="sxs-lookup"><span data-stu-id="768b9-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="768b9-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="768b9-186">Response</span></span>

<span data-ttu-id="768b9-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="768b9-187">The following is an example of the response.</span></span>

<span data-ttu-id="768b9-188">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="768b9-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="768b9-189">Exemplo 3: Criar um fluxo de usuário com os valores padrão e configuração para conectores de API</span><span class="sxs-lookup"><span data-stu-id="768b9-189">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="768b9-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="768b9-190">Request</span></span>

<span data-ttu-id="768b9-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="768b9-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="768b9-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="768b9-192">HTTP</span></span>](#tab/http)
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
            "@odata.id": "{apiConnectorId}"
        },
        "postAttributeCollection":{
            "@odata.id": "{apiConnectorId}"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="768b9-193">C#</span><span class="sxs-lookup"><span data-stu-id="768b9-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="768b9-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="768b9-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="768b9-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="768b9-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="768b9-196">Java</span><span class="sxs-lookup"><span data-stu-id="768b9-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="768b9-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="768b9-197">Response</span></span>

<span data-ttu-id="768b9-198">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="768b9-198">The following is an example of the response.</span></span>

<span data-ttu-id="768b9-199">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="768b9-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="768b9-200">**Observação:** A `apiConnectorConfiguration` propriedade sempre retorna um valor ' {} .</span><span class="sxs-lookup"><span data-stu-id="768b9-200">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="768b9-201">Para ver o valor completo com as propriedades de navegação, use [esta](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="768b9-201">To see full value with the navigation properties, use [this](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

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
    "Error: create_b2cUserFlow_from_b2cuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
