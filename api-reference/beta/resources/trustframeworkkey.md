---
title: tipo de recurso trustFrameworkKey
description: Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia. A estrutura desse recurso segue o formato definido na RFC 7517 seção 4.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d61548707d9530d30f81b61ad88dd29ae2576c8
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734529"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="3e407-105">tipo de recurso trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="3e407-105">trustFrameworkKey resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e407-106">Representa um JWK (chave Web JSON).</span><span class="sxs-lookup"><span data-stu-id="3e407-106">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="3e407-107">TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia.</span><span class="sxs-lookup"><span data-stu-id="3e407-107">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="3e407-108">A estrutura desse recurso segue o formato definido na [RFC 7517 seção 4](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="3e407-108">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="3e407-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e407-109">Properties</span></span>

| <span data-ttu-id="3e407-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e407-110">Property</span></span>     | <span data-ttu-id="3e407-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e407-111">Type</span></span>        | <span data-ttu-id="3e407-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e407-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3e407-113">filho</span><span class="sxs-lookup"><span data-stu-id="3e407-113">kid</span></span> | <span data-ttu-id="3e407-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-114">string</span></span> | <span data-ttu-id="3e407-115">O identificador exclusivo da chave.</span><span class="sxs-lookup"><span data-stu-id="3e407-115">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="3e407-116">kty</span><span class="sxs-lookup"><span data-stu-id="3e407-116">kty</span></span> | <span data-ttu-id="3e407-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-117">string</span></span> | <span data-ttu-id="3e407-118">O parâmetro "KTY" (tipo de chave) identifica a família de algoritmos de criptografia usada com a chave, os valores válidos são RSA, Oct.</span><span class="sxs-lookup"><span data-stu-id="3e407-118">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="3e407-119">Use</span><span class="sxs-lookup"><span data-stu-id="3e407-119">use</span></span> | <span data-ttu-id="3e407-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-120">string</span></span> | <span data-ttu-id="3e407-121">O parâmetro "Use" (uso de chave pública) identifica o uso pretendido da chave pública.</span><span class="sxs-lookup"><span data-stu-id="3e407-121">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="3e407-122">O parâmetro "Use" é empregado para indicar se uma chave pública é usada para criptografar os dados ou para verificar a assinatura dos dados.</span><span class="sxs-lookup"><span data-stu-id="3e407-122">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="3e407-123">Os valores possíveis são 1.</span><span class="sxs-lookup"><span data-stu-id="3e407-123">Possible values are    1.</span></span> <span data-ttu-id="3e407-124">"SIG" (assinatura) 2.</span><span class="sxs-lookup"><span data-stu-id="3e407-124">"sig" (signature)    2.</span></span>  <span data-ttu-id="3e407-125">"Enc" (criptografia)</span><span class="sxs-lookup"><span data-stu-id="3e407-125">"enc" (encryption)</span></span>   |
| <span data-ttu-id="3e407-126">x5c</span><span class="sxs-lookup"><span data-stu-id="3e407-126">x5c</span></span> | <span data-ttu-id="3e407-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-127">string collection</span></span> | <span data-ttu-id="3e407-128">O parâmetro "x5c" (cadeia de certificados X. 509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="3e407-128">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="3e407-129">x5t</span><span class="sxs-lookup"><span data-stu-id="3e407-129">x5t</span></span> | <span data-ttu-id="3e407-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-130">string</span></span> | <span data-ttu-id="3e407-131">O parâmetro "x5t" (impressão digital SHA-1 do certificado 509) é uma impressão digital SHA-1 codificada por base64url (conhecida</span><span class="sxs-lookup"><span data-stu-id="3e407-131">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="3e407-132">Digest) da codificação DER de um certificado X. 509 [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="3e407-132">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="3e407-133">minúscula</span><span class="sxs-lookup"><span data-stu-id="3e407-133">e</span></span> | <span data-ttu-id="3e407-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-134">string</span></span> | <span data-ttu-id="3e407-135">Chave RSA – expoente público</span><span class="sxs-lookup"><span data-stu-id="3e407-135">RSA Key - public exponent</span></span> |
| <span data-ttu-id="3e407-136">d</span><span class="sxs-lookup"><span data-stu-id="3e407-136">d</span></span>| <span data-ttu-id="3e407-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-137">string</span></span> | <span data-ttu-id="3e407-138">Chave RSA-expoente privado.</span><span class="sxs-lookup"><span data-stu-id="3e407-138">RSA Key - private exponent.</span></span> <span data-ttu-id="3e407-139">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-139">Field cannot be read back.</span></span> |
| <span data-ttu-id="3e407-140">m</span><span class="sxs-lookup"><span data-stu-id="3e407-140">n</span></span> | <span data-ttu-id="3e407-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-141">string</span></span> | <span data-ttu-id="3e407-142">Chave RSA-módulo</span><span class="sxs-lookup"><span data-stu-id="3e407-142">RSA Key - modulus</span></span> |
| <span data-ttu-id="3e407-143">p</span><span class="sxs-lookup"><span data-stu-id="3e407-143">p</span></span> | <span data-ttu-id="3e407-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-144">string</span></span> | <span data-ttu-id="3e407-145">Chave RSA-primeira linha.</span><span class="sxs-lookup"><span data-stu-id="3e407-145">RSA Key - first prime.</span></span> <span data-ttu-id="3e407-146">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-146">Field cannot be read back.</span></span> |
| <span data-ttu-id="3e407-147">q</span><span class="sxs-lookup"><span data-stu-id="3e407-147">q</span></span> | <span data-ttu-id="3e407-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-148">string</span></span> | <span data-ttu-id="3e407-149">Chave RSA-segundo primo.</span><span class="sxs-lookup"><span data-stu-id="3e407-149">RSA Key - second prime.</span></span> <span data-ttu-id="3e407-150">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-150">Field cannot be read back.</span></span> |
| <span data-ttu-id="3e407-151">distribuição</span><span class="sxs-lookup"><span data-stu-id="3e407-151">dp</span></span> | <span data-ttu-id="3e407-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-152">string</span></span> | <span data-ttu-id="3e407-153">Expoente da chave RSA-First.</span><span class="sxs-lookup"><span data-stu-id="3e407-153">RSA Key - first exponent.</span></span> <span data-ttu-id="3e407-154">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-154">Field cannot be read back.</span></span> |
| <span data-ttu-id="3e407-155">DQ</span><span class="sxs-lookup"><span data-stu-id="3e407-155">dq</span></span> | <span data-ttu-id="3e407-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-156">string</span></span> | <span data-ttu-id="3e407-157">Expoente da chave RSA-segundo.</span><span class="sxs-lookup"><span data-stu-id="3e407-157">RSA Key - second exponent.</span></span> <span data-ttu-id="3e407-158">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-158">Field cannot be read back.</span></span> |
| <span data-ttu-id="3e407-159">QI</span><span class="sxs-lookup"><span data-stu-id="3e407-159">qi</span></span> | <span data-ttu-id="3e407-160">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-160">string</span></span> | <span data-ttu-id="3e407-161">O coeficiente de chave RSA.</span><span class="sxs-lookup"><span data-stu-id="3e407-161">RSA Key - Coefficient.</span></span> <span data-ttu-id="3e407-162">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-162">Field cannot be read back.</span></span> |
| <span data-ttu-id="3e407-163">f</span><span class="sxs-lookup"><span data-stu-id="3e407-163">k</span></span> | <span data-ttu-id="3e407-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e407-164">string</span></span> | <span data-ttu-id="3e407-165">Chave simétrica para tipo de chave Oct.</span><span class="sxs-lookup"><span data-stu-id="3e407-165">Symmetric Key for oct key type.</span></span> <span data-ttu-id="3e407-166">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="3e407-166">Field cannot be read back.</span></span>   |
| <span data-ttu-id="3e407-167">nbf</span><span class="sxs-lookup"><span data-stu-id="3e407-167">nbf</span></span> | <span data-ttu-id="3e407-168">int</span><span class="sxs-lookup"><span data-stu-id="3e407-168">int</span></span> | <span data-ttu-id="3e407-169">Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.)</span><span class="sxs-lookup"><span data-stu-id="3e407-169">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="3e407-170">exp</span><span class="sxs-lookup"><span data-stu-id="3e407-170">exp</span></span> | <span data-ttu-id="3e407-171">int</span><span class="sxs-lookup"><span data-stu-id="3e407-171">int</span></span> | <span data-ttu-id="3e407-172">Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.)</span><span class="sxs-lookup"><span data-stu-id="3e407-172">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="3e407-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e407-173">JSON representation</span></span>

<span data-ttu-id="3e407-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e407-174">The following is a JSON representation of the resource.</span></span>

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
