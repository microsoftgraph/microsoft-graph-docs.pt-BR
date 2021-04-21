---
title: 'identityApiConnector: uploadClientCertificate'
description: Carregue uma chave de formato PKCS 12 (PFX) para uma configuração de autenticação de conectores de API.
localization_priority: Normal
author: nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ed5491867a08999ede0a7db12482b6ee4e0598c8
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920069"
---
# <a name="identityapiconnector-uploadclientcertificate"></a><span data-ttu-id="bd77a-103">identityApiConnector: uploadClientCertificate</span><span class="sxs-lookup"><span data-stu-id="bd77a-103">identityApiConnector: uploadClientCertificate</span></span>

<span data-ttu-id="bd77a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd77a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd77a-105">Carregue uma chave de formato PKCS 12 (.pfx) para a configuração de autenticação de um conector de API.</span><span class="sxs-lookup"><span data-stu-id="bd77a-105">Upload a PKCS 12 format key (.pfx) to an API connector's authentication configuration.</span></span> <span data-ttu-id="bd77a-106">A entrada é um valor codificado de base 64 do conteúdo do certificado PKCS 12.</span><span class="sxs-lookup"><span data-stu-id="bd77a-106">The input is a base-64 encoded value of the PKCS 12 certificate contents.</span></span> <span data-ttu-id="bd77a-107">Este método retorna uma [apiConnector](../resources/identityApiConnector.md).</span><span class="sxs-lookup"><span data-stu-id="bd77a-107">This method returns an [apiConnector](../resources/identityApiConnector.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd77a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bd77a-108">Permissions</span></span>

<span data-ttu-id="bd77a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd77a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd77a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd77a-111">Permission type</span></span>                        | <span data-ttu-id="bd77a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd77a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bd77a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd77a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd77a-114">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd77a-114">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="bd77a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd77a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd77a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd77a-116">Not supported.</span></span>  |
| <span data-ttu-id="bd77a-117">Application</span><span class="sxs-lookup"><span data-stu-id="bd77a-117">Application</span></span>                            | <span data-ttu-id="bd77a-118">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd77a-118">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="bd77a-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="bd77a-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bd77a-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bd77a-120">Global administrator</span></span>
* <span data-ttu-id="bd77a-121">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="bd77a-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bd77a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd77a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/apiconnectors/{id}/uploadClientCertificate
```

## <a name="request-headers"></a><span data-ttu-id="bd77a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd77a-123">Request headers</span></span>

| <span data-ttu-id="bd77a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="bd77a-124">Name</span></span>          | <span data-ttu-id="bd77a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd77a-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd77a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd77a-126">Authorization</span></span> | <span data-ttu-id="bd77a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd77a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd77a-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="bd77a-129">Content-type</span></span>  | <span data-ttu-id="bd77a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd77a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd77a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd77a-132">Request body</span></span>

<span data-ttu-id="bd77a-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd77a-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="bd77a-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd77a-134">Property</span></span>|<span data-ttu-id="bd77a-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd77a-135">Type</span></span>|<span data-ttu-id="bd77a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd77a-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd77a-137">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="bd77a-137">pkcs12Value</span></span>|<span data-ttu-id="bd77a-138">String</span><span class="sxs-lookup"><span data-stu-id="bd77a-138">String</span></span>| <span data-ttu-id="bd77a-139">Este é o campo para enviar o conteúdo pfx.</span><span class="sxs-lookup"><span data-stu-id="bd77a-139">This is the field for sending the pfx content.</span></span> <span data-ttu-id="bd77a-140">O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado.</span><span class="sxs-lookup"><span data-stu-id="bd77a-140">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="bd77a-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd77a-141">Required.</span></span>|
|<span data-ttu-id="bd77a-142">password</span><span class="sxs-lookup"><span data-stu-id="bd77a-142">password</span></span>|<span data-ttu-id="bd77a-143">String</span><span class="sxs-lookup"><span data-stu-id="bd77a-143">String</span></span>| <span data-ttu-id="bd77a-144">Essa é a senha do arquivo pfx.</span><span class="sxs-lookup"><span data-stu-id="bd77a-144">This is the password for the pfx file.</span></span> <span data-ttu-id="bd77a-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd77a-145">Required.</span></span> <span data-ttu-id="bd77a-146">Se nenhuma senha for usada, ainda deverá fornecer um valor `""` de .</span><span class="sxs-lookup"><span data-stu-id="bd77a-146">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="response"></a><span data-ttu-id="bd77a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd77a-147">Response</span></span>

<span data-ttu-id="bd77a-148">Se tiver êxito, este método retornará um código de resposta e o `200 OK` [apiConnector](../resources/identityApiConnector.md) cujo `authenticationConfiguration` contém as informações públicas do certificado do cliente.</span><span class="sxs-lookup"><span data-stu-id="bd77a-148">If successful, this method returns a `200 OK` response code and the [apiConnector](../resources/identityApiConnector.md) whose `authenticationConfiguration` contains the public information of the client certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="bd77a-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd77a-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd77a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd77a-150">Request</span></span>

<span data-ttu-id="bd77a-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd77a-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bd77a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd77a-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityapiconnector_uploadclientcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/identity/apiconnectors/{id}/uploadClientCertificate
Content-type: application/json

{
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "<password>"
}
```
# <a name="c"></a>[<span data-ttu-id="bd77a-153">C#</span><span class="sxs-lookup"><span data-stu-id="bd77a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityapiconnector-uploadclientcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd77a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd77a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityapiconnector-uploadclientcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd77a-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd77a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityapiconnector-uploadclientcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd77a-156">Java</span><span class="sxs-lookup"><span data-stu-id="bd77a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityapiconnector-uploadclientcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd77a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd77a-157">Response</span></span>

<span data-ttu-id="bd77a-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd77a-158">The following is an example of the response.</span></span>

> <span data-ttu-id="bd77a-159">**Observação:** `authenticationConfiguration` na resposta é do tipo [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) porque isso representa as informações públicas dos certificados carregados.</span><span class="sxs-lookup"><span data-stu-id="bd77a-159">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id": "guid",
    "displayName": "My API connector",
    "targetUrl": "https://api.contoso.com/endpoint",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
        "certificateList": [
            {
                "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                "notAfter": 1666350522,
                "notBefore": 1508670522,
                "isActive": true
            },
            {
                "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                "notAfter": 1766350522,
                "notBefore": 1608670522,
                "isActive": false
            }
        ]
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed982019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityApiConnector: uploadClientCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
