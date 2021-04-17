---
title: Criar identityApiConnector
description: Crie um novo objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cb83cd4484ab20f88c9362d7b67a294a6359ff49
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882404"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="898d9-103">Criar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="898d9-103">Create identityApiConnector</span></span>

<span data-ttu-id="898d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="898d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="898d9-105">Crie um novo [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="898d9-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="898d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="898d9-106">Permissions</span></span>

<span data-ttu-id="898d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="898d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="898d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="898d9-109">Permission type</span></span>                        | <span data-ttu-id="898d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="898d9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="898d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="898d9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="898d9-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="898d9-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="898d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="898d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="898d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="898d9-114">Not supported.</span></span>  |
| <span data-ttu-id="898d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="898d9-115">Application</span></span>                            | <span data-ttu-id="898d9-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="898d9-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="898d9-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="898d9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="898d9-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="898d9-118">Global administrator</span></span>
* <span data-ttu-id="898d9-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="898d9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="898d9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="898d9-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="898d9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="898d9-121">Request headers</span></span>

| <span data-ttu-id="898d9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="898d9-122">Name</span></span>          | <span data-ttu-id="898d9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="898d9-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="898d9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="898d9-124">Authorization</span></span> | <span data-ttu-id="898d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="898d9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="898d9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="898d9-127">Content-Type</span></span>  | <span data-ttu-id="898d9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="898d9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="898d9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="898d9-130">Request body</span></span>

<span data-ttu-id="898d9-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="898d9-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="898d9-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityApiConnector](../resources/identityapiconnector.md).</span><span class="sxs-lookup"><span data-stu-id="898d9-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="898d9-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="898d9-133">Property</span></span>|<span data-ttu-id="898d9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="898d9-134">Type</span></span>|<span data-ttu-id="898d9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="898d9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="898d9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="898d9-136">displayName</span></span>|<span data-ttu-id="898d9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="898d9-137">String</span></span>| <span data-ttu-id="898d9-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="898d9-138">The name of the API connector.</span></span> |
|<span data-ttu-id="898d9-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="898d9-139">targetUrl</span></span>|<span data-ttu-id="898d9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="898d9-140">String</span></span>| <span data-ttu-id="898d9-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="898d9-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="898d9-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="898d9-142">authenticationConfiguration</span></span>|[<span data-ttu-id="898d9-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="898d9-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="898d9-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="898d9-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="898d9-145">[Autenticação básica](../resources/basicauthentication.md) e certificado cliente [PKCS 12](../resources/pkcs12certificate.md) são suportados.</span><span class="sxs-lookup"><span data-stu-id="898d9-145">[Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="898d9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="898d9-146">Response</span></span>

<span data-ttu-id="898d9-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="898d9-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="898d9-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="898d9-148">Examples</span></span>

### <a name="example-1-create-an-api-connector-with-basic-authentication"></a><span data-ttu-id="898d9-149">Exemplo 1: Criar um conector de API com autenticação básica</span><span class="sxs-lookup"><span data-stu-id="898d9-149">Example 1: Create an API connector with basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="898d9-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="898d9-150">Request</span></span>

<span data-ttu-id="898d9-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="898d9-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username": "MyUsername",
      "password": "MyPassword"
    }
}
```

#### <a name="response"></a><span data-ttu-id="898d9-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="898d9-152">Response</span></span>

<span data-ttu-id="898d9-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="898d9-153">The following is an example of the response.</span></span>

><span data-ttu-id="898d9-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="898d9-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "MyUsername",
        "password": "******"
    }
}
```

### <a name="example-2-create-an-api-connector-with-client-certificate-authentication"></a><span data-ttu-id="898d9-155">Exemplo 2: Criar um conector de API com autenticação de certificado de cliente</span><span class="sxs-lookup"><span data-stu-id="898d9-155">Example 2: Create an API connector with client certificate authentication</span></span>

#### <a name="request"></a><span data-ttu-id="898d9-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="898d9-156">Request</span></span>

<span data-ttu-id="898d9-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="898d9-157">The following is an example of the request.</span></span>

> <span data-ttu-id="898d9-158">**Observação:** `authenticationConfiguration` na solicitação é do tipo [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md), que representa a configuração de um certificado necessário para carregar ou criar.</span><span class="sxs-lookup"><span data-stu-id="898d9-158">**Note:** `authenticationConfiguration` in the request is of type [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md), which represents the configuration of a certificate needed on upload or create.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type":"#microsoft.graph.pkcs12Certificate",
        "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        "password": "CertificatePassword"
    }
}
```

#### <a name="response"></a><span data-ttu-id="898d9-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="898d9-159">Response</span></span>

<span data-ttu-id="898d9-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="898d9-160">The following is an example of the response.</span></span>

> <span data-ttu-id="898d9-161">**Observação:** `authenticationConfiguration` na resposta é do tipo [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) porque isso representa as informações públicas dos certificados carregados.</span><span class="sxs-lookup"><span data-stu-id="898d9-161">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
        "certificateList": [
            {
                "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                "notAfter": 1666350522,
                "notBefore": 1508670522,
                "isActive": true
            }
        ]
    }
}
```
