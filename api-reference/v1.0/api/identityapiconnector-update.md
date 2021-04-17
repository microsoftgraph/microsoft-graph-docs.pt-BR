---
title: Atualizar identityApiConnector
description: Atualize as propriedades de um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 23491e1e36400e22d58e4eabef90c72728367f63
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882757"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="f8314-103">Atualizar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="f8314-103">Update identityApiConnector</span></span>

<span data-ttu-id="f8314-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8314-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8314-105">Atualize as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="f8314-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8314-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8314-106">Permissions</span></span>

<span data-ttu-id="f8314-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8314-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8314-109">Permission type</span></span>                        | <span data-ttu-id="f8314-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8314-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f8314-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8314-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8314-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8314-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="f8314-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8314-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8314-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8314-114">Not supported.</span></span>  |
| <span data-ttu-id="f8314-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8314-115">Application</span></span>                            | <span data-ttu-id="f8314-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8314-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="f8314-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f8314-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f8314-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f8314-118">Global administrator</span></span>
* <span data-ttu-id="f8314-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="f8314-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f8314-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8314-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="f8314-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8314-121">Request headers</span></span>
|<span data-ttu-id="f8314-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f8314-122">Name</span></span>|<span data-ttu-id="f8314-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8314-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8314-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8314-124">Authorization</span></span>|<span data-ttu-id="f8314-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8314-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f8314-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8314-127">Content-Type</span></span>|<span data-ttu-id="f8314-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8314-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8314-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8314-130">Request body</span></span>
<span data-ttu-id="f8314-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="f8314-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="f8314-132">A tabela a seguir mostra as propriedades do [identityApiConnector](../resources/identityapiconnector.md) que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="f8314-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="f8314-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8314-133">Property</span></span>|<span data-ttu-id="f8314-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8314-134">Type</span></span>|<span data-ttu-id="f8314-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8314-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8314-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f8314-136">displayName</span></span>|<span data-ttu-id="f8314-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8314-137">String</span></span>| <span data-ttu-id="f8314-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="f8314-138">The name of the API connector.</span></span> |
|<span data-ttu-id="f8314-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="f8314-139">targetUrl</span></span>|<span data-ttu-id="f8314-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8314-140">String</span></span>| <span data-ttu-id="f8314-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="f8314-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="f8314-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8314-142">authenticationConfiguration</span></span>|[<span data-ttu-id="f8314-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="f8314-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="f8314-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="f8314-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="f8314-145">Somente [autenticação básica e](../resources/basicauthentication.md) certificado cliente [PKCS 12](../resources/pkcs12certificate.md) são suportados.</span><span class="sxs-lookup"><span data-stu-id="f8314-145">Only [Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="f8314-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8314-146">Response</span></span>

<span data-ttu-id="f8314-147">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8314-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f8314-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8314-148">Examples</span></span>

### <a name="example-1-changing-display-name-targeturl-and-username--password-used-for-basic-authentication"></a><span data-ttu-id="f8314-149">Exemplo 1: Alterar nome de exibição, targetUrl e nome de usuário & senha usada para autenticação básica</span><span class="sxs-lookup"><span data-stu-id="f8314-149">Example 1: Changing display name, targetUrl, and username & password used for basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="f8314-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8314-150">Request</span></span>

<span data-ttu-id="f8314-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8314-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/apiConnectors/{identityApiConnectorId}
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

#### <a name="response"></a><span data-ttu-id="f8314-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8314-152">Response</span></span>

<span data-ttu-id="f8314-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8314-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-changing-api-connector-to-use-client-certificate-authentication"></a><span data-ttu-id="f8314-154">Exemplo 2: Alterar o conector da API para usar a autenticação de certificado do cliente</span><span class="sxs-lookup"><span data-stu-id="f8314-154">Example 2: Changing API connector to use client certificate authentication</span></span>

<span data-ttu-id="f8314-155">Isso substituirá qualquer configuração anterior authenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8314-155">This will overwrite any previous authenticationConfiguration settings.</span></span> <span data-ttu-id="f8314-156">Para alterar a autenticação básica para a autenticação de certificado, use isso.</span><span class="sxs-lookup"><span data-stu-id="f8314-156">To change from Basic authentication to certificate authentication, use this.</span></span> <span data-ttu-id="f8314-157">Para adicionar certificados adicionais à lista de certificados, use o [método Carregar certificado do](../api/identityapiconnector-uploadclientcertificate.md) cliente.</span><span class="sxs-lookup"><span data-stu-id="f8314-157">To add additional certificates to list of certificates, use the [Upload client certificate](../api/identityapiconnector-uploadclientcertificate.md) method.</span></span> <span data-ttu-id="f8314-158">Ao usar esse método, as operações "Get" ou "List" dos conectores de API serão do tipo `authenticationConfiguration` [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span><span class="sxs-lookup"><span data-stu-id="f8314-158">When using this method, consequent "Get" or "List" operations of API connectors, `authenticationConfiguration` will be of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span></span>

#### <a name="request"></a><span data-ttu-id="f8314-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8314-159">Request</span></span>

<span data-ttu-id="f8314-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8314-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/apiConnectors/be1f769b-9b13-437e-b540-79a905c4932c
Content-Type: application/json

{
  "authenticationConfiguration": {
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "secret"
  }
}
```

#### <a name="response"></a><span data-ttu-id="f8314-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8314-161">Response</span></span>

<span data-ttu-id="f8314-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8314-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
