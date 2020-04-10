---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: Carregar uma chave PKCS 12 Format (PFX) em um conjunto de chaves.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d5b2d2c10194156a1b577437d1e7a90773b80a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219008"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="1ef5a-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="1ef5a-103">trustFrameworkKeySet: uploadPkcs12</span></span>

<span data-ttu-id="1ef5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef5a-105">Carregar uma chave do formato PKCS12 (PFX) para um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="1ef5a-105">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="1ef5a-106">A entrada é um valor codificado de base 64 do conteúdo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-106">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="1ef5a-107">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="1ef5a-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef5a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ef5a-108">Permissions</span></span>

<span data-ttu-id="1ef5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ef5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ef5a-111">Permission type</span></span>                        | <span data-ttu-id="1ef5a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ef5a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ef5a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ef5a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ef5a-114">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1ef5a-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="1ef5a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ef5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-116">Not supported.</span></span> |
| <span data-ttu-id="1ef5a-117">Application</span><span class="sxs-lookup"><span data-stu-id="1ef5a-117">Application</span></span>                            | <span data-ttu-id="1ef5a-118">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1ef5a-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ef5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ef5a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="1ef5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef5a-120">Request headers</span></span>

| <span data-ttu-id="1ef5a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1ef5a-121">Name</span></span>          | <span data-ttu-id="1ef5a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef5a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1ef5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ef5a-123">Authorization</span></span> | <span data-ttu-id="1ef5a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ef5a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1ef5a-126">Content-type</span></span>  | <span data-ttu-id="1ef5a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ef5a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef5a-129">Request body</span></span>

<span data-ttu-id="1ef5a-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1ef5a-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1ef5a-131">Parameter</span></span>    | <span data-ttu-id="1ef5a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ef5a-132">Type</span></span>        | <span data-ttu-id="1ef5a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef5a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ef5a-134">key</span><span class="sxs-lookup"><span data-stu-id="1ef5a-134">key</span></span>|<span data-ttu-id="1ef5a-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1ef5a-135">String</span></span>|<span data-ttu-id="1ef5a-136">Este é o campo para enviar conteúdo de PFX.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-136">This is the field for sending pfx content.</span></span> <span data-ttu-id="1ef5a-137">O valor deve ser uma versão de codificação de base 64 do conteúdo de certificado real.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-137">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="1ef5a-138">password</span><span class="sxs-lookup"><span data-stu-id="1ef5a-138">password</span></span>|<span data-ttu-id="1ef5a-139">String</span><span class="sxs-lookup"><span data-stu-id="1ef5a-139">String</span></span>|<span data-ttu-id="1ef5a-140">Este é o campo para enviar a senha para o conteúdo de PFX.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-140">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="1ef5a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ef5a-141">Response</span></span>

<span data-ttu-id="1ef5a-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-142">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ef5a-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1ef5a-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ef5a-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef5a-144">Request</span></span>

<span data-ttu-id="1ef5a-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ef5a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ef5a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1ef5a-147">C#</span><span class="sxs-lookup"><span data-stu-id="1ef5a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ef5a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ef5a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ef5a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ef5a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ef5a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ef5a-150">Response</span></span>

<span data-ttu-id="1ef5a-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-151">The following is an example of the response.</span></span>

> <span data-ttu-id="1ef5a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ef5a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "sig",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
