---
title: Tipo de recurso trustFrameworkKey
description: Representa um JWK (JSON Web Key). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica. A estrutura desse recurso segue o formato definido na RFC 7517 Seção 4.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b50e82748db6c0c26252ce6b79290781fa88819b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945631"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="2551d-105">Tipo de recurso trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="2551d-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="2551d-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2551d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2551d-107">Representa um JWK (JSON Web Key).</span><span class="sxs-lookup"><span data-stu-id="2551d-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="2551d-108">TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica.</span><span class="sxs-lookup"><span data-stu-id="2551d-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="2551d-109">A estrutura desse recurso segue o formato definido na [RFC 7517 Seção 4](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="2551d-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="2551d-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2551d-110">Properties</span></span>

| <span data-ttu-id="2551d-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2551d-111">Property</span></span>     | <span data-ttu-id="2551d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2551d-112">Type</span></span>        | <span data-ttu-id="2551d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2551d-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2551d-114">kid</span><span class="sxs-lookup"><span data-stu-id="2551d-114">kid</span></span> | <span data-ttu-id="2551d-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-115">string</span></span> | <span data-ttu-id="2551d-116">O identificador exclusivo da chave.</span><span class="sxs-lookup"><span data-stu-id="2551d-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="2551d-117">kty</span><span class="sxs-lookup"><span data-stu-id="2551d-117">kty</span></span> | <span data-ttu-id="2551d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-118">String</span></span> | <span data-ttu-id="2551d-119">O **parâmetro kty** (tipo de chave) identifica a família de algoritmos criptográficos usados com a chave, Os valores válidos são `rsa` , `oct` .</span><span class="sxs-lookup"><span data-stu-id="2551d-119">The **kty** (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are `rsa`, `oct`.</span></span> |
| <span data-ttu-id="2551d-120">use</span><span class="sxs-lookup"><span data-stu-id="2551d-120">use</span></span> | <span data-ttu-id="2551d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-121">String</span></span> | <span data-ttu-id="2551d-122">O **parâmetro use** (uso de chave pública) identifica o uso pretendido da chave pública.</span><span class="sxs-lookup"><span data-stu-id="2551d-122">The **use** (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="2551d-123">O **parâmetro** use é empregado para indicar se uma chave pública é usada para criptografar dados ou verificar a assinatura em dados.</span><span class="sxs-lookup"><span data-stu-id="2551d-123">The **use** parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="2551d-124">Os valores possíveis são: `sig` (assinatura), `enc` (criptografia)</span><span class="sxs-lookup"><span data-stu-id="2551d-124">Possible values are: `sig` (signature), `enc` (encryption)</span></span>  |
| <span data-ttu-id="2551d-125">x5c</span><span class="sxs-lookup"><span data-stu-id="2551d-125">x5c</span></span> | <span data-ttu-id="2551d-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-126">string collection</span></span> | <span data-ttu-id="2551d-127">O **parâmetro x5c** (cadeia de certificados X.509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="2551d-127">The **x5c** (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="2551d-128">x5t</span><span class="sxs-lookup"><span data-stu-id="2551d-128">x5t</span></span> | <span data-ttu-id="2551d-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-129">string</span></span> | <span data-ttu-id="2551d-130">O **parâmetro x5t** (X.509 certificate SHA-1 thumbprint) é uma impressão digital SHA-1 codificada com base64url (a.k.a.</span><span class="sxs-lookup"><span data-stu-id="2551d-130">The **x5t** (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="2551d-131">digest) da codificação DER de um certificado X.509 [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="2551d-131">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="2551d-132">e</span><span class="sxs-lookup"><span data-stu-id="2551d-132">e</span></span> | <span data-ttu-id="2551d-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-133">string</span></span> | <span data-ttu-id="2551d-134">CHAVE RSA - expoente público</span><span class="sxs-lookup"><span data-stu-id="2551d-134">RSA Key - public exponent</span></span> |
| <span data-ttu-id="2551d-135">d</span><span class="sxs-lookup"><span data-stu-id="2551d-135">d</span></span>| <span data-ttu-id="2551d-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-136">string</span></span> | <span data-ttu-id="2551d-137">CHAVE RSA - expoente particular.</span><span class="sxs-lookup"><span data-stu-id="2551d-137">RSA Key - private exponent.</span></span> <span data-ttu-id="2551d-138">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-138">Field cannot be read back.</span></span> |
| <span data-ttu-id="2551d-139">n</span><span class="sxs-lookup"><span data-stu-id="2551d-139">n</span></span> | <span data-ttu-id="2551d-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-140">string</span></span> | <span data-ttu-id="2551d-141">Chave RSA - módulo</span><span class="sxs-lookup"><span data-stu-id="2551d-141">RSA Key - modulus</span></span> |
| <span data-ttu-id="2551d-142">p</span><span class="sxs-lookup"><span data-stu-id="2551d-142">p</span></span> | <span data-ttu-id="2551d-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-143">string</span></span> | <span data-ttu-id="2551d-144">Chave RSA - primeiro prime.</span><span class="sxs-lookup"><span data-stu-id="2551d-144">RSA Key - first prime.</span></span> <span data-ttu-id="2551d-145">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-145">Field cannot be read back.</span></span> |
| <span data-ttu-id="2551d-146">q</span><span class="sxs-lookup"><span data-stu-id="2551d-146">q</span></span> | <span data-ttu-id="2551d-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-147">string</span></span> | <span data-ttu-id="2551d-148">CHAVE RSA - segundo prime.</span><span class="sxs-lookup"><span data-stu-id="2551d-148">RSA Key - second prime.</span></span> <span data-ttu-id="2551d-149">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-149">Field cannot be read back.</span></span> |
| <span data-ttu-id="2551d-150">dp</span><span class="sxs-lookup"><span data-stu-id="2551d-150">dp</span></span> | <span data-ttu-id="2551d-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-151">string</span></span> | <span data-ttu-id="2551d-152">Chave RSA - primeiro expoente.</span><span class="sxs-lookup"><span data-stu-id="2551d-152">RSA Key - first exponent.</span></span> <span data-ttu-id="2551d-153">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-153">Field cannot be read back.</span></span> |
| <span data-ttu-id="2551d-154">dq</span><span class="sxs-lookup"><span data-stu-id="2551d-154">dq</span></span> | <span data-ttu-id="2551d-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-155">string</span></span> | <span data-ttu-id="2551d-156">Chave RSA - segundo expoente.</span><span class="sxs-lookup"><span data-stu-id="2551d-156">RSA Key - second exponent.</span></span> <span data-ttu-id="2551d-157">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-157">Field cannot be read back.</span></span> |
| <span data-ttu-id="2551d-158">qi</span><span class="sxs-lookup"><span data-stu-id="2551d-158">qi</span></span> | <span data-ttu-id="2551d-159">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-159">string</span></span> | <span data-ttu-id="2551d-160">Chave RSA - Coeficiente.</span><span class="sxs-lookup"><span data-stu-id="2551d-160">RSA Key - Coefficient.</span></span> <span data-ttu-id="2551d-161">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-161">Field cannot be read back.</span></span> |
| <span data-ttu-id="2551d-162">k</span><span class="sxs-lookup"><span data-stu-id="2551d-162">k</span></span> | <span data-ttu-id="2551d-163">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2551d-163">string</span></span> | <span data-ttu-id="2551d-164">Chave Simétrica para o tipo de chave de oct.</span><span class="sxs-lookup"><span data-stu-id="2551d-164">Symmetric Key for oct key type.</span></span> <span data-ttu-id="2551d-165">O campo não pode ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="2551d-165">Field cannot be read back.</span></span>   |
| <span data-ttu-id="2551d-166">nbf</span><span class="sxs-lookup"><span data-stu-id="2551d-166">nbf</span></span> | <span data-ttu-id="2551d-167">int</span><span class="sxs-lookup"><span data-stu-id="2551d-167">int</span></span> | <span data-ttu-id="2551d-168">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="2551d-168">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="2551d-169">exp</span><span class="sxs-lookup"><span data-stu-id="2551d-169">exp</span></span> | <span data-ttu-id="2551d-170">int</span><span class="sxs-lookup"><span data-stu-id="2551d-170">int</span></span> | <span data-ttu-id="2551d-171">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="2551d-171">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="2551d-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2551d-172">JSON representation</span></span>

<span data-ttu-id="2551d-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2551d-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKey",
  "baseType": null
}-->

```json
{
  "d": "String",
  "dp": "String",
  "dq": "String",
  "e": "String",
  "exp": 1024,
  "k": "String",
  "kid": "String",
  "kty": "String",
  "n": "String",
  "nbf": 1024,
  "p": "String",
  "q": "String",
  "qi": "String",
  "use": "String",
  "x5c": ["String"],
  "x5t": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKey resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


