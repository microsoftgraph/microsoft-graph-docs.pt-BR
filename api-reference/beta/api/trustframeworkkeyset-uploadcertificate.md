---
title: 'trustFrameworkKeySet: uploadCertificate'
description: Carregar um certificado em um conjunto de chaves.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0342565ca8c7e652118c525a3c51c4700840d718
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215893"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="5b629-103">trustFrameworkKeySet: uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="5b629-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="5b629-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b629-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b629-105">Carregar um certificado em um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="5b629-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="5b629-106">A entrada é um valor codificado em base 64 do conteúdo do certificado.</span><span class="sxs-lookup"><span data-stu-id="5b629-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="5b629-107">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="5b629-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b629-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b629-108">Permissions</span></span>

<span data-ttu-id="5b629-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b629-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b629-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b629-111">Permission type</span></span>                        | <span data-ttu-id="5b629-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b629-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b629-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b629-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b629-114">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5b629-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="5b629-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b629-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b629-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b629-116">Not supported.</span></span> |
| <span data-ttu-id="5b629-117">Application</span><span class="sxs-lookup"><span data-stu-id="5b629-117">Application</span></span>                            | <span data-ttu-id="5b629-118">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5b629-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b629-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b629-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="5b629-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b629-120">Request headers</span></span>

| <span data-ttu-id="5b629-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5b629-121">Name</span></span>          | <span data-ttu-id="5b629-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b629-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5b629-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b629-123">Authorization</span></span> | <span data-ttu-id="5b629-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b629-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5b629-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="5b629-126">Content-type</span></span> | <span data-ttu-id="5b629-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b629-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b629-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b629-129">Request body</span></span>

<span data-ttu-id="5b629-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b629-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b629-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5b629-131">Parameter</span></span>    | <span data-ttu-id="5b629-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b629-132">Type</span></span>        | <span data-ttu-id="5b629-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b629-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b629-134">key</span><span class="sxs-lookup"><span data-stu-id="5b629-134">key</span></span>|<span data-ttu-id="5b629-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="5b629-135">String</span></span>| <span data-ttu-id="5b629-136">Este é o campo para enviar conteúdo de certificado.</span><span class="sxs-lookup"><span data-stu-id="5b629-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="5b629-137">O valor deve ser uma versão de codificação de base 64 do conteúdo de certificado real.</span><span class="sxs-lookup"><span data-stu-id="5b629-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="5b629-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b629-138">Response</span></span>

<span data-ttu-id="5b629-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b629-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b629-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b629-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b629-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b629-141">Request</span></span>

<span data-ttu-id="5b629-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b629-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b629-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b629-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadCertificate
Content-type: application/json

{
  "key": "key-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5b629-144">C#</span><span class="sxs-lookup"><span data-stu-id="5b629-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b629-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b629-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b629-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b629-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b629-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b629-147">Response</span></span>

<span data-ttu-id="5b629-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b629-148">The following is an example of the response.</span></span>

> <span data-ttu-id="5b629-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b629-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "kty": "oct",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
