---
title: Criar b2cUserFlow
description: Criar um novo objeto b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e001b0835e0ca902939d71b6425434cc4ee0446
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319650"
---
# <a name="create-b2cuserflow"></a><span data-ttu-id="a6507-103">Criar b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="a6507-103">Create b2cUserFlow</span></span>

<span data-ttu-id="a6507-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6507-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6507-105">Criar um novo objeto [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="a6507-105">Create a new [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6507-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6507-106">Permissions</span></span>

<span data-ttu-id="a6507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6507-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6507-109">Permission type</span></span>      | <span data-ttu-id="a6507-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6507-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6507-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6507-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6507-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a6507-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a6507-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6507-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a6507-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6507-114">Not supported.</span></span>|
|<span data-ttu-id="a6507-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6507-115">Application</span></span>|<span data-ttu-id="a6507-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a6507-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a6507-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="a6507-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a6507-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a6507-118">Global administrator</span></span>
* <span data-ttu-id="a6507-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="a6507-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a6507-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6507-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="a6507-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6507-121">Request headers</span></span>

|<span data-ttu-id="a6507-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a6507-122">Name</span></span>|<span data-ttu-id="a6507-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6507-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a6507-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6507-124">Authorization</span></span>|<span data-ttu-id="a6507-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6507-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a6507-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6507-127">Content-Type</span></span>|<span data-ttu-id="a6507-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6507-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6507-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6507-130">Request body</span></span>

<span data-ttu-id="a6507-131">No corpo da solicitação, forneça uma representação JSON de um [b2cUserFlow](../resources/b2cuserflows.md).</span><span class="sxs-lookup"><span data-stu-id="a6507-131">In the request body, provide a JSON representation of a [b2cUserFlow](../resources/b2cuserflows.md).</span></span>

|<span data-ttu-id="a6507-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6507-132">Property</span></span>|<span data-ttu-id="a6507-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6507-133">Type</span></span>|<span data-ttu-id="a6507-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6507-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6507-135">id</span><span class="sxs-lookup"><span data-stu-id="a6507-135">id</span></span>|<span data-ttu-id="a6507-136">String</span><span class="sxs-lookup"><span data-stu-id="a6507-136">String</span></span>|<span data-ttu-id="a6507-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6507-137">Required.</span></span> <span data-ttu-id="a6507-138">O nome do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="a6507-138">The name of the user flow.</span></span> <span data-ttu-id="a6507-139">O nome será pré-instalado com `B2C_1` após a criação.</span><span class="sxs-lookup"><span data-stu-id="a6507-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="a6507-140">userflowtype</span><span class="sxs-lookup"><span data-stu-id="a6507-140">userFlowType</span></span>|<span data-ttu-id="a6507-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6507-141">String</span></span>|<span data-ttu-id="a6507-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6507-142">Required.</span></span> <span data-ttu-id="a6507-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="a6507-143">The type of user flow you are creating.</span></span> <span data-ttu-id="a6507-144">Os valores com suporte para **Userflowtype** são:</span><span class="sxs-lookup"><span data-stu-id="a6507-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="a6507-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a6507-145">userFlowTypeVersion</span></span>|<span data-ttu-id="a6507-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="a6507-146">Float</span></span>|<span data-ttu-id="a6507-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6507-147">Required.</span></span> <span data-ttu-id="a6507-148">A versão do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="a6507-148">The version of the user flow.</span></span>|
|<span data-ttu-id="a6507-149">identityProviders</span><span class="sxs-lookup"><span data-stu-id="a6507-149">identityProviders</span></span>|<span data-ttu-id="a6507-150">coleção [identityprovider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="a6507-150">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="a6507-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a6507-151">Optional.</span></span> <span data-ttu-id="a6507-152">Os provedores de identidade que você deseja incluir no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="a6507-152">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="a6507-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6507-153">Response</span></span>

<span data-ttu-id="a6507-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local com um URI para o objeto [b2cUserFlow](../resources/b2cuserflows.md) criado para essa solicitação, com o `B2C_1` prefixo adicionado ao nome.</span><span class="sxs-lookup"><span data-stu-id="a6507-154">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cUserFlow](../resources/b2cuserflows.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="a6507-155">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="a6507-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="a6507-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a6507-156">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="a6507-157">Exemplo 1: criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="a6507-157">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="a6507-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6507-158">Request</span></span>

<span data-ttu-id="a6507-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6507-159">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a6507-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6507-160">Response</span></span>

<span data-ttu-id="a6507-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6507-161">The following is an example of the response.</span></span>

<span data-ttu-id="a6507-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6507-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="a6507-163">Exemplo 2: criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="a6507-163">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="a6507-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6507-164">Request</span></span>

<span data-ttu-id="a6507-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6507-165">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a6507-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6507-166">Response</span></span>

<span data-ttu-id="a6507-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6507-167">The following is an example of the response.</span></span>

<span data-ttu-id="a6507-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6507-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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
