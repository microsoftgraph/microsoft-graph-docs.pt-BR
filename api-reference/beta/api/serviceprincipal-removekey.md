---
title: 'servicePrincipalName: removeKey'
description: Remover uma credencial de chave de um servicePrincipalName
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 932ec0fa86b377f3614cd5e986b6d99935d27369
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076691"
---
# <a name="serviceprincipal-removekey"></a><span data-ttu-id="0b626-103">servicePrincipalName: removeKey</span><span class="sxs-lookup"><span data-stu-id="0b626-103">servicePrincipal: removeKey</span></span>

<span data-ttu-id="0b626-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b626-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b626-105">Remover uma credencial de chave de um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0b626-105">Remove a key credential from a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="0b626-106">Este método junto com o [addKey](serviceprincipal-addkey.md) pode ser usado por um servicePrincipalName para automatizar as chaves de expiração.</span><span class="sxs-lookup"><span data-stu-id="0b626-106">This method along with [addKey](serviceprincipal-addkey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="0b626-107">[Criar o servicePrincipalName](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar](../api/serviceprincipal-update.md) as operações do servicePrincipalName podem continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer servicePrincipalName com ou sem o contexto de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0b626-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="0b626-108">Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.</span><span class="sxs-lookup"><span data-stu-id="0b626-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b626-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b626-109">Permissions</span></span>

|<span data-ttu-id="0b626-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b626-110">Permission type</span></span>      | <span data-ttu-id="0b626-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b626-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b626-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b626-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b626-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b626-113">None.</span></span>  |
|<span data-ttu-id="0b626-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b626-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b626-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b626-115">None.</span></span>    |
|<span data-ttu-id="0b626-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b626-116">Application</span></span> | <span data-ttu-id="0b626-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b626-117">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="0b626-118">Um servicePrincipalName não precisa de nenhuma permissão específica para a distribuição de suas próprias chaves.</span><span class="sxs-lookup"><span data-stu-id="0b626-118">A servicePrincipal does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b626-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b626-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="0b626-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b626-120">Request headers</span></span>

| <span data-ttu-id="0b626-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0b626-121">Name</span></span>           | <span data-ttu-id="0b626-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b626-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0b626-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b626-123">Authorization</span></span>  | <span data-ttu-id="0b626-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b626-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0b626-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b626-126">Content-Type</span></span>   | <span data-ttu-id="0b626-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b626-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b626-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b626-129">Request body</span></span>

<span data-ttu-id="0b626-130">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="0b626-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="0b626-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b626-131">Property</span></span>  | <span data-ttu-id="0b626-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b626-132">Type</span></span> | <span data-ttu-id="0b626-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b626-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="0b626-134">keyId</span><span class="sxs-lookup"><span data-stu-id="0b626-134">keyId</span></span>     | <span data-ttu-id="0b626-135">GUID</span><span class="sxs-lookup"><span data-stu-id="0b626-135">GUID</span></span> | <span data-ttu-id="0b626-136">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="0b626-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="0b626-137">evidência</span><span class="sxs-lookup"><span data-stu-id="0b626-137">proof</span></span> | <span data-ttu-id="0b626-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b626-138">String</span></span> | <span data-ttu-id="0b626-139">Um token JWT auto-assinado usado como prova de posse das chaves existentes.</span><span class="sxs-lookup"><span data-stu-id="0b626-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="0b626-140">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes de servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0b626-140">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="0b626-141">O token deve conter os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="0b626-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="0b626-142">`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="0b626-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="0b626-143">`iss` -Issuer precisa ser a __ID__  do servicePrincipalName que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="0b626-143">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="0b626-144">`nbf` – Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="0b626-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="0b626-145">`exp` – O tempo de expiração deve ser "nbf" + 10 min.</span><span class="sxs-lookup"><span data-stu-id="0b626-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="0b626-146">Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.</span><span class="sxs-lookup"><span data-stu-id="0b626-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="0b626-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b626-147">Response</span></span>

<span data-ttu-id="0b626-148">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="0b626-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0b626-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0b626-149">Examples</span></span>

<span data-ttu-id="0b626-150">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="0b626-150">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0b626-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b626-151">Request</span></span>

<span data-ttu-id="0b626-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b626-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b626-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b626-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="javascript"></a>[<span data-ttu-id="0b626-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b626-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b626-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b626-155">Response</span></span>

<span data-ttu-id="0b626-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b626-156">The following is an example of the response.</span></span>

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
  "description": "servicePrincipal: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


