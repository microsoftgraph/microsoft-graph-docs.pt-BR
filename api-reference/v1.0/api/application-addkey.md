---
title: 'aplicativo: addKey'
description: Adicione uma credencial de chave a um aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f61f463e7071a168328781a8fbd4d990a5fdfd
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288633"
---
# <a name="application-addkey"></a><span data-ttu-id="6344a-103">aplicativo: addKey</span><span class="sxs-lookup"><span data-stu-id="6344a-103">application: addKey</span></span>

<span data-ttu-id="6344a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6344a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6344a-105">Adicione uma credencial de chave a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="6344a-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="6344a-106">Este método, junto com o [RemoveKey](application-removekey.md) , pode ser usado por um aplicativo para automatizar as chaves de expiração.</span><span class="sxs-lookup"><span data-stu-id="6344a-106">This method, along with [removeKey](application-removekey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="6344a-107">[Create Application](../api/application-post-applications.md) and [Update Application](../api/application-update.md) Operations pode continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer aplicativo com ou sem um contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="6344a-107">[Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) operations can continue to be used to add and update key credentials for any application with or without a user's context.</span></span>

<span data-ttu-id="6344a-108">Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="6344a-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="6344a-109">Os aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço.</span><span class="sxs-lookup"><span data-stu-id="6344a-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="6344a-110">Você pode usar a operação [Atualizar aplicativo](../api/application-update.md) para executar uma atualização.</span><span class="sxs-lookup"><span data-stu-id="6344a-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="6344a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="6344a-111">Permissions</span></span>

|<span data-ttu-id="6344a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6344a-112">Permission type</span></span>      | <span data-ttu-id="6344a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6344a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6344a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6344a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6344a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6344a-115">None.</span></span>  |
|<span data-ttu-id="6344a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6344a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6344a-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6344a-117">None.</span></span>    |
|<span data-ttu-id="6344a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6344a-118">Application</span></span> | <span data-ttu-id="6344a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6344a-119">None.</span></span> |

> [!NOTE] 
> <span data-ttu-id="6344a-120">Um aplicativo não precisa de nenhuma permissão específica para rolar suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="6344a-120">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="6344a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6344a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="6344a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6344a-122">Request headers</span></span>

| <span data-ttu-id="6344a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6344a-123">Name</span></span>           | <span data-ttu-id="6344a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6344a-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6344a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6344a-125">Authorization</span></span>  | <span data-ttu-id="6344a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6344a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6344a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6344a-128">Content-Type</span></span>   | <span data-ttu-id="6344a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6344a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6344a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6344a-131">Request body</span></span>

<span data-ttu-id="6344a-132">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="6344a-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="6344a-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6344a-133">Property</span></span>     | <span data-ttu-id="6344a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6344a-134">Type</span></span>   |<span data-ttu-id="6344a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6344a-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6344a-136">keycredential</span><span class="sxs-lookup"><span data-stu-id="6344a-136">keyCredential</span></span> | [<span data-ttu-id="6344a-137">keycredential</span><span class="sxs-lookup"><span data-stu-id="6344a-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="6344a-138">A nova credencial de chave de aplicativo a ser adicionada.</span><span class="sxs-lookup"><span data-stu-id="6344a-138">The new application key credential to add.</span></span> <span data-ttu-id="6344a-139">O __tipo__, __uso__ e __chave__ são propriedades obrigatórias para esse uso.</span><span class="sxs-lookup"><span data-stu-id="6344a-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="6344a-140">Os tipos de chave com suporte são:</span><span class="sxs-lookup"><span data-stu-id="6344a-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="6344a-141">`AsymmetricX509Cert`: O uso deve ser `Verify` .</span><span class="sxs-lookup"><span data-stu-id="6344a-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="6344a-142">`X509CertAndPassword`: O uso deve ser`Sign`</span><span class="sxs-lookup"><span data-stu-id="6344a-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="6344a-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="6344a-143">passwordCredential</span></span> | [<span data-ttu-id="6344a-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="6344a-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="6344a-145">Só é necessário definir o __secretText__ que deve conter a senha para a chave.</span><span class="sxs-lookup"><span data-stu-id="6344a-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="6344a-146">Essa propriedade é obrigatória somente para chaves de tipo `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="6344a-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="6344a-147">Defini-lo como `null` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="6344a-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="6344a-148">evidência</span><span class="sxs-lookup"><span data-stu-id="6344a-148">proof</span></span> | <span data-ttu-id="6344a-149">String</span><span class="sxs-lookup"><span data-stu-id="6344a-149">String</span></span> | <span data-ttu-id="6344a-150">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="6344a-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="6344a-151">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6344a-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="6344a-152">O token deve conter as seguintes declarações:</span><span class="sxs-lookup"><span data-stu-id="6344a-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="6344a-153">`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="6344a-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="6344a-154">`iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="6344a-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="6344a-155">`nbf`-Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="6344a-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="6344a-156">`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="6344a-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="6344a-157">Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.</span><span class="sxs-lookup"><span data-stu-id="6344a-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="6344a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6344a-158">Response</span></span>

<span data-ttu-id="6344a-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [keycredential](../resources/keycredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6344a-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6344a-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6344a-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="6344a-161">Exemplo 1: adicionar uma nova credencial de chave a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="6344a-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="6344a-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6344a-162">Request</span></span>

<span data-ttu-id="6344a-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6344a-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="6344a-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6344a-164">Response</span></span>

<span data-ttu-id="6344a-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6344a-165">The following is an example of the response.</span></span>

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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="6344a-166">Exemplo 2: adicionar uma credencial de chave e uma senha associada para a chave</span><span class="sxs-lookup"><span data-stu-id="6344a-166">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="6344a-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6344a-167">Request</span></span>

<span data-ttu-id="6344a-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6344a-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="6344a-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6344a-169">Response</span></span>

<span data-ttu-id="6344a-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6344a-170">The following is an example of the response.</span></span>

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
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
