---
title: Criar b2xIdentityUserFlow
description: Crie um novo objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f64b29b242f92caf59a9318caff89f9b401a120e
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844375"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="36518-103">Criar b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="36518-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="36518-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36518-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36518-105">Crie um novo [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="36518-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36518-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="36518-106">Permissions</span></span>

<span data-ttu-id="36518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36518-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36518-109">Permission type</span></span>      | <span data-ttu-id="36518-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36518-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36518-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36518-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36518-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36518-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="36518-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36518-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="36518-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36518-114">Not supported.</span></span>|
|<span data-ttu-id="36518-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36518-115">Application</span></span>|<span data-ttu-id="36518-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36518-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="36518-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="36518-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="36518-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="36518-118">Global administrator</span></span>
* <span data-ttu-id="36518-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="36518-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="36518-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36518-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="36518-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36518-121">Request headers</span></span>

|<span data-ttu-id="36518-122">Nome</span><span class="sxs-lookup"><span data-stu-id="36518-122">Name</span></span>|<span data-ttu-id="36518-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="36518-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="36518-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="36518-124">Authorization</span></span>|<span data-ttu-id="36518-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36518-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="36518-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36518-127">Content-Type</span></span>|<span data-ttu-id="36518-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36518-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36518-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36518-130">Request body</span></span>

<span data-ttu-id="36518-131">No corpo da solicitação, forneça uma representação JSON de [um b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="36518-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="36518-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36518-132">Property</span></span>|<span data-ttu-id="36518-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="36518-133">Type</span></span>|<span data-ttu-id="36518-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="36518-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36518-135">id</span><span class="sxs-lookup"><span data-stu-id="36518-135">id</span></span>|<span data-ttu-id="36518-136">String</span><span class="sxs-lookup"><span data-stu-id="36518-136">String</span></span>|<span data-ttu-id="36518-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36518-137">Required.</span></span> <span data-ttu-id="36518-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="36518-138">The name of the user flow.</span></span> <span data-ttu-id="36518-139">O nome será pré-canetado após `B2X_1` a criação.</span><span class="sxs-lookup"><span data-stu-id="36518-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="36518-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="36518-140">userFlowType</span></span>|<span data-ttu-id="36518-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36518-141">String</span></span>|<span data-ttu-id="36518-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36518-142">Required.</span></span> <span data-ttu-id="36518-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="36518-143">The type of user flow you are creating.</span></span> <span data-ttu-id="36518-144">Esse valor sempre `signUpOrSignIn` será.</span><span class="sxs-lookup"><span data-stu-id="36518-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="36518-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="36518-145">userFlowTypeVersion</span></span>|<span data-ttu-id="36518-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="36518-146">Float</span></span>|<span data-ttu-id="36518-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36518-147">Required.</span></span> <span data-ttu-id="36518-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="36518-148">The version of the user flow.</span></span> <span data-ttu-id="36518-149">Esse valor sempre será 1.</span><span class="sxs-lookup"><span data-stu-id="36518-149">This value will always be 1.</span></span>|
|<span data-ttu-id="36518-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="36518-150">identityProviders</span></span>|<span data-ttu-id="36518-151">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="36518-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="36518-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="36518-152">Optional.</span></span> <span data-ttu-id="36518-153">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="36518-153">The identity providers you want to include in the user flow.</span></span>|
|<span data-ttu-id="36518-154">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="36518-154">apiConnectorConfiguration</span></span>|[<span data-ttu-id="36518-155">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="36518-155">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="36518-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="36518-156">Optional.</span></span> <span data-ttu-id="36518-157">Configuração para habilitar um conector de API para uso como parte do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="36518-157">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="36518-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="36518-158">Response</span></span>

<span data-ttu-id="36518-159">Se tiver êxito, este método retornará um código de resposta e um título de local com um URI para o objeto `201 Created` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) criado para essa solicitação, com o prefixo adicionado ao `B2X_1` nome.</span><span class="sxs-lookup"><span data-stu-id="36518-159">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="36518-160">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="36518-160">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="36518-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36518-161">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="36518-162">Exemplo 1: Criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="36518-162">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="36518-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36518-163">Request</span></span>

<span data-ttu-id="36518-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36518-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36518-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="36518-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36518-166">C#</span><span class="sxs-lookup"><span data-stu-id="36518-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36518-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36518-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36518-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36518-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36518-169">Java</span><span class="sxs-lookup"><span data-stu-id="36518-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36518-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="36518-170">Response</span></span>

<span data-ttu-id="36518-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36518-171">The following is an example of the response.</span></span>

<span data-ttu-id="36518-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36518-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="36518-173">Exemplo 2: Criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="36518-173">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="36518-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36518-174">Request</span></span>

<span data-ttu-id="36518-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36518-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36518-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="36518-176">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36518-177">C#</span><span class="sxs-lookup"><span data-stu-id="36518-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36518-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36518-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36518-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36518-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36518-180">Java</span><span class="sxs-lookup"><span data-stu-id="36518-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36518-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="36518-181">Response</span></span>

<span data-ttu-id="36518-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36518-182">The following is an example of the response.</span></span>

<span data-ttu-id="36518-183">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36518-183">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="36518-184">Exemplo 3: Criar um fluxo de usuário com os valores padrão e a configuração para conectores de API</span><span class="sxs-lookup"><span data-stu-id="36518-184">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="36518-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36518-185">Request</span></span>

<span data-ttu-id="36518-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36518-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36518-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="36518-187">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36518-188">C#</span><span class="sxs-lookup"><span data-stu-id="36518-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36518-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36518-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36518-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36518-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36518-191">Java</span><span class="sxs-lookup"><span data-stu-id="36518-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36518-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="36518-192">Response</span></span>

<span data-ttu-id="36518-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36518-193">The following is an example of the response.</span></span>

<span data-ttu-id="36518-194">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36518-194">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="36518-195">**Observação:** A `apiConnectorConfiguration` propriedade sempre retorna um valor ' {} '.</span><span class="sxs-lookup"><span data-stu-id="36518-195">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="36518-196">Para ver o valor completo com as propriedades de navegação, use [esta](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="36518-196">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

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
