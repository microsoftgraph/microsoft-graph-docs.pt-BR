---
title: Configurar um conector de API em um fluxo de usuários
description: Habilita ou desabilite um conector de API para uma etapa específica em um fluxo de usuário atualizando a propriedade apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 22bbb3d88860a3fcce098748cae8e7058ea21fc8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664451"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="3167c-103">Configurar userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="3167c-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="3167c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3167c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3167c-105">Atualize a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) para habilitar ou desabilitar um conector de API em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3167c-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="3167c-106">Cada relação da [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.</span><span class="sxs-lookup"><span data-stu-id="3167c-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="3167c-107">Você configura um conector de API para uma etapa específica de cada vez, conforme mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="3167c-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="3167c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3167c-108">Permissions</span></span>

<span data-ttu-id="3167c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3167c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3167c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3167c-111">Permission type</span></span>|<span data-ttu-id="3167c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3167c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3167c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3167c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3167c-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3167c-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3167c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3167c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3167c-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3167c-116">Not supported</span></span>|
|<span data-ttu-id="3167c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3167c-117">Application</span></span>|<span data-ttu-id="3167c-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3167c-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3167c-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="3167c-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3167c-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3167c-120">Global administrator</span></span>
* <span data-ttu-id="3167c-121">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="3167c-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3167c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3167c-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3167c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3167c-123">Request headers</span></span>

|<span data-ttu-id="3167c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3167c-124">Name</span></span>|<span data-ttu-id="3167c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3167c-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3167c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3167c-126">Authorization</span></span>|<span data-ttu-id="3167c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3167c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3167c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3167c-129">Content-Type</span></span>|<span data-ttu-id="3167c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3167c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3167c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3167c-132">Request body</span></span>

<span data-ttu-id="3167c-133">No corpo da solicitação, forneça uma representação JSON da `id` [identidadeApiConnector](../resources/identityapiconnector.md) que você deseja usar a etapa específica.</span><span class="sxs-lookup"><span data-stu-id="3167c-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="3167c-134">Para desabilitar um conector de API, o valor pode ser {} .</span><span class="sxs-lookup"><span data-stu-id="3167c-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="3167c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3167c-135">Response</span></span>

<span data-ttu-id="3167c-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3167c-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3167c-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3167c-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="3167c-138">Exemplo 1: Habilitar o conector de API para Federação pós-IDP ao se inscrever</span><span class="sxs-lookup"><span data-stu-id="3167c-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="3167c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3167c-139">Request</span></span>

<span data-ttu-id="3167c-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3167c-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3167c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3167c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="3167c-142">C#</span><span class="sxs-lookup"><span data-stu-id="3167c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3167c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3167c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3167c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3167c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3167c-145">Java</span><span class="sxs-lookup"><span data-stu-id="3167c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="3167c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3167c-146">Response</span></span> 

<span data-ttu-id="3167c-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3167c-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="3167c-148">Exemplo 2: Habilitar o conector de API para a coleção Post Attribute ao se inscrever</span><span class="sxs-lookup"><span data-stu-id="3167c-148">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="3167c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3167c-149">Request</span></span> 

<span data-ttu-id="3167c-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3167c-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3167c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="3167c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="3167c-152">C#</span><span class="sxs-lookup"><span data-stu-id="3167c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3167c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3167c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3167c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3167c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3167c-155">Java</span><span class="sxs-lookup"><span data-stu-id="3167c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3167c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3167c-156">Response</span></span>

<span data-ttu-id="3167c-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3167c-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="3167c-158">Exemplo 3: Desabilitar um conector de API para a coleção Post Attribute ao se inscrever</span><span class="sxs-lookup"><span data-stu-id="3167c-158">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="3167c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3167c-159">Request</span></span> 

<span data-ttu-id="3167c-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3167c-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3167c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="3167c-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```
# <a name="javascript"></a>[<span data-ttu-id="3167c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3167c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3167c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3167c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3167c-164">Java</span><span class="sxs-lookup"><span data-stu-id="3167c-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3167c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3167c-165">Response</span></span>

<span data-ttu-id="3167c-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3167c-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
