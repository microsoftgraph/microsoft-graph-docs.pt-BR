---
title: Criar b2xIdentityUserFlow
description: Crie um novo objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: b5f5d702a7707e942db6bbd6dd85eca02e26eb49
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882847"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="f26a3-103">Criar b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="f26a3-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="f26a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f26a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f26a3-105">Crie um novo [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f26a3-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f26a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f26a3-106">Permissions</span></span>

<span data-ttu-id="f26a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f26a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f26a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f26a3-109">Permission type</span></span>      | <span data-ttu-id="f26a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f26a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f26a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f26a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f26a3-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26a3-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f26a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f26a3-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f26a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f26a3-114">Not supported.</span></span>|
|<span data-ttu-id="f26a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f26a3-115">Application</span></span>|<span data-ttu-id="f26a3-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26a3-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f26a3-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f26a3-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f26a3-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f26a3-118">Global administrator</span></span>
* <span data-ttu-id="f26a3-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="f26a3-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f26a3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f26a3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="f26a3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f26a3-121">Request headers</span></span>

|<span data-ttu-id="f26a3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f26a3-122">Name</span></span>|<span data-ttu-id="f26a3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26a3-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f26a3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f26a3-124">Authorization</span></span>|<span data-ttu-id="f26a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f26a3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f26a3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f26a3-127">Content-Type</span></span>|<span data-ttu-id="f26a3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f26a3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f26a3-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f26a3-130">Request body</span></span>

<span data-ttu-id="f26a3-131">No corpo da solicitação, forneça uma representação JSON de [um b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="f26a3-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="f26a3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f26a3-132">Property</span></span>|<span data-ttu-id="f26a3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f26a3-133">Type</span></span>|<span data-ttu-id="f26a3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26a3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f26a3-135">id</span><span class="sxs-lookup"><span data-stu-id="f26a3-135">id</span></span>|<span data-ttu-id="f26a3-136">String</span><span class="sxs-lookup"><span data-stu-id="f26a3-136">String</span></span>|<span data-ttu-id="f26a3-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f26a3-137">Required.</span></span> <span data-ttu-id="f26a3-138">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="f26a3-138">The name of the user flow.</span></span> <span data-ttu-id="f26a3-139">O nome será pré-canetado após `B2X_1` a criação.</span><span class="sxs-lookup"><span data-stu-id="f26a3-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="f26a3-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="f26a3-140">userFlowType</span></span>|<span data-ttu-id="f26a3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f26a3-141">String</span></span>|<span data-ttu-id="f26a3-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f26a3-142">Required.</span></span> <span data-ttu-id="f26a3-143">O tipo de fluxo de usuário que você está criando.</span><span class="sxs-lookup"><span data-stu-id="f26a3-143">The type of user flow you are creating.</span></span> <span data-ttu-id="f26a3-144">Esse valor sempre será `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="f26a3-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="f26a3-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="f26a3-145">userFlowTypeVersion</span></span>|<span data-ttu-id="f26a3-146">Flutuação</span><span class="sxs-lookup"><span data-stu-id="f26a3-146">Float</span></span>|<span data-ttu-id="f26a3-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f26a3-147">Required.</span></span> <span data-ttu-id="f26a3-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="f26a3-148">The version of the user flow.</span></span> <span data-ttu-id="f26a3-149">Esse valor sempre será 1.</span><span class="sxs-lookup"><span data-stu-id="f26a3-149">This value will always be 1.</span></span>|
|<span data-ttu-id="f26a3-150">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26a3-150">apiConnectorConfiguration</span></span>|[<span data-ttu-id="f26a3-151">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26a3-151">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="f26a3-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f26a3-152">Optional.</span></span> <span data-ttu-id="f26a3-153">Configuração para habilitar um conector de API para uso como parte do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f26a3-153">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="f26a3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f26a3-154">Response</span></span>

<span data-ttu-id="f26a3-155">Se tiver êxito, este método retornará um código de resposta e um header Location com um URI para o objeto `201 Created` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) criado para essa solicitação, com o prefixo adicionado ao `B2X_1` nome.</span><span class="sxs-lookup"><span data-stu-id="f26a3-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="f26a3-156">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="f26a3-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="f26a3-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f26a3-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="f26a3-158">Exemplo 1: Criar um fluxo de usuário com os valores padrão</span><span class="sxs-lookup"><span data-stu-id="f26a3-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="f26a3-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f26a3-159">Request</span></span>

<span data-ttu-id="f26a3-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f26a3-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

#### <a name="response"></a><span data-ttu-id="f26a3-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f26a3-161">Response</span></span>

<span data-ttu-id="f26a3-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f26a3-162">The following is an example of the response.</span></span>

<span data-ttu-id="f26a3-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f26a3-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="f26a3-164">Exemplo 2: Criar um fluxo de usuário com os valores padrão e um provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="f26a3-164">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="f26a3-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f26a3-165">Request</span></span>

<span data-ttu-id="f26a3-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f26a3-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
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

#### <a name="response"></a><span data-ttu-id="f26a3-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f26a3-167">Response</span></span>

<span data-ttu-id="f26a3-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f26a3-168">The following is an example of the response.</span></span>

<span data-ttu-id="f26a3-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f26a3-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="f26a3-170">Exemplo 3: Criar um fluxo de usuário com os valores padrão e configuração para conectores de API</span><span class="sxs-lookup"><span data-stu-id="f26a3-170">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="f26a3-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f26a3-171">Request</span></span>

<span data-ttu-id="f26a3-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f26a3-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration":{
        "postFederationSignup":{
            "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"
        },
        "postAttributeCollection":{
            "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="f26a3-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f26a3-173">Response</span></span>

<span data-ttu-id="f26a3-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f26a3-174">The following is an example of the response.</span></span>

<span data-ttu-id="f26a3-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f26a3-175">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="f26a3-176">**Observação:** A `apiConnectorConfiguration` propriedade sempre retorna um valor ' {} .</span><span class="sxs-lookup"><span data-stu-id="f26a3-176">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="f26a3-177">Para ver o valor completo com as propriedades de navegação, use [esta](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="f26a3-177">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows/$entity",
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
