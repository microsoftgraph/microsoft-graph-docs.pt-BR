---
title: 'trustFrameworkKeySet: uploadCertificate'
description: Carregar um certificado em um conjunto de chaves.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 726e2d98ca1002f9e3a9e3d8a7bf705550767529
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937501"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="6730a-103">trustFrameworkKeySet: uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="6730a-103">trustFrameworkKeySet: uploadCertificate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6730a-104">Carregar um certificado em um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="6730a-104">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="6730a-105">A entrada é um valor codificado em base 64 do conteúdo do certificado.</span><span class="sxs-lookup"><span data-stu-id="6730a-105">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="6730a-106">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="6730a-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6730a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6730a-107">Permissions</span></span>

<span data-ttu-id="6730a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6730a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6730a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6730a-110">Permission type</span></span>                        | <span data-ttu-id="6730a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6730a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6730a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6730a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6730a-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6730a-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="6730a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6730a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6730a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6730a-115">Not supported.</span></span> |
| <span data-ttu-id="6730a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6730a-116">Application</span></span>                            | <span data-ttu-id="6730a-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6730a-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6730a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6730a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="6730a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6730a-119">Request headers</span></span>

| <span data-ttu-id="6730a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6730a-120">Name</span></span>          | <span data-ttu-id="6730a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6730a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6730a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6730a-122">Authorization</span></span> | <span data-ttu-id="6730a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6730a-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6730a-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="6730a-125">Content-type</span></span> | <span data-ttu-id="6730a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6730a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6730a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6730a-128">Request body</span></span>

<span data-ttu-id="6730a-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6730a-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6730a-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6730a-130">Parameter</span></span>    | <span data-ttu-id="6730a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6730a-131">Type</span></span>        | <span data-ttu-id="6730a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6730a-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6730a-133">key</span><span class="sxs-lookup"><span data-stu-id="6730a-133">key</span></span>|<span data-ttu-id="6730a-134">String</span><span class="sxs-lookup"><span data-stu-id="6730a-134">String</span></span>| <span data-ttu-id="6730a-135">Este é o campo para enviar conteúdo de certificado.</span><span class="sxs-lookup"><span data-stu-id="6730a-135">This is the field for sending certificate content.</span></span> <span data-ttu-id="6730a-136">O valor deve ser uma versão de codificação de base 64 do conteúdo de certificado real.</span><span class="sxs-lookup"><span data-stu-id="6730a-136">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="6730a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6730a-137">Response</span></span>

<span data-ttu-id="6730a-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6730a-138">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6730a-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6730a-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6730a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6730a-140">Request</span></span>

<span data-ttu-id="6730a-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6730a-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6730a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6730a-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6730a-143">C#</span><span class="sxs-lookup"><span data-stu-id="6730a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6730a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6730a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6730a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6730a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6730a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6730a-146">Response</span></span>

<span data-ttu-id="6730a-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6730a-147">The following is an example of the response.</span></span>

> <span data-ttu-id="6730a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6730a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
