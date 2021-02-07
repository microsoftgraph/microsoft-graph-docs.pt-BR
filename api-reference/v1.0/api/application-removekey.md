---
title: 'application: removeKey'
description: Remover uma credencial de chave de um aplicativo
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f2b2dfcc25fa7dfd88173572b71e9c52e580c5b6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131450"
---
# <a name="application-removekey"></a><span data-ttu-id="d3b5f-103">application: removeKey</span><span class="sxs-lookup"><span data-stu-id="d3b5f-103">application: removeKey</span></span>

<span data-ttu-id="d3b5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3b5f-105">Remova uma credencial de chave de um [aplicativo.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="d3b5f-105">Remove a key credential from an [application](../resources/application.md).</span></span> <span data-ttu-id="d3b5f-106">Esse método, [juntamente com addKey,](application-addkey.md) pode ser usado por um aplicativo para automatizar a rolagem de suas chaves expiradas.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-106">This method along with [addKey](application-addkey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="d3b5f-107">[Criar operações servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Update servicePrincipal](../api/serviceprincipal-update.md) podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer aplicativo com aplicativo ou contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any application with application or a user's context.</span></span>

<span data-ttu-id="d3b5f-108">Como parte da validação da solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3b5f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3b5f-109">Permissions</span></span>

|<span data-ttu-id="d3b5f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3b5f-110">Permission type</span></span>      | <span data-ttu-id="d3b5f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3b5f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3b5f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3b5f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3b5f-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-113">None.</span></span>  |
|<span data-ttu-id="d3b5f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3b5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3b5f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-115">None.</span></span>    |
|<span data-ttu-id="d3b5f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3b5f-116">Application</span></span> | <span data-ttu-id="d3b5f-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-117">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="d3b5f-118">Um aplicativo não precisa de nenhuma permissão específica para rolar suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-118">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="d3b5f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3b5f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="d3b5f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b5f-120">Request headers</span></span>

| <span data-ttu-id="d3b5f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d3b5f-121">Name</span></span>           | <span data-ttu-id="d3b5f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b5f-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d3b5f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3b5f-123">Authorization</span></span>  | <span data-ttu-id="d3b5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3b5f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3b5f-126">Content-Type</span></span>   | <span data-ttu-id="d3b5f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3b5f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b5f-129">Request body</span></span>

<span data-ttu-id="d3b5f-130">No corpo da solicitação, forneça as seguintes propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="d3b5f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3b5f-131">Property</span></span>  | <span data-ttu-id="d3b5f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3b5f-132">Type</span></span> | <span data-ttu-id="d3b5f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b5f-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="d3b5f-134">keyId</span><span class="sxs-lookup"><span data-stu-id="d3b5f-134">keyId</span></span>     | <span data-ttu-id="d3b5f-135">GUID</span><span class="sxs-lookup"><span data-stu-id="d3b5f-135">GUID</span></span> | <span data-ttu-id="d3b5f-136">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="d3b5f-137">proof</span><span class="sxs-lookup"><span data-stu-id="d3b5f-137">proof</span></span> | <span data-ttu-id="d3b5f-138">String</span><span class="sxs-lookup"><span data-stu-id="d3b5f-138">String</span></span> | <span data-ttu-id="d3b5f-139">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="d3b5f-140">Esse token de JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-140">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="d3b5f-141">O token deve conter os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="d3b5f-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="d3b5f-142">`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="d3b5f-143">`iss` - O emissor deve ser o __ID__ do aplicativo que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-143">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="d3b5f-144">`nbf` – Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="d3b5f-145">`exp` – O tempo de expiração deve ser "nbf" + 10 min.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="d3b5f-146">Aqui está um exemplo [de código](/graph/application-rollkey-prooftoken) que pode ser usado para gerar esse token de comprovação de posse.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="d3b5f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3b5f-147">Response</span></span>

<span data-ttu-id="d3b5f-148">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d3b5f-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3b5f-149">Examples</span></span>

<span data-ttu-id="d3b5f-150">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-150">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d3b5f-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b5f-151">Request</span></span>

<span data-ttu-id="d3b5f-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3b5f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3b5f-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d3b5f-154">C#</span><span class="sxs-lookup"><span data-stu-id="d3b5f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3b5f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3b5f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3b5f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3b5f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3b5f-157">Java</span><span class="sxs-lookup"><span data-stu-id="d3b5f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3b5f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3b5f-158">Response</span></span>

<span data-ttu-id="d3b5f-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3b5f-159">The following is an example of the response.</span></span>

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

