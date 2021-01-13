---
title: Configurar um conector de API em um fluxo de usuários
description: Habilita ou desabilita um conector de API para uma etapa específica em um fluxo de usuário atualizando a propriedade apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf5315c6100c55686001245f91a7a2847a2b5689
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843990"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="0a029-103">Configurar userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="0a029-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="0a029-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a029-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a029-105">Atualize a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) para habilitar ou desabilitar um conector de API em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="0a029-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="0a029-106">Cada relação do [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.</span><span class="sxs-lookup"><span data-stu-id="0a029-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="0a029-107">Você configura um conector de API para uma etapa específica, uma de cada vez, conforme mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="0a029-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a029-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0a029-108">Permissions</span></span>

<span data-ttu-id="0a029-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a029-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a029-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a029-111">Permission type</span></span>|<span data-ttu-id="0a029-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a029-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a029-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a029-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a029-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a029-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0a029-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a029-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a029-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0a029-116">Not supported</span></span>|
|<span data-ttu-id="0a029-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a029-117">Application</span></span>|<span data-ttu-id="0a029-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a029-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0a029-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="0a029-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0a029-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="0a029-120">Global administrator</span></span>
* <span data-ttu-id="0a029-121">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="0a029-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0a029-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a029-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{b2cUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0a029-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a029-123">Request headers</span></span>

|<span data-ttu-id="0a029-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0a029-124">Name</span></span>|<span data-ttu-id="0a029-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a029-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a029-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a029-126">Authorization</span></span>|<span data-ttu-id="0a029-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a029-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0a029-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a029-129">Content-Type</span></span>|<span data-ttu-id="0a029-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a029-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a029-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a029-132">Request body</span></span>

<span data-ttu-id="0a029-133">No corpo da solicitação, forneça uma representação JSON do `id` [identityApiConnector](../resources/identityapiconnector.md) que você deseja usar na etapa específica.</span><span class="sxs-lookup"><span data-stu-id="0a029-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="0a029-134">Para desabilitar um conector de API, o valor pode ser {} .</span><span class="sxs-lookup"><span data-stu-id="0a029-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="0a029-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a029-135">Response</span></span>

<span data-ttu-id="0a029-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a029-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0a029-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0a029-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="0a029-138">Exemplo 1: Habilitar conector de API para Federação Pós-IDP ao se inscrever</span><span class="sxs-lookup"><span data-stu-id="0a029-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="0a029-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a029-139">Request</span></span>

<span data-ttu-id="0a029-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a029-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0a029-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a029-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="0a029-142">C#</span><span class="sxs-lookup"><span data-stu-id="0a029-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a029-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a029-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a029-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a029-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a029-145">Java</span><span class="sxs-lookup"><span data-stu-id="0a029-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="0a029-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a029-146">Response</span></span> 

<span data-ttu-id="0a029-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0a029-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="0a029-148">Exemplo 2: Habilitar o conector de API para a Coleta de Atributos Post ao se inscrever</span><span class="sxs-lookup"><span data-stu-id="0a029-148">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="0a029-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a029-149">Request</span></span> 

<span data-ttu-id="0a029-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a029-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0a029-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a029-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="0a029-152">C#</span><span class="sxs-lookup"><span data-stu-id="0a029-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a029-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a029-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a029-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a029-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a029-155">Java</span><span class="sxs-lookup"><span data-stu-id="0a029-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0a029-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a029-156">Response</span></span>

<span data-ttu-id="0a029-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0a029-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="0a029-158">Exemplo 3: Desabilitar um conector de API para Coleta de Atributos Post ao se inscrever</span><span class="sxs-lookup"><span data-stu-id="0a029-158">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="0a029-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a029-159">Request</span></span> 

<span data-ttu-id="0a029-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a029-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0a029-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a029-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```
# <a name="javascript"></a>[<span data-ttu-id="0a029-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a029-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a029-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a029-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a029-164">Java</span><span class="sxs-lookup"><span data-stu-id="0a029-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0a029-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a029-165">Response</span></span>

<span data-ttu-id="0a029-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0a029-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
