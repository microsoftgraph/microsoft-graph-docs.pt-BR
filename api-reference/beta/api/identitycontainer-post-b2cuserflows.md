---
title: Criar b2cIdentityUserFlow
description: Criar um novo objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 98d603632e724817cec2d4c97e06389608cc3f10
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705867"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="ea779-103">Criar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="ea779-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="ea779-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea779-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea779-105">Criar um novo objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="ea779-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea779-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea779-106">Permissions</span></span>

<span data-ttu-id="ea779-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea779-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea779-109">Permission type</span></span>      | <span data-ttu-id="ea779-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea779-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea779-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea779-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea779-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea779-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ea779-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea779-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ea779-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea779-114">Not supported.</span></span>|
|<span data-ttu-id="ea779-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea779-115">Application</span></span>|<span data-ttu-id="ea779-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea779-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ea779-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ea779-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ea779-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ea779-118">Global administrator</span></span>
* <span data-ttu-id="ea779-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="ea779-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ea779-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea779-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="ea779-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea779-121">Request headers</span></span>

|<span data-ttu-id="ea779-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ea779-122">Name</span></span>|<span data-ttu-id="ea779-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea779-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ea779-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea779-124">Authorization</span></span>|<span data-ttu-id="ea779-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea779-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ea779-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea779-127">Content-Type</span></span>|<span data-ttu-id="ea779-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea779-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea779-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea779-130">Request body</span></span>

<span data-ttu-id="ea779-131">No corpo da solicitação, forneça uma representação JSON de um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="ea779-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="ea779-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea779-132">Property</span></span>|<span data-ttu-id="ea779-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea779-133">Type</span></span>|<span data-ttu-id="ea779-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea779-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea779-135">id</span><span class="sxs-lookup"><span data-stu-id="ea779-135">id</span></span>|<span data-ttu-id="ea779-136">String</span><span class="sxs-lookup"><span data-stu-id="ea779-136">String</span></span>|<span data-ttu-id="ea779-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea779-137">Required.</span></span> <span data-ttu-id="ea779-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="ea779-138">The name of the user flow.</span></span> <span data-ttu-id="ea779-139">O nome será pré-instalado com `B2C_1` após a criação.</span><span class="sxs-lookup"><span data-stu-id="ea779-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="ea779-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="ea779-140">userFlowType</span></span>|<span data-ttu-id="ea779-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea779-141">String</span></span>|<span data-ttu-id="ea779-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea779-142">Required.</span></span> <span data-ttu-id="ea779-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="ea779-143">The type of user flow you are creating.</span></span> <span data-ttu-id="ea779-144">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="ea779-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="ea779-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ea779-145">userFlowTypeVersion</span></span>|<span data-ttu-id="ea779-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="ea779-146">Float</span></span>|<span data-ttu-id="ea779-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea779-147">Required.</span></span> <span data-ttu-id="ea779-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="ea779-148">The version of the user flow.</span></span>|
|<span data-ttu-id="ea779-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="ea779-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="ea779-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea779-150">Boolean</span></span>|<span data-ttu-id="ea779-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea779-151">Optional.</span></span> <span data-ttu-id="ea779-152">Determina se a personalização de idioma está habilitada no fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ea779-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="ea779-153">A personalização de idioma não é habilitada por padrão para os fluxos de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ea779-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="ea779-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="ea779-154">defaultLanguageTag</span></span>|<span data-ttu-id="ea779-155">String</span><span class="sxs-lookup"><span data-stu-id="ea779-155">String</span></span>|<span data-ttu-id="ea779-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea779-156">Optional.</span></span>  <span data-ttu-id="ea779-157">Especifica o idioma padrão do b2cIdentityUserFlow usado quando nenhuma `ui_locale` marca é especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea779-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="ea779-158">Este campo é compatível com [RFC 5646](https://tools.ietf.org/html/rfc5646) .</span><span class="sxs-lookup"><span data-stu-id="ea779-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="ea779-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="ea779-159">identityProviders</span></span>|<span data-ttu-id="ea779-160">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="ea779-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="ea779-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea779-161">Optional.</span></span> <span data-ttu-id="ea779-162">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="ea779-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="ea779-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea779-163">Response</span></span>

<span data-ttu-id="ea779-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local com um URI para o objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) criado para essa solicitação, com o `B2C_1` prefixo adicionado ao nome.</span><span class="sxs-lookup"><span data-stu-id="ea779-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="ea779-165">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="ea779-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="ea779-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ea779-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="ea779-167">Exemplo 1: criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="ea779-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="ea779-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea779-168">Request</span></span>

<span data-ttu-id="ea779-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea779-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea779-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea779-170">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="ea779-171">C#</span><span class="sxs-lookup"><span data-stu-id="ea779-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea779-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea779-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea779-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea779-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea779-174">Java</span><span class="sxs-lookup"><span data-stu-id="ea779-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ea779-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea779-175">Response</span></span>

<span data-ttu-id="ea779-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea779-176">The following is an example of the response.</span></span>

<span data-ttu-id="ea779-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ea779-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="ea779-178">Exemplo 2: criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="ea779-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="ea779-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea779-179">Request</span></span>

<span data-ttu-id="ea779-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea779-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea779-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea779-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ea779-182">C#</span><span class="sxs-lookup"><span data-stu-id="ea779-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea779-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea779-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea779-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea779-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea779-185">Java</span><span class="sxs-lookup"><span data-stu-id="ea779-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ea779-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea779-186">Response</span></span>

<span data-ttu-id="ea779-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea779-187">The following is an example of the response.</span></span>

<span data-ttu-id="ea779-188">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ea779-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
