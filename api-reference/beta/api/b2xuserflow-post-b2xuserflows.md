---
title: Criar b2xUserFlow
description: Criar um novo objeto b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2a7b73aae6c918557ef4d2c7dc0357e138333eda
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319636"
---
# <a name="create-b2xuserflow"></a><span data-ttu-id="d8358-103">Criar b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="d8358-103">Create b2xUserFlow</span></span>

<span data-ttu-id="d8358-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8358-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8358-105">Criar um novo objeto [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="d8358-105">Create a new [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8358-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8358-106">Permissions</span></span>

<span data-ttu-id="d8358-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8358-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8358-109">Permission type</span></span>      | <span data-ttu-id="d8358-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8358-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8358-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8358-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8358-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d8358-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d8358-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8358-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d8358-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8358-114">Not supported.</span></span>|
|<span data-ttu-id="d8358-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8358-115">Application</span></span>|<span data-ttu-id="d8358-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d8358-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d8358-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="d8358-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d8358-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d8358-118">Global administrator</span></span>
* <span data-ttu-id="d8358-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="d8358-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d8358-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8358-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="d8358-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8358-121">Request headers</span></span>

|<span data-ttu-id="d8358-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d8358-122">Name</span></span>|<span data-ttu-id="d8358-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8358-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d8358-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8358-124">Authorization</span></span>|<span data-ttu-id="d8358-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8358-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d8358-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8358-127">Content-Type</span></span>|<span data-ttu-id="d8358-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8358-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8358-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8358-130">Request body</span></span>

<span data-ttu-id="d8358-131">No corpo da solicitação, forneça uma representação JSON de um [b2xUserFlow](../resources/b2xuserflows.md).</span><span class="sxs-lookup"><span data-stu-id="d8358-131">In the request body, provide a JSON representation of a [b2xUserFlow](../resources/b2xuserflows.md).</span></span>

|<span data-ttu-id="d8358-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8358-132">Property</span></span>|<span data-ttu-id="d8358-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8358-133">Type</span></span>|<span data-ttu-id="d8358-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8358-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8358-135">id</span><span class="sxs-lookup"><span data-stu-id="d8358-135">id</span></span>|<span data-ttu-id="d8358-136">String</span><span class="sxs-lookup"><span data-stu-id="d8358-136">String</span></span>|<span data-ttu-id="d8358-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8358-137">Required.</span></span> <span data-ttu-id="d8358-138">O nome do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8358-138">The name of the user flow.</span></span> <span data-ttu-id="d8358-139">O nome será pré-instalado com `B2X_1` após a criação.</span><span class="sxs-lookup"><span data-stu-id="d8358-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="d8358-140">userflowtype</span><span class="sxs-lookup"><span data-stu-id="d8358-140">userFlowType</span></span>|<span data-ttu-id="d8358-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8358-141">String</span></span>|<span data-ttu-id="d8358-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8358-142">Required.</span></span> <span data-ttu-id="d8358-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="d8358-143">The type of user flow you are creating.</span></span> <span data-ttu-id="d8358-144">Esse valor será sempre `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="d8358-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="d8358-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="d8358-145">userFlowTypeVersion</span></span>|<span data-ttu-id="d8358-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="d8358-146">Float</span></span>|<span data-ttu-id="d8358-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8358-147">Required.</span></span> <span data-ttu-id="d8358-148">A versão do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8358-148">The version of the user flow.</span></span> <span data-ttu-id="d8358-149">Esse valor será sempre 1.</span><span class="sxs-lookup"><span data-stu-id="d8358-149">This value will always be 1.</span></span>|
|<span data-ttu-id="d8358-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="d8358-150">identityProviders</span></span>|<span data-ttu-id="d8358-151">coleção [identityprovider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="d8358-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="d8358-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8358-152">Optional.</span></span> <span data-ttu-id="d8358-153">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8358-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="d8358-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8358-154">Response</span></span>

<span data-ttu-id="d8358-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local com um URI para o objeto [b2xUserFlow](../resources/b2xuserflows.md) criado para essa solicitação, com o `B2X_1` prefixo adicionado ao nome.</span><span class="sxs-lookup"><span data-stu-id="d8358-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xUserFlow](../resources/b2xuserflows.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="d8358-156">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="d8358-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="d8358-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d8358-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="d8358-158">Exemplo 1: criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="d8358-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="d8358-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8358-159">Request</span></span>

<span data-ttu-id="d8358-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8358-160">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d8358-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8358-161">Response</span></span>

<span data-ttu-id="d8358-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8358-162">The following is an example of the response.</span></span>

<span data-ttu-id="d8358-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8358-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="d8358-164">Exemplo 2: criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="d8358-164">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="d8358-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8358-165">Request</span></span>

<span data-ttu-id="d8358-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8358-166">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d8358-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8358-167">Response</span></span>

<span data-ttu-id="d8358-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8358-168">The following is an example of the response.</span></span>

<span data-ttu-id="d8358-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8358-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
