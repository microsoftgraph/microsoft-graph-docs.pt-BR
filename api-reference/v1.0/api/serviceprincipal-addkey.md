---
title: 'servicePrincipalName: addKey'
description: Adicione uma credencial de chave a um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a4193d8f879e254c2a276a3f63416c8a3da6b4b1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334446"
---
# <a name="serviceprincipal-addkey"></a><span data-ttu-id="945c2-103">servicePrincipalName: addKey</span><span class="sxs-lookup"><span data-stu-id="945c2-103">servicePrincipal: addKey</span></span>

<span data-ttu-id="945c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="945c2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="945c2-105">Adiciona uma credencial de chave a um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="945c2-105">Adds a key credential to a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="945c2-106">Este método junto com o [RemoveKey](serviceprincipal-removekey.md) pode ser usado por um servicePrincipalName para automatizar as chaves de expiração.</span><span class="sxs-lookup"><span data-stu-id="945c2-106">This method along with [removeKey](serviceprincipal-removekey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="945c2-107">[Criar o servicePrincipalName](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar](../api/serviceprincipal-update.md) as operações do servicePrincipalName podem continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer servicePrincipalName com ou sem o contexto de um usuário.</span><span class="sxs-lookup"><span data-stu-id="945c2-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="945c2-108">Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="945c2-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="945c2-109">Os servicePrincipalName que não têm certificados válidos existentes (por exemplo: nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço.</span><span class="sxs-lookup"><span data-stu-id="945c2-109">ServicePrincipals that don’t have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="945c2-110">[Atualize o servicePrincipalName](../api/serviceprincipal-update.md) pode ser usado para executar uma atualização.</span><span class="sxs-lookup"><span data-stu-id="945c2-110">[Update servicePrincipal](../api/serviceprincipal-update.md) can be used to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="945c2-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="945c2-111">Permissions</span></span>

|<span data-ttu-id="945c2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="945c2-112">Permission type</span></span>      | <span data-ttu-id="945c2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="945c2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="945c2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="945c2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="945c2-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="945c2-115">None.</span></span>  |
|<span data-ttu-id="945c2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="945c2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="945c2-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="945c2-117">None.</span></span>    |
|<span data-ttu-id="945c2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="945c2-118">Application</span></span> | <span data-ttu-id="945c2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="945c2-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="945c2-120">Um servicePrincipalName não precisa de nenhuma permissão específica para o rolo de suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="945c2-120">A servicePrincipal does not need any specific permission to roll it's own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="945c2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="945c2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="945c2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="945c2-122">Request headers</span></span>

| <span data-ttu-id="945c2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="945c2-123">Name</span></span>           | <span data-ttu-id="945c2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="945c2-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="945c2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="945c2-125">Authorization</span></span>  | <span data-ttu-id="945c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="945c2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="945c2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="945c2-128">Content-Type</span></span>   | <span data-ttu-id="945c2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="945c2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="945c2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="945c2-131">Request body</span></span>

<span data-ttu-id="945c2-132">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="945c2-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="945c2-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="945c2-133">Property</span></span>     | <span data-ttu-id="945c2-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="945c2-134">Type</span></span>   |<span data-ttu-id="945c2-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="945c2-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="945c2-136">keycredential</span><span class="sxs-lookup"><span data-stu-id="945c2-136">keyCredential</span></span> | [<span data-ttu-id="945c2-137">keycredential</span><span class="sxs-lookup"><span data-stu-id="945c2-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="945c2-138">A nova credencial de chave de servicePrincipalName a ser adicionada.</span><span class="sxs-lookup"><span data-stu-id="945c2-138">The new servicePrincipal key credential to add.</span></span> <span data-ttu-id="945c2-139">O __tipo__, __uso__ e __chave__ são propriedades obrigatórias para esse uso.</span><span class="sxs-lookup"><span data-stu-id="945c2-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="945c2-140">Os tipos de chave com suporte são:</span><span class="sxs-lookup"><span data-stu-id="945c2-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="945c2-141">`AsymmetricX509Cert`: O uso deve ser `Verify` .</span><span class="sxs-lookup"><span data-stu-id="945c2-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="945c2-142">`X509CertAndPassword`: O uso deve ser`Sign`</span><span class="sxs-lookup"><span data-stu-id="945c2-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="945c2-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="945c2-143">passwordCredential</span></span> | [<span data-ttu-id="945c2-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="945c2-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="945c2-145">Só é necessário definir o __secretText__ que deve conter a senha para a chave.</span><span class="sxs-lookup"><span data-stu-id="945c2-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="945c2-146">Essa propriedade é obrigatória somente para chaves de tipo `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="945c2-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="945c2-147">Defini-lo como `null` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="945c2-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="945c2-148">evidência</span><span class="sxs-lookup"><span data-stu-id="945c2-148">proof</span></span> | <span data-ttu-id="945c2-149">String</span><span class="sxs-lookup"><span data-stu-id="945c2-149">String</span></span> | <span data-ttu-id="945c2-150">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="945c2-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="945c2-151">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes de servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="945c2-151">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="945c2-152">O token deve conter as seguintes declarações:</span><span class="sxs-lookup"><span data-stu-id="945c2-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="945c2-153">`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="945c2-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="945c2-154">`iss`-Issuer precisa ser a __ID__ do servicePrincipalName que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="945c2-154">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="945c2-155">`nbf`-Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="945c2-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="945c2-156">`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="945c2-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="945c2-157">Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.</span><span class="sxs-lookup"><span data-stu-id="945c2-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|


## <a name="response"></a><span data-ttu-id="945c2-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="945c2-158">Response</span></span>

<span data-ttu-id="945c2-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [keycredential](../resources/keycredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="945c2-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="945c2-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="945c2-160">Examples</span></span>

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a><span data-ttu-id="945c2-161">Exemplo 1: adicionando uma nova credencial de chave a um servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="945c2-161">Example 1: Adding a new key credential to a servicePrincipal</span></span>

#### <a name="request"></a><span data-ttu-id="945c2-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="945c2-162">Request</span></span>

<span data-ttu-id="945c2-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="945c2-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="945c2-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="945c2-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/serviceprincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="945c2-165">C#</span><span class="sxs-lookup"><span data-stu-id="945c2-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="945c2-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="945c2-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="945c2-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="945c2-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="945c2-168">Java</span><span class="sxs-lookup"><span data-stu-id="945c2-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addkey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="945c2-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="945c2-169">Response</span></span>

<span data-ttu-id="945c2-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="945c2-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="945c2-171">Exemplo 2: adicionando uma credencial de chave e uma senha associada para a chave</span><span class="sxs-lookup"><span data-stu-id="945c2-171">Example 2: Adding a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="945c2-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="945c2-172">Request</span></span>

<span data-ttu-id="945c2-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="945c2-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/serviceprincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```

#### <a name="response"></a><span data-ttu-id="945c2-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="945c2-174">Response</span></span>

<span data-ttu-id="945c2-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="945c2-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: serviceprincipal_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
