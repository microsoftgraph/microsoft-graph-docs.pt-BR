---
title: tipo de recurso trustFrameworkKey
description: Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia. A estrutura desse recurso segue o formato definido na RFC 7517 seção 4.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7650976a437eb862acd5994d7e1dd14830d5e3b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083929"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="d6539-105">tipo de recurso trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="d6539-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="d6539-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6539-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6539-107">Representa um JWK (chave Web JSON).</span><span class="sxs-lookup"><span data-stu-id="d6539-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="d6539-108">TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia.</span><span class="sxs-lookup"><span data-stu-id="d6539-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="d6539-109">A estrutura desse recurso segue o formato definido na [RFC 7517 seção 4](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="d6539-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="d6539-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6539-110">Properties</span></span>

| <span data-ttu-id="d6539-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6539-111">Property</span></span>     | <span data-ttu-id="d6539-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6539-112">Type</span></span>        | <span data-ttu-id="d6539-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6539-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d6539-114">filho</span><span class="sxs-lookup"><span data-stu-id="d6539-114">kid</span></span> | <span data-ttu-id="d6539-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-115">string</span></span> | <span data-ttu-id="d6539-116">O identificador exclusivo da chave.</span><span class="sxs-lookup"><span data-stu-id="d6539-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="d6539-117">kty</span><span class="sxs-lookup"><span data-stu-id="d6539-117">kty</span></span> | <span data-ttu-id="d6539-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-118">string</span></span> | <span data-ttu-id="d6539-119">O parâmetro "KTY" (tipo de chave) identifica a família de algoritmos de criptografia usada com a chave, os valores válidos são RSA, Oct.</span><span class="sxs-lookup"><span data-stu-id="d6539-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="d6539-120">Use</span><span class="sxs-lookup"><span data-stu-id="d6539-120">use</span></span> | <span data-ttu-id="d6539-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-121">string</span></span> | <span data-ttu-id="d6539-122">O parâmetro "Use" (uso de chave pública) identifica o uso pretendido da chave pública.</span><span class="sxs-lookup"><span data-stu-id="d6539-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="d6539-123">O parâmetro "Use" é empregado para indicar se uma chave pública é usada para criptografar os dados ou para verificar a assinatura dos dados.</span><span class="sxs-lookup"><span data-stu-id="d6539-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="d6539-124">Os valores possíveis são 1.</span><span class="sxs-lookup"><span data-stu-id="d6539-124">Possible values are    1.</span></span> <span data-ttu-id="d6539-125">"SIG" (assinatura) 2.</span><span class="sxs-lookup"><span data-stu-id="d6539-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="d6539-126">"Enc" (criptografia)</span><span class="sxs-lookup"><span data-stu-id="d6539-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="d6539-127">x5c</span><span class="sxs-lookup"><span data-stu-id="d6539-127">x5c</span></span> | <span data-ttu-id="d6539-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-128">string collection</span></span> | <span data-ttu-id="d6539-129">O parâmetro "x5c" (cadeia de certificados X. 509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="d6539-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="d6539-130">x5t</span><span class="sxs-lookup"><span data-stu-id="d6539-130">x5t</span></span> | <span data-ttu-id="d6539-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-131">string</span></span> | <span data-ttu-id="d6539-132">O parâmetro "x5t" (impressão digital SHA-1 do certificado 509) é uma impressão digital SHA-1 codificada por base64url (conhecida</span><span class="sxs-lookup"><span data-stu-id="d6539-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="d6539-133">Digest) da codificação DER de um certificado X. 509 [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="d6539-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="d6539-134">minúscula</span><span class="sxs-lookup"><span data-stu-id="d6539-134">e</span></span> | <span data-ttu-id="d6539-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-135">string</span></span> | <span data-ttu-id="d6539-136">Chave RSA – expoente público</span><span class="sxs-lookup"><span data-stu-id="d6539-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="d6539-137">d</span><span class="sxs-lookup"><span data-stu-id="d6539-137">d</span></span>| <span data-ttu-id="d6539-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-138">string</span></span> | <span data-ttu-id="d6539-139">Chave RSA-expoente privado.</span><span class="sxs-lookup"><span data-stu-id="d6539-139">RSA Key - private exponent.</span></span> <span data-ttu-id="d6539-140">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="d6539-141">n</span><span class="sxs-lookup"><span data-stu-id="d6539-141">n</span></span> | <span data-ttu-id="d6539-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-142">string</span></span> | <span data-ttu-id="d6539-143">Chave RSA-módulo</span><span class="sxs-lookup"><span data-stu-id="d6539-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="d6539-144">p</span><span class="sxs-lookup"><span data-stu-id="d6539-144">p</span></span> | <span data-ttu-id="d6539-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-145">string</span></span> | <span data-ttu-id="d6539-146">Chave RSA-primeira linha.</span><span class="sxs-lookup"><span data-stu-id="d6539-146">RSA Key - first prime.</span></span> <span data-ttu-id="d6539-147">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="d6539-148">q</span><span class="sxs-lookup"><span data-stu-id="d6539-148">q</span></span> | <span data-ttu-id="d6539-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-149">string</span></span> | <span data-ttu-id="d6539-150">Chave RSA-segundo primo.</span><span class="sxs-lookup"><span data-stu-id="d6539-150">RSA Key - second prime.</span></span> <span data-ttu-id="d6539-151">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="d6539-152">distribuição</span><span class="sxs-lookup"><span data-stu-id="d6539-152">dp</span></span> | <span data-ttu-id="d6539-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-153">string</span></span> | <span data-ttu-id="d6539-154">Expoente da chave RSA-First.</span><span class="sxs-lookup"><span data-stu-id="d6539-154">RSA Key - first exponent.</span></span> <span data-ttu-id="d6539-155">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="d6539-156">DQ</span><span class="sxs-lookup"><span data-stu-id="d6539-156">dq</span></span> | <span data-ttu-id="d6539-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-157">string</span></span> | <span data-ttu-id="d6539-158">Expoente da chave RSA-segundo.</span><span class="sxs-lookup"><span data-stu-id="d6539-158">RSA Key - second exponent.</span></span> <span data-ttu-id="d6539-159">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="d6539-160">QI</span><span class="sxs-lookup"><span data-stu-id="d6539-160">qi</span></span> | <span data-ttu-id="d6539-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-161">string</span></span> | <span data-ttu-id="d6539-162">O coeficiente de chave RSA.</span><span class="sxs-lookup"><span data-stu-id="d6539-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="d6539-163">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="d6539-164">f</span><span class="sxs-lookup"><span data-stu-id="d6539-164">k</span></span> | <span data-ttu-id="d6539-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6539-165">string</span></span> | <span data-ttu-id="d6539-166">Chave simétrica para tipo de chave Oct.</span><span class="sxs-lookup"><span data-stu-id="d6539-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="d6539-167">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="d6539-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="d6539-168">nbf</span><span class="sxs-lookup"><span data-stu-id="d6539-168">nbf</span></span> | <span data-ttu-id="d6539-169">int</span><span class="sxs-lookup"><span data-stu-id="d6539-169">int</span></span> | <span data-ttu-id="d6539-170">Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.)</span><span class="sxs-lookup"><span data-stu-id="d6539-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="d6539-171">exp</span><span class="sxs-lookup"><span data-stu-id="d6539-171">exp</span></span> | <span data-ttu-id="d6539-172">int</span><span class="sxs-lookup"><span data-stu-id="d6539-172">int</span></span> | <span data-ttu-id="d6539-173">Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.)</span><span class="sxs-lookup"><span data-stu-id="d6539-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="d6539-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6539-174">JSON representation</span></span>

<span data-ttu-id="d6539-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6539-175">The following is a JSON representation of the resource.</span></span>

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


