---
title: 'servicePrincipal: addKey'
description: Adicione uma credencial de chave a uma servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1010f2a5e1a26f834eeeabc9bfe7946515a529bd
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292081"
---
# <a name="serviceprincipal-addkey"></a><span data-ttu-id="accb0-103">servicePrincipal: addKey</span><span class="sxs-lookup"><span data-stu-id="accb0-103">servicePrincipal: addKey</span></span>

<span data-ttu-id="accb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="accb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="accb0-105">Adiciona uma credencial de chave a [um servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="accb0-105">Adds a key credential to a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="accb0-106">Esse método, [juntamente com removeKey,](serviceprincipal-removekey.md) pode ser usado por uma servicePrincipal para automatizar a rolagem de suas chaves expiradas.</span><span class="sxs-lookup"><span data-stu-id="accb0-106">This method along with [removeKey](serviceprincipal-removekey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="accb0-107">[Criar operações servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Update servicePrincipal](../api/serviceprincipal-update.md) podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer servicePrincipal com ou sem o contexto de um usuário.</span><span class="sxs-lookup"><span data-stu-id="accb0-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="accb0-108">Como parte da validação da solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="accb0-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="accb0-109">ServicePrincipals que não têm certificados válidos existentes (ou seja, se nenhum certificado tiver sido adicionado ainda ou todos os certificados expiraram), não poderão usar essa ação de serviço.</span><span class="sxs-lookup"><span data-stu-id="accb0-109">ServicePrincipals that don’t have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="accb0-110">[Atualizar servicePrincipal](../api/serviceprincipal-update.md) pode ser usado para executar uma atualização.</span><span class="sxs-lookup"><span data-stu-id="accb0-110">[Update servicePrincipal](../api/serviceprincipal-update.md) can be used to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="accb0-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="accb0-111">Permissions</span></span>

|<span data-ttu-id="accb0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="accb0-112">Permission type</span></span>      | <span data-ttu-id="accb0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="accb0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="accb0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="accb0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="accb0-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="accb0-115">None.</span></span>  |
|<span data-ttu-id="accb0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="accb0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="accb0-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="accb0-117">None.</span></span>    |
|<span data-ttu-id="accb0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="accb0-118">Application</span></span> | <span data-ttu-id="accb0-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="accb0-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="accb0-120">Uma servicePrincipal não precisa de nenhuma permissão específica para rolar suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="accb0-120">A servicePrincipal does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="accb0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="accb0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="accb0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="accb0-122">Request headers</span></span>

| <span data-ttu-id="accb0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="accb0-123">Name</span></span>           | <span data-ttu-id="accb0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="accb0-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="accb0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="accb0-125">Authorization</span></span>  | <span data-ttu-id="accb0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="accb0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="accb0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="accb0-128">Content-Type</span></span>   | <span data-ttu-id="accb0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="accb0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="accb0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="accb0-131">Request body</span></span>

<span data-ttu-id="accb0-132">No corpo da solicitação, forneça as seguintes propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="accb0-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="accb0-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="accb0-133">Property</span></span>     | <span data-ttu-id="accb0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="accb0-134">Type</span></span>   |<span data-ttu-id="accb0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="accb0-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="accb0-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="accb0-136">keyCredential</span></span> | [<span data-ttu-id="accb0-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="accb0-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="accb0-138">A nova credencial de chave servicePrincipal a ser acrescentada.</span><span class="sxs-lookup"><span data-stu-id="accb0-138">The new servicePrincipal key credential to add.</span></span> <span data-ttu-id="accb0-139">O __tipo__, __uso__ __e chave__ são propriedades necessárias para esse uso.</span><span class="sxs-lookup"><span data-stu-id="accb0-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="accb0-140">Os tipos de chave com suporte são:</span><span class="sxs-lookup"><span data-stu-id="accb0-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="accb0-141">`AsymmetricX509Cert`: o uso deve `Verify` ser.</span><span class="sxs-lookup"><span data-stu-id="accb0-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="accb0-142">`X509CertAndPassword`: o uso deve ser `Sign`</span><span class="sxs-lookup"><span data-stu-id="accb0-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="accb0-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="accb0-143">passwordCredential</span></span> | [<span data-ttu-id="accb0-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="accb0-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="accb0-145">Somente __secretText__ é necessário para ser definido que deve conter a senha da chave.</span><span class="sxs-lookup"><span data-stu-id="accb0-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="accb0-146">Essa propriedade é necessária somente para chaves do tipo `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="accb0-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="accb0-147">De definida como `null` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="accb0-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="accb0-148">proof</span><span class="sxs-lookup"><span data-stu-id="accb0-148">proof</span></span> | <span data-ttu-id="accb0-149">String</span><span class="sxs-lookup"><span data-stu-id="accb0-149">String</span></span> | <span data-ttu-id="accb0-150">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="accb0-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="accb0-151">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="accb0-151">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="accb0-152">O token deve conter os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="accb0-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="accb0-153">`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="accb0-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="accb0-154">`iss` - O emissor precisa ser a __ID__  do servicePrincipal que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="accb0-154">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="accb0-155">`nbf` – Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="accb0-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="accb0-156">`exp` – O tempo de expiração deve ser "nbf" + 10 min.</span><span class="sxs-lookup"><span data-stu-id="accb0-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="accb0-157">Aqui está um exemplo [de código](/graph/application-rollkey-prooftoken) que pode ser usado para gerar esse token de comprovação de posse.</span><span class="sxs-lookup"><span data-stu-id="accb0-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="accb0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="accb0-158">Response</span></span>

<span data-ttu-id="accb0-159">Se bem-sucedido, este método retorna um código `200 OK` de resposta e um novo objeto [keyCredential](../resources/keycredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="accb0-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="accb0-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="accb0-160">Examples</span></span>

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a><span data-ttu-id="accb0-161">Exemplo 1: Adicionando uma nova credencial de chave a uma servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="accb0-161">Example 1: Adding a new key credential to a servicePrincipal</span></span>

#### <a name="request"></a><span data-ttu-id="accb0-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="accb0-162">Request</span></span>

<span data-ttu-id="accb0-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="accb0-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="accb0-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="accb0-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
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
# <a name="javascript"></a>[<span data-ttu-id="accb0-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="accb0-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="accb0-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="accb0-166">Response</span></span>

<span data-ttu-id="accb0-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="accb0-167">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="accb0-168">Exemplo 2: Adicionando uma credencial de chave e uma senha associada à chave</span><span class="sxs-lookup"><span data-stu-id="accb0-168">Example 2: Adding a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="accb0-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="accb0-169">Request</span></span>

<span data-ttu-id="accb0-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="accb0-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="accb0-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="accb0-171">Response</span></span>

<span data-ttu-id="accb0-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="accb0-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
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
  ]
}-->



