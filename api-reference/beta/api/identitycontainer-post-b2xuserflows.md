---
title: Criar b2xIdentityUserFlow
description: Criar um novo objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c178fef7450121574e15fb34245a8843fc120e97
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953500"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="d6399-103">Criar b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="d6399-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="d6399-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6399-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6399-105">Criar um novo objeto [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="d6399-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6399-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6399-106">Permissions</span></span>

<span data-ttu-id="d6399-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6399-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6399-109">Permission type</span></span>      | <span data-ttu-id="d6399-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6399-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6399-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6399-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6399-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6399-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d6399-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6399-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d6399-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6399-114">Not supported.</span></span>|
|<span data-ttu-id="d6399-115">Application</span><span class="sxs-lookup"><span data-stu-id="d6399-115">Application</span></span>|<span data-ttu-id="d6399-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6399-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d6399-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="d6399-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d6399-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d6399-118">Global administrator</span></span>
* <span data-ttu-id="d6399-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="d6399-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d6399-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6399-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="d6399-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6399-121">Request headers</span></span>

|<span data-ttu-id="d6399-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d6399-122">Name</span></span>|<span data-ttu-id="d6399-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6399-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d6399-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6399-124">Authorization</span></span>|<span data-ttu-id="d6399-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6399-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6399-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6399-127">Content-Type</span></span>|<span data-ttu-id="d6399-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6399-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6399-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6399-130">Request body</span></span>

<span data-ttu-id="d6399-131">No corpo da solicitação, forneça uma representação JSON de um [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="d6399-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="d6399-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6399-132">Property</span></span>|<span data-ttu-id="d6399-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6399-133">Type</span></span>|<span data-ttu-id="d6399-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6399-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6399-135">id</span><span class="sxs-lookup"><span data-stu-id="d6399-135">id</span></span>|<span data-ttu-id="d6399-136">String</span><span class="sxs-lookup"><span data-stu-id="d6399-136">String</span></span>|<span data-ttu-id="d6399-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6399-137">Required.</span></span> <span data-ttu-id="d6399-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="d6399-138">The name of the user flow.</span></span> <span data-ttu-id="d6399-139">O nome será pré-instalado com `B2X_1` após a criação.</span><span class="sxs-lookup"><span data-stu-id="d6399-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="d6399-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="d6399-140">userFlowType</span></span>|<span data-ttu-id="d6399-141">String</span><span class="sxs-lookup"><span data-stu-id="d6399-141">String</span></span>|<span data-ttu-id="d6399-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6399-142">Required.</span></span> <span data-ttu-id="d6399-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="d6399-143">The type of user flow you are creating.</span></span> <span data-ttu-id="d6399-144">Esse valor será sempre `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="d6399-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="d6399-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="d6399-145">userFlowTypeVersion</span></span>|<span data-ttu-id="d6399-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="d6399-146">Float</span></span>|<span data-ttu-id="d6399-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6399-147">Required.</span></span> <span data-ttu-id="d6399-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="d6399-148">The version of the user flow.</span></span> <span data-ttu-id="d6399-149">Esse valor será sempre 1.</span><span class="sxs-lookup"><span data-stu-id="d6399-149">This value will always be 1.</span></span>|
|<span data-ttu-id="d6399-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="d6399-150">identityProviders</span></span>|<span data-ttu-id="d6399-151">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="d6399-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="d6399-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6399-152">Optional.</span></span> <span data-ttu-id="d6399-153">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6399-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="d6399-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6399-154">Response</span></span>

<span data-ttu-id="d6399-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local com um URI para o objeto [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) criado para essa solicitação, com o `B2X_1` prefixo adicionado ao nome.</span><span class="sxs-lookup"><span data-stu-id="d6399-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="d6399-156">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="d6399-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="d6399-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6399-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="d6399-158">Exemplo 1: criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="d6399-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="d6399-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6399-159">Request</span></span>

<span data-ttu-id="d6399-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6399-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6399-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6399-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d6399-162">C#</span><span class="sxs-lookup"><span data-stu-id="d6399-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6399-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6399-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6399-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6399-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6399-165">Java</span><span class="sxs-lookup"><span data-stu-id="d6399-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6399-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6399-166">Response</span></span>

<span data-ttu-id="d6399-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d6399-167">The following is an example of the response.</span></span>

<span data-ttu-id="d6399-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6399-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="d6399-169">Exemplo 2: criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="d6399-169">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="d6399-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6399-170">Request</span></span>

<span data-ttu-id="d6399-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6399-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6399-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6399-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d6399-173">C#</span><span class="sxs-lookup"><span data-stu-id="d6399-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6399-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6399-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6399-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6399-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6399-176">Java</span><span class="sxs-lookup"><span data-stu-id="d6399-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6399-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6399-177">Response</span></span>

<span data-ttu-id="d6399-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d6399-178">The following is an example of the response.</span></span>

<span data-ttu-id="d6399-179">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6399-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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


