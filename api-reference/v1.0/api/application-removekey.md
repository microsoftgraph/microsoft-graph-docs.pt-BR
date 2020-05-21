---
title: 'aplicativo: removeKey'
description: Remover uma credencial de chave de um aplicativo
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a366da38cafd83c715f31f61ec01ecdcc6b7da1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334687"
---
# <a name="application-removekey"></a><span data-ttu-id="18c93-103">aplicativo: removeKey</span><span class="sxs-lookup"><span data-stu-id="18c93-103">application: removeKey</span></span>

<span data-ttu-id="18c93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18c93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18c93-105">Remover uma credencial de chave de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="18c93-105">Remove a key credential from an [application](../resources/application.md).</span></span> <span data-ttu-id="18c93-106">Este método junto com o [addKey](application-addkey.md) pode ser usado por um aplicativo para automatizar a interrupção de suas chaves de expiração.</span><span class="sxs-lookup"><span data-stu-id="18c93-106">This method along with [addKey](application-addkey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="18c93-107">[Criar o servicePrincipalName](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar](../api/serviceprincipal-update.md) as operações do servicePrincipalName podem continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer aplicativo com o aplicativo ou o contexto de um usuário.</span><span class="sxs-lookup"><span data-stu-id="18c93-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any application with application or a user's context.</span></span>

<span data-ttu-id="18c93-108">Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="18c93-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="18c93-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="18c93-109">Permissions</span></span>

|<span data-ttu-id="18c93-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18c93-110">Permission type</span></span>      | <span data-ttu-id="18c93-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18c93-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18c93-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18c93-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18c93-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18c93-113">None.</span></span>  |
|<span data-ttu-id="18c93-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18c93-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18c93-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="18c93-115">None.</span></span>    |
|<span data-ttu-id="18c93-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18c93-116">Application</span></span> | <span data-ttu-id="18c93-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18c93-117">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="18c93-118">Um aplicativo não precisa de nenhuma permissão específica para rolar suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="18c93-118">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="18c93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18c93-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="18c93-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18c93-120">Request headers</span></span>

| <span data-ttu-id="18c93-121">Nome</span><span class="sxs-lookup"><span data-stu-id="18c93-121">Name</span></span>           | <span data-ttu-id="18c93-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="18c93-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="18c93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18c93-123">Authorization</span></span>  | <span data-ttu-id="18c93-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18c93-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18c93-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18c93-126">Content-Type</span></span>   | <span data-ttu-id="18c93-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18c93-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18c93-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18c93-129">Request body</span></span>

<span data-ttu-id="18c93-130">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="18c93-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="18c93-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18c93-131">Property</span></span>  | <span data-ttu-id="18c93-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="18c93-132">Type</span></span> | <span data-ttu-id="18c93-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="18c93-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="18c93-134">keyId</span><span class="sxs-lookup"><span data-stu-id="18c93-134">keyId</span></span>     | <span data-ttu-id="18c93-135">GUID</span><span class="sxs-lookup"><span data-stu-id="18c93-135">GUID</span></span> | <span data-ttu-id="18c93-136">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="18c93-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="18c93-137">evidência</span><span class="sxs-lookup"><span data-stu-id="18c93-137">proof</span></span> | <span data-ttu-id="18c93-138">String</span><span class="sxs-lookup"><span data-stu-id="18c93-138">String</span></span> | <span data-ttu-id="18c93-139">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="18c93-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="18c93-140">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18c93-140">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="18c93-141">O token deve conter as seguintes declarações:</span><span class="sxs-lookup"><span data-stu-id="18c93-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="18c93-142">`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="18c93-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="18c93-143">`iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="18c93-143">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="18c93-144">`nbf`-Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="18c93-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="18c93-145">`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="18c93-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="18c93-146">Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.</span><span class="sxs-lookup"><span data-stu-id="18c93-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="18c93-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="18c93-147">Response</span></span>

<span data-ttu-id="18c93-148">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="18c93-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="18c93-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18c93-149">Examples</span></span>

<span data-ttu-id="18c93-150">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="18c93-150">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="18c93-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18c93-151">Request</span></span>

<span data-ttu-id="18c93-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18c93-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="18c93-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="18c93-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removekey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="18c93-154">C#</span><span class="sxs-lookup"><span data-stu-id="18c93-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18c93-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18c93-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18c93-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18c93-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18c93-157">Java</span><span class="sxs-lookup"><span data-stu-id="18c93-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18c93-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="18c93-158">Response</span></span>

<span data-ttu-id="18c93-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18c93-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
