---
title: Criar b2xUserFlow
description: Criar um novo objeto b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 544b113054ac728dcc1d360e1e3ba50618dac60d
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329576"
---
# <a name="create-b2xuserflow"></a><span data-ttu-id="047ed-103">Criar b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="047ed-103">Create b2xUserFlow</span></span>

<span data-ttu-id="047ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="047ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="047ed-105">Criar um novo objeto [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="047ed-105">Create a new [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="047ed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="047ed-106">Permissions</span></span>

<span data-ttu-id="047ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="047ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="047ed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="047ed-109">Permission type</span></span>      | <span data-ttu-id="047ed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="047ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="047ed-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="047ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="047ed-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="047ed-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="047ed-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="047ed-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="047ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="047ed-114">Not supported.</span></span>|
|<span data-ttu-id="047ed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="047ed-115">Application</span></span>|<span data-ttu-id="047ed-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="047ed-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="047ed-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="047ed-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="047ed-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="047ed-118">Global administrator</span></span>
* <span data-ttu-id="047ed-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="047ed-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="047ed-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="047ed-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="047ed-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="047ed-121">Request headers</span></span>

|<span data-ttu-id="047ed-122">Nome</span><span class="sxs-lookup"><span data-stu-id="047ed-122">Name</span></span>|<span data-ttu-id="047ed-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="047ed-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="047ed-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="047ed-124">Authorization</span></span>|<span data-ttu-id="047ed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="047ed-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="047ed-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="047ed-127">Content-Type</span></span>|<span data-ttu-id="047ed-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="047ed-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="047ed-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="047ed-130">Request body</span></span>

<span data-ttu-id="047ed-131">No corpo da solicitação, forneça uma representação JSON de um [b2xUserFlow](../resources/b2xuserflows.md).</span><span class="sxs-lookup"><span data-stu-id="047ed-131">In the request body, provide a JSON representation of a [b2xUserFlow](../resources/b2xuserflows.md).</span></span>

|<span data-ttu-id="047ed-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="047ed-132">Property</span></span>|<span data-ttu-id="047ed-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="047ed-133">Type</span></span>|<span data-ttu-id="047ed-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="047ed-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="047ed-135">id</span><span class="sxs-lookup"><span data-stu-id="047ed-135">id</span></span>|<span data-ttu-id="047ed-136">String</span><span class="sxs-lookup"><span data-stu-id="047ed-136">String</span></span>|<span data-ttu-id="047ed-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="047ed-137">Required.</span></span> <span data-ttu-id="047ed-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="047ed-138">The name of the user flow.</span></span> <span data-ttu-id="047ed-139">O nome será pré-instalado com `B2X_1` após a criação.</span><span class="sxs-lookup"><span data-stu-id="047ed-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="047ed-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="047ed-140">userFlowType</span></span>|<span data-ttu-id="047ed-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="047ed-141">String</span></span>|<span data-ttu-id="047ed-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="047ed-142">Required.</span></span> <span data-ttu-id="047ed-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="047ed-143">The type of user flow you are creating.</span></span> <span data-ttu-id="047ed-144">Esse valor será sempre `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="047ed-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="047ed-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="047ed-145">userFlowTypeVersion</span></span>|<span data-ttu-id="047ed-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="047ed-146">Float</span></span>|<span data-ttu-id="047ed-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="047ed-147">Required.</span></span> <span data-ttu-id="047ed-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="047ed-148">The version of the user flow.</span></span> <span data-ttu-id="047ed-149">Esse valor será sempre 1.</span><span class="sxs-lookup"><span data-stu-id="047ed-149">This value will always be 1.</span></span>|
|<span data-ttu-id="047ed-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="047ed-150">identityProviders</span></span>|<span data-ttu-id="047ed-151">coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="047ed-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="047ed-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="047ed-152">Optional.</span></span> <span data-ttu-id="047ed-153">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="047ed-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="047ed-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="047ed-154">Response</span></span>

<span data-ttu-id="047ed-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local com um URI para o objeto [b2xUserFlow](../resources/b2xuserflows.md) criado para essa solicitação, com o `B2X_1` prefixo adicionado ao nome.</span><span class="sxs-lookup"><span data-stu-id="047ed-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xUserFlow](../resources/b2xuserflows.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="047ed-156">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="047ed-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="047ed-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="047ed-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="047ed-158">Exemplo 1: criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="047ed-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="047ed-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="047ed-159">Request</span></span>

<span data-ttu-id="047ed-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="047ed-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="047ed-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="047ed-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="047ed-162">C#</span><span class="sxs-lookup"><span data-stu-id="047ed-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="047ed-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="047ed-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="047ed-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="047ed-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="047ed-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="047ed-165">Response</span></span>

<span data-ttu-id="047ed-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="047ed-166">The following is an example of the response.</span></span>

<span data-ttu-id="047ed-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="047ed-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="047ed-168">Exemplo 2: criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="047ed-168">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="047ed-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="047ed-169">Request</span></span>

<span data-ttu-id="047ed-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="047ed-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="047ed-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="047ed-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="047ed-172">C#</span><span class="sxs-lookup"><span data-stu-id="047ed-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="047ed-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="047ed-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="047ed-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="047ed-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="047ed-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="047ed-175">Response</span></span>

<span data-ttu-id="047ed-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="047ed-176">The following is an example of the response.</span></span>

<span data-ttu-id="047ed-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="047ed-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
