---
title: Criar identityApiConnector
description: Crie um novo objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 06515ca0ca1f302ee94cb06e7a58c5dcae518c1b
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508852"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="52112-103">Criar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="52112-103">Create identityApiConnector</span></span>

<span data-ttu-id="52112-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52112-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52112-105">Crie um novo [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="52112-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52112-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="52112-106">Permissions</span></span>

<span data-ttu-id="52112-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52112-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52112-109">Permission type</span></span>                        | <span data-ttu-id="52112-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52112-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="52112-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52112-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52112-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52112-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="52112-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52112-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52112-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52112-114">Not supported.</span></span>  |
| <span data-ttu-id="52112-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52112-115">Application</span></span>                            | <span data-ttu-id="52112-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52112-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="52112-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="52112-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="52112-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="52112-118">Global administrator</span></span>
* <span data-ttu-id="52112-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="52112-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="52112-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52112-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="52112-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52112-121">Request headers</span></span>

| <span data-ttu-id="52112-122">Nome</span><span class="sxs-lookup"><span data-stu-id="52112-122">Name</span></span>          | <span data-ttu-id="52112-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="52112-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="52112-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="52112-124">Authorization</span></span> | <span data-ttu-id="52112-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52112-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="52112-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52112-127">Content-Type</span></span>  | <span data-ttu-id="52112-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52112-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52112-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52112-130">Request body</span></span>

<span data-ttu-id="52112-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="52112-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="52112-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityApiConnector](../resources/identityapiconnector.md).</span><span class="sxs-lookup"><span data-stu-id="52112-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="52112-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52112-133">Property</span></span>|<span data-ttu-id="52112-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="52112-134">Type</span></span>|<span data-ttu-id="52112-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="52112-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52112-136">displayName</span><span class="sxs-lookup"><span data-stu-id="52112-136">displayName</span></span>|<span data-ttu-id="52112-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52112-137">String</span></span>| <span data-ttu-id="52112-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="52112-138">The name of the API connector.</span></span> |
|<span data-ttu-id="52112-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="52112-139">targetUrl</span></span>|<span data-ttu-id="52112-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52112-140">String</span></span>| <span data-ttu-id="52112-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="52112-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="52112-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="52112-142">authenticationConfiguration</span></span>|[<span data-ttu-id="52112-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="52112-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="52112-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="52112-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="52112-145">[Autenticação básica](../resources/basicauthentication.md) e certificado cliente [PKCS 12](../resources/pkcs12certificate.md) são suportados.</span><span class="sxs-lookup"><span data-stu-id="52112-145">[Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="52112-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="52112-146">Response</span></span>

<span data-ttu-id="52112-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52112-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52112-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52112-148">Examples</span></span>

### <a name="example-1-create-an-api-connector-with-basic-authentication"></a><span data-ttu-id="52112-149">Exemplo 1: Criar um conector de API com autenticação básica</span><span class="sxs-lookup"><span data-stu-id="52112-149">Example 1: Create an API connector with basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="52112-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52112-150">Request</span></span>

<span data-ttu-id="52112-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52112-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="52112-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="52112-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username":"<USERNAME>",
      "password":"<PASSWORD>"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="52112-153">C#</span><span class="sxs-lookup"><span data-stu-id="52112-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52112-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52112-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52112-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52112-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52112-156">Java</span><span class="sxs-lookup"><span data-stu-id="52112-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="52112-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="52112-157">Response</span></span>

<span data-ttu-id="52112-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52112-158">The following is an example of the response.</span></span>

><span data-ttu-id="52112-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52112-159">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```

### <a name="example-2-create-an-api-connector-with-client-certificate-authentication"></a><span data-ttu-id="52112-160">Exemplo 2: Criar um conector de API com autenticação de certificado de cliente</span><span class="sxs-lookup"><span data-stu-id="52112-160">Example 2: Create an API connector with client certificate authentication</span></span>

#### <a name="request"></a><span data-ttu-id="52112-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52112-161">Request</span></span>

<span data-ttu-id="52112-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52112-162">The following is an example of the request.</span></span>

> <span data-ttu-id="52112-163">**Observação:** `authenticationConfiguration` na solicitação é do tipo [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md), que representa a configuração de um certificado necessário para carregar ou criar.</span><span class="sxs-lookup"><span data-stu-id="52112-163">**Note:** `authenticationConfiguration` in the request is of type [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md), which represents the configuration of a certificate needed on upload or create.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->
```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type":"#microsoft.graph.pkcs12Certificate",
        "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        "password": "<password>"
    }
}
```

#### <a name="response"></a><span data-ttu-id="52112-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="52112-164">Response</span></span>

<span data-ttu-id="52112-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52112-165">The following is an example of the response.</span></span>

> <span data-ttu-id="52112-166">**Observação:** `authenticationConfiguration` na resposta é do tipo [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) porque isso representa as informações públicas dos certificados carregados.</span><span class="sxs-lookup"><span data-stu-id="52112-166">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
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
