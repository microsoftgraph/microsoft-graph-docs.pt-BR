---
title: 'aplicativo: addKey'
description: Adicione uma credencial de chave a um aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a39946a0188f1fb8327e4f5269aac106d89c8acd
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289387"
---
# <a name="application-addkey"></a><span data-ttu-id="822f8-103">aplicativo: addKey</span><span class="sxs-lookup"><span data-stu-id="822f8-103">application: addKey</span></span>

<span data-ttu-id="822f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="822f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="822f8-105">Adicione uma credencial de chave a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="822f8-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="822f8-106">Esse método, junto com o [RemoveKey](application-removekey.md), pode ser usado por um aplicativo para automatizar as chaves de expiração.</span><span class="sxs-lookup"><span data-stu-id="822f8-106">This method, along with [removeKey](application-removekey.md), can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="822f8-107">Você pode continuar a usar as operações [criar aplicativo](../api/application-post-applications.md) e [Atualizar](../api/application-update.md) aplicativo de aplicativo para adicionar e atualizar as principais credenciais de qualquer aplicativo com ou sem o contexto de um usuário.</span><span class="sxs-lookup"><span data-stu-id="822f8-107">You can continue to use the [Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) application operations to add and update key credentials for any application with or without a user's context.</span></span> 

<span data-ttu-id="822f8-108">Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="822f8-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="822f8-109">Os aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço.</span><span class="sxs-lookup"><span data-stu-id="822f8-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="822f8-110">Você pode usar a operação [Atualizar aplicativo](../api/application-update.md) para executar uma atualização.</span><span class="sxs-lookup"><span data-stu-id="822f8-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="822f8-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="822f8-111">Permissions</span></span>

|<span data-ttu-id="822f8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="822f8-112">Permission type</span></span>      | <span data-ttu-id="822f8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="822f8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="822f8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="822f8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="822f8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="822f8-115">None.</span></span>  |
|<span data-ttu-id="822f8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="822f8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="822f8-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="822f8-117">None.</span></span>    |
|<span data-ttu-id="822f8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="822f8-118">Application</span></span> | <span data-ttu-id="822f8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="822f8-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="822f8-120">Um aplicativo não precisa de nenhuma permissão específica para rolar suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="822f8-120">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="822f8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="822f8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="822f8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="822f8-122">Request headers</span></span>

| <span data-ttu-id="822f8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="822f8-123">Name</span></span>           | <span data-ttu-id="822f8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="822f8-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="822f8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="822f8-125">Authorization</span></span>  | <span data-ttu-id="822f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="822f8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="822f8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="822f8-128">Content-Type</span></span>   | <span data-ttu-id="822f8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="822f8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="822f8-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="822f8-131">Request body</span></span>

<span data-ttu-id="822f8-132">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="822f8-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="822f8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="822f8-133">Property</span></span>     | <span data-ttu-id="822f8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="822f8-134">Type</span></span>   |<span data-ttu-id="822f8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="822f8-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="822f8-136">keycredential</span><span class="sxs-lookup"><span data-stu-id="822f8-136">keyCredential</span></span> | [<span data-ttu-id="822f8-137">keycredential</span><span class="sxs-lookup"><span data-stu-id="822f8-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="822f8-138">A nova credencial de chave de aplicativo a ser adicionada.</span><span class="sxs-lookup"><span data-stu-id="822f8-138">The new application key credential to add.</span></span> <span data-ttu-id="822f8-139">O __tipo__, __uso__ e __chave__ são propriedades obrigatórias para esse uso.</span><span class="sxs-lookup"><span data-stu-id="822f8-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="822f8-140">Os tipos de chave com suporte são:</span><span class="sxs-lookup"><span data-stu-id="822f8-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="822f8-141">`AsymmetricX509Cert`: O uso deve ser `Verify` .</span><span class="sxs-lookup"><span data-stu-id="822f8-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="822f8-142">`X509CertAndPassword`: O uso deve ser`Sign`</span><span class="sxs-lookup"><span data-stu-id="822f8-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="822f8-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="822f8-143">passwordCredential</span></span> | [<span data-ttu-id="822f8-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="822f8-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="822f8-145">Só é necessário definir o __secretText__ que deve conter a senha para a chave.</span><span class="sxs-lookup"><span data-stu-id="822f8-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="822f8-146">Essa propriedade é obrigatória somente para chaves de tipo `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="822f8-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="822f8-147">Defini-lo como `null` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="822f8-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="822f8-148">evidência</span><span class="sxs-lookup"><span data-stu-id="822f8-148">proof</span></span> | <span data-ttu-id="822f8-149">String</span><span class="sxs-lookup"><span data-stu-id="822f8-149">String</span></span> | <span data-ttu-id="822f8-150">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="822f8-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="822f8-151">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="822f8-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="822f8-152">O token deve conter as seguintes declarações:</span><span class="sxs-lookup"><span data-stu-id="822f8-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="822f8-153">`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="822f8-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="822f8-154">`iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="822f8-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="822f8-155">`nbf`-Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="822f8-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="822f8-156">`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="822f8-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="822f8-157">Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.</span><span class="sxs-lookup"><span data-stu-id="822f8-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="822f8-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="822f8-158">Response</span></span>

<span data-ttu-id="822f8-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [keycredential](../resources/keycredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="822f8-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="822f8-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="822f8-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="822f8-161">Exemplo 1: adicionar uma nova credencial de chave a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="822f8-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="822f8-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="822f8-162">Request</span></span>

<span data-ttu-id="822f8-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="822f8-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="822f8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="822f8-164">Response</span></span>

<span data-ttu-id="822f8-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="822f8-165">The following is an example of the response.</span></span>

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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="822f8-166">Exemplo 2: adicionar uma credencial de chave e uma senha associada para a chave</span><span class="sxs-lookup"><span data-stu-id="822f8-166">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="822f8-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="822f8-167">Request</span></span>

<span data-ttu-id="822f8-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="822f8-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="822f8-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="822f8-169">Response</span></span>

<span data-ttu-id="822f8-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="822f8-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
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
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
