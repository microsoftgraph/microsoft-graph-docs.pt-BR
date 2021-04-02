---
title: Atualizar identityApiConnector
description: Atualize as propriedades de um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b7383d82f30f76bc97fc9e66dd57c21044a963ca
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508628"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="91010-103">Atualizar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="91010-103">Update identityApiConnector</span></span>

<span data-ttu-id="91010-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91010-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91010-105">Atualize as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="91010-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91010-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="91010-106">Permissions</span></span>

<span data-ttu-id="91010-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91010-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91010-109">Permission type</span></span>                        | <span data-ttu-id="91010-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91010-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="91010-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91010-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91010-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91010-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="91010-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91010-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91010-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91010-114">Not supported.</span></span>  |
| <span data-ttu-id="91010-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91010-115">Application</span></span>                            | <span data-ttu-id="91010-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91010-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="91010-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="91010-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="91010-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="91010-118">Global administrator</span></span>
* <span data-ttu-id="91010-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="91010-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="91010-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91010-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="91010-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91010-121">Request headers</span></span>
|<span data-ttu-id="91010-122">Nome</span><span class="sxs-lookup"><span data-stu-id="91010-122">Name</span></span>|<span data-ttu-id="91010-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="91010-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="91010-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="91010-124">Authorization</span></span>|<span data-ttu-id="91010-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91010-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="91010-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91010-127">Content-Type</span></span>|<span data-ttu-id="91010-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91010-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91010-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91010-130">Request body</span></span>
<span data-ttu-id="91010-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="91010-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="91010-132">A tabela a seguir mostra as propriedades do [identityApiConnector](../resources/identityapiconnector.md) que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="91010-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="91010-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91010-133">Property</span></span>|<span data-ttu-id="91010-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="91010-134">Type</span></span>|<span data-ttu-id="91010-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="91010-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91010-136">displayName</span><span class="sxs-lookup"><span data-stu-id="91010-136">displayName</span></span>|<span data-ttu-id="91010-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91010-137">String</span></span>| <span data-ttu-id="91010-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="91010-138">The name of the API connector.</span></span> |
|<span data-ttu-id="91010-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="91010-139">targetUrl</span></span>|<span data-ttu-id="91010-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91010-140">String</span></span>| <span data-ttu-id="91010-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="91010-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="91010-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="91010-142">authenticationConfiguration</span></span>|[<span data-ttu-id="91010-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="91010-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="91010-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="91010-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="91010-145">Somente [autenticação básica e](../resources/basicauthentication.md) certificado cliente [PKCS 12](../resources/pkcs12certificate.md) são suportados.</span><span class="sxs-lookup"><span data-stu-id="91010-145">Only [Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="91010-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="91010-146">Response</span></span>

<span data-ttu-id="91010-147">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91010-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="91010-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="91010-148">Examples</span></span>

### <a name="example-1-changing-display-name-targeturl-and-username--password-used-for-basic-authentication"></a><span data-ttu-id="91010-149">Exemplo 1: Alterar nome de exibição, targetUrl e nome de usuário & senha usada para autenticação básica</span><span class="sxs-lookup"><span data-stu-id="91010-149">Example 1: Changing display name, targetUrl, and username & password used for basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="91010-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91010-150">Request</span></span>

<span data-ttu-id="91010-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91010-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91010-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="91010-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "displayName": "New Test API",
  "targetUrl": "https://otherapi.com/api/endpoint",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.basicAuthentication",
    "username":"<NEW_USERNAME>", 
    "password":"<NEW_PASSWORD>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="91010-153">C#</span><span class="sxs-lookup"><span data-stu-id="91010-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91010-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91010-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91010-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91010-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91010-156">Java</span><span class="sxs-lookup"><span data-stu-id="91010-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="91010-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="91010-157">Response</span></span>

<span data-ttu-id="91010-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91010-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-changing-api-connector-to-use-client-certificate-authentication"></a><span data-ttu-id="91010-159">Exemplo 2: Alterar o conector da API para usar a autenticação de certificado do cliente</span><span class="sxs-lookup"><span data-stu-id="91010-159">Example 2: Changing API connector to use client certificate authentication</span></span>

> <span data-ttu-id="91010-160">**Observação:** Isso substituirá qualquer configuração anterior authenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="91010-160">**Note:** This will overwrite any previous authenticationConfiguration settings.</span></span> <span data-ttu-id="91010-161">Para alterar a autenticação básica para a autenticação de certificado, use isso.</span><span class="sxs-lookup"><span data-stu-id="91010-161">To change from Basic authentication to certificate authentication, use this.</span></span> <span data-ttu-id="91010-162">Para adicionar certificados adicionais à lista de certificados, use o [método Carregar certificado do](../api/identityapiconnector-uploadclientcertificate.md) cliente.</span><span class="sxs-lookup"><span data-stu-id="91010-162">To add additional certificates to list of certificates, use the [Upload client certificate](../api/identityapiconnector-uploadclientcertificate.md) method.</span></span> <span data-ttu-id="91010-163">Ao usar esse método, as operações "Get" ou "List" dos conectores de API serão do tipo `authenticationConfiguration` [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span><span class="sxs-lookup"><span data-stu-id="91010-163">When using this method, consequent "Get" or "List" operations of API connectors, `authenticationConfiguration` will be of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span></span>

#### <a name="request"></a><span data-ttu-id="91010-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91010-164">Request</span></span>

<span data-ttu-id="91010-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91010-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "authenticationConfiguration": {
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "secret"
  }
}
```

#### <a name="response"></a><span data-ttu-id="91010-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="91010-166">Response</span></span>

<span data-ttu-id="91010-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91010-167">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
