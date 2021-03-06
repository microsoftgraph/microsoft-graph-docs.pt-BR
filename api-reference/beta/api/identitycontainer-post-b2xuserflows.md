---
title: Criar b2xIdentityUserFlow
description: Crie um novo objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: af73dffdebe41d41e33b463c9c347d36f542985d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515888"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="5bc64-103">Criar b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="5bc64-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="5bc64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bc64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bc64-105">Crie um novo [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="5bc64-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bc64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bc64-106">Permissions</span></span>

<span data-ttu-id="5bc64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bc64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bc64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bc64-109">Permission type</span></span>      | <span data-ttu-id="5bc64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bc64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bc64-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bc64-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5bc64-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bc64-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5bc64-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bc64-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5bc64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bc64-114">Not supported.</span></span>|
|<span data-ttu-id="5bc64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc64-115">Application</span></span>|<span data-ttu-id="5bc64-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bc64-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5bc64-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="5bc64-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5bc64-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5bc64-118">Global administrator</span></span>
* <span data-ttu-id="5bc64-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="5bc64-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5bc64-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bc64-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="5bc64-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bc64-121">Request headers</span></span>

|<span data-ttu-id="5bc64-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5bc64-122">Name</span></span>|<span data-ttu-id="5bc64-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bc64-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5bc64-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bc64-124">Authorization</span></span>|<span data-ttu-id="5bc64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bc64-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5bc64-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bc64-127">Content-Type</span></span>|<span data-ttu-id="5bc64-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bc64-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bc64-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bc64-130">Request body</span></span>

<span data-ttu-id="5bc64-131">No corpo da solicitação, forneça uma representação JSON de [um b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="5bc64-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="5bc64-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bc64-132">Property</span></span>|<span data-ttu-id="5bc64-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bc64-133">Type</span></span>|<span data-ttu-id="5bc64-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bc64-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bc64-135">id</span><span class="sxs-lookup"><span data-stu-id="5bc64-135">id</span></span>|<span data-ttu-id="5bc64-136">String</span><span class="sxs-lookup"><span data-stu-id="5bc64-136">String</span></span>|<span data-ttu-id="5bc64-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bc64-137">Required.</span></span> <span data-ttu-id="5bc64-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="5bc64-138">The name of the user flow.</span></span> <span data-ttu-id="5bc64-139">O nome será pré-canetado após `B2X_1` a criação.</span><span class="sxs-lookup"><span data-stu-id="5bc64-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="5bc64-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="5bc64-140">userFlowType</span></span>|<span data-ttu-id="5bc64-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bc64-141">String</span></span>|<span data-ttu-id="5bc64-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bc64-142">Required.</span></span> <span data-ttu-id="5bc64-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="5bc64-143">The type of user flow you are creating.</span></span> <span data-ttu-id="5bc64-144">Esse valor sempre será `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="5bc64-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="5bc64-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="5bc64-145">userFlowTypeVersion</span></span>|<span data-ttu-id="5bc64-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="5bc64-146">Float</span></span>|<span data-ttu-id="5bc64-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bc64-147">Required.</span></span> <span data-ttu-id="5bc64-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="5bc64-148">The version of the user flow.</span></span> <span data-ttu-id="5bc64-149">Esse valor sempre será 1.</span><span class="sxs-lookup"><span data-stu-id="5bc64-149">This value will always be 1.</span></span>|
|<span data-ttu-id="5bc64-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="5bc64-150">identityProviders</span></span>|<span data-ttu-id="5bc64-151">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="5bc64-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="5bc64-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5bc64-152">Optional.</span></span> <span data-ttu-id="5bc64-153">Os provedores de identidade que você deseja incluir no fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="5bc64-153">The identity providers you want to include in the user flow.</span></span>|
|<span data-ttu-id="5bc64-154">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="5bc64-154">apiConnectorConfiguration</span></span>|[<span data-ttu-id="5bc64-155">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="5bc64-155">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="5bc64-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5bc64-156">Optional.</span></span> <span data-ttu-id="5bc64-157">Configuração para habilitar um conector de API para uso como parte do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="5bc64-157">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="5bc64-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bc64-158">Response</span></span>

<span data-ttu-id="5bc64-159">Se tiver êxito, este método retornará um código de resposta e um header Location com um URI para o objeto `201 Created` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) criado para essa solicitação, com o prefixo adicionado ao `B2X_1` nome.</span><span class="sxs-lookup"><span data-stu-id="5bc64-159">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="5bc64-160">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="5bc64-160">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="5bc64-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5bc64-161">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="5bc64-162">Exemplo 1: Criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="5bc64-162">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="5bc64-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bc64-163">Request</span></span>

<span data-ttu-id="5bc64-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bc64-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bc64-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bc64-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="5bc64-166">C#</span><span class="sxs-lookup"><span data-stu-id="5bc64-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bc64-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bc64-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bc64-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bc64-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bc64-169">Java</span><span class="sxs-lookup"><span data-stu-id="5bc64-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bc64-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bc64-170">Response</span></span>

<span data-ttu-id="5bc64-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bc64-171">The following is an example of the response.</span></span>

<span data-ttu-id="5bc64-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5bc64-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="5bc64-173">Exemplo 2: Criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="5bc64-173">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="5bc64-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bc64-174">Request</span></span>

<span data-ttu-id="5bc64-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bc64-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bc64-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bc64-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="5bc64-177">C#</span><span class="sxs-lookup"><span data-stu-id="5bc64-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bc64-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bc64-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bc64-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bc64-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bc64-180">Java</span><span class="sxs-lookup"><span data-stu-id="5bc64-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bc64-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bc64-181">Response</span></span>

<span data-ttu-id="5bc64-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bc64-182">The following is an example of the response.</span></span>

<span data-ttu-id="5bc64-183">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5bc64-183">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="5bc64-184">Exemplo 3: Criar um fluxo de usuário com os valores padrão e configuração para conectores de API</span><span class="sxs-lookup"><span data-stu-id="5bc64-184">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="5bc64-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bc64-185">Request</span></span>

<span data-ttu-id="5bc64-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bc64-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bc64-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bc64-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
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
# <a name="c"></a>[<span data-ttu-id="5bc64-188">C#</span><span class="sxs-lookup"><span data-stu-id="5bc64-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bc64-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bc64-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bc64-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bc64-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bc64-191">Java</span><span class="sxs-lookup"><span data-stu-id="5bc64-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bc64-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bc64-192">Response</span></span>

<span data-ttu-id="5bc64-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bc64-193">The following is an example of the response.</span></span>

<span data-ttu-id="5bc64-194">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5bc64-194">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="5bc64-195">**Observação:** A `apiConnectorConfiguration` propriedade sempre retorna um valor ' {} .</span><span class="sxs-lookup"><span data-stu-id="5bc64-195">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="5bc64-196">Para ver o valor completo com as propriedades de navegação, use [esta](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="5bc64-196">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows/$entity",
    "id": "B2X_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
