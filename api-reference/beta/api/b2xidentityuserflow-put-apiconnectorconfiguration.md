---
title: Configurar um conector de API em um fluxo de usuário
description: Habilitar ou desabilitar um conector de API para uma etapa específica em um fluxo de usuário, atualizando a propriedade apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6291c0205f69090a22d33cec847087731af75304
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720063"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="32fc0-103">Configurar userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="32fc0-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="32fc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32fc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32fc0-105">Atualize a propriedade [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em um [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) para habilitar ou desabilitar um conector de API em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="32fc0-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="32fc0-106">Cada relação do [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.</span><span class="sxs-lookup"><span data-stu-id="32fc0-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="32fc0-107">Você configura um conector de API para uma etapa específica de cada vez, conforme mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="32fc0-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="32fc0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="32fc0-108">Permissions</span></span>

<span data-ttu-id="32fc0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32fc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32fc0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32fc0-111">Permission type</span></span>|<span data-ttu-id="32fc0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32fc0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32fc0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32fc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32fc0-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fc0-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="32fc0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32fc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32fc0-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="32fc0-116">Not supported</span></span>|
|<span data-ttu-id="32fc0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32fc0-117">Application</span></span>|<span data-ttu-id="32fc0-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fc0-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="32fc0-119">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="32fc0-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="32fc0-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="32fc0-120">Global administrator</span></span>
* <span data-ttu-id="32fc0-121">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="32fc0-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="32fc0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32fc0-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="32fc0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32fc0-123">Request headers</span></span>

|<span data-ttu-id="32fc0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="32fc0-124">Name</span></span>|<span data-ttu-id="32fc0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="32fc0-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32fc0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="32fc0-126">Authorization</span></span>|<span data-ttu-id="32fc0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32fc0-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32fc0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32fc0-129">Content-Type</span></span>|<span data-ttu-id="32fc0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32fc0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32fc0-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32fc0-132">Request body</span></span>

<span data-ttu-id="32fc0-133">No corpo da solicitação, forneça uma representação JSON do `id` [identityApiConnector](../resources/identityapiconnector.md) que você deseja usar para a etapa específica.</span><span class="sxs-lookup"><span data-stu-id="32fc0-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="32fc0-134">Para desabilitar um conector de API, o valor pode ser {} .</span><span class="sxs-lookup"><span data-stu-id="32fc0-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="32fc0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32fc0-135">Response</span></span>

<span data-ttu-id="32fc0-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32fc0-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="32fc0-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="32fc0-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="32fc0-138">Exemplo 1: habilitar o conector de API para postar Federação IDP ao inscrever-se</span><span class="sxs-lookup"><span data-stu-id="32fc0-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="32fc0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32fc0-139">Request</span></span>

<span data-ttu-id="32fc0-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32fc0-140">The following is an example of the request.</span></span>

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

---

#### <a name="response"></a><span data-ttu-id="32fc0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="32fc0-141">Response</span></span> 

<span data-ttu-id="32fc0-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32fc0-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="32fc0-143">Exemplo 2: habilitar o conector de API para o conjunto de atributos post ao inscrever-se</span><span class="sxs-lookup"><span data-stu-id="32fc0-143">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="32fc0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32fc0-144">Request</span></span> 

<span data-ttu-id="32fc0-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32fc0-145">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="32fc0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="32fc0-146">Response</span></span>

<span data-ttu-id="32fc0-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32fc0-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="32fc0-148">Exemplo 3: desabilitar um conector de API para coleção de atributos post ao inscrever-se</span><span class="sxs-lookup"><span data-stu-id="32fc0-148">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="32fc0-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32fc0-149">Request</span></span> 

<span data-ttu-id="32fc0-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32fc0-150">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="32fc0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="32fc0-151">Response</span></span>

<span data-ttu-id="32fc0-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32fc0-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
