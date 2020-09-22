---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: Carregar uma chave PKCS 12 Format (PFX) em um conjunto de chaves.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a657b7bf8ca90236649647d8a1d4d054134e2c95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027263"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="f0c6c-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="f0c6c-103">trustFrameworkKeySet: uploadPkcs12</span></span>

<span data-ttu-id="f0c6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0c6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c6c-105">Carregar uma chave do formato PKCS12 (PFX) para um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="f0c6c-105">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="f0c6c-106">A entrada é um valor codificado de base 64 do conteúdo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-106">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="f0c6c-107">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="f0c6c-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0c6c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0c6c-108">Permissions</span></span>

<span data-ttu-id="f0c6c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0c6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0c6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0c6c-111">Permission type</span></span>                        | <span data-ttu-id="f0c6c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0c6c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0c6c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0c6c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0c6c-114">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f0c6c-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="f0c6c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0c6c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0c6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-116">Not supported.</span></span> |
| <span data-ttu-id="f0c6c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0c6c-117">Application</span></span>                            | <span data-ttu-id="f0c6c-118">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f0c6c-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0c6c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c6c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="f0c6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c6c-120">Request headers</span></span>

| <span data-ttu-id="f0c6c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f0c6c-121">Name</span></span>          | <span data-ttu-id="f0c6c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c6c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f0c6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0c6c-123">Authorization</span></span> | <span data-ttu-id="f0c6c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0c6c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f0c6c-126">Content-type</span></span>  | <span data-ttu-id="f0c6c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0c6c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c6c-129">Request body</span></span>

<span data-ttu-id="f0c6c-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0c6c-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0c6c-131">Parameter</span></span>    | <span data-ttu-id="f0c6c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0c6c-132">Type</span></span>        | <span data-ttu-id="f0c6c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c6c-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0c6c-134">key</span><span class="sxs-lookup"><span data-stu-id="f0c6c-134">key</span></span>|<span data-ttu-id="f0c6c-135">String</span><span class="sxs-lookup"><span data-stu-id="f0c6c-135">String</span></span>|<span data-ttu-id="f0c6c-136">Este é o campo para enviar conteúdo de PFX.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-136">This is the field for sending pfx content.</span></span> <span data-ttu-id="f0c6c-137">O valor deve ser uma versão de codificação de base 64 do conteúdo de certificado real.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-137">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="f0c6c-138">password</span><span class="sxs-lookup"><span data-stu-id="f0c6c-138">password</span></span>|<span data-ttu-id="f0c6c-139">String</span><span class="sxs-lookup"><span data-stu-id="f0c6c-139">String</span></span>|<span data-ttu-id="f0c6c-140">Este é o campo para enviar a senha para o conteúdo de PFX.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-140">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="f0c6c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c6c-141">Response</span></span>

<span data-ttu-id="f0c6c-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-142">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0c6c-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0c6c-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0c6c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c6c-144">Request</span></span>

<span data-ttu-id="f0c6c-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0c6c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c6c-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f0c6c-147">C#</span><span class="sxs-lookup"><span data-stu-id="f0c6c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0c6c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0c6c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0c6c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0c6c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0c6c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c6c-150">Response</span></span>

<span data-ttu-id="f0c6c-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-151">The following is an example of the response.</span></span>

> <span data-ttu-id="f0c6c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0c6c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


