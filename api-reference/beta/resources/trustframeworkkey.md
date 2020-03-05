---
title: tipo de recurso trustFrameworkKey
description: Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia. A estrutura desse recurso segue o formato definido na RFC 7517 seção 4.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a9b94075b7a81fdb596038afac21fbf6cbc68f42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519649"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="afa35-105">tipo de recurso trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="afa35-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="afa35-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="afa35-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afa35-107">Representa um JWK (chave Web JSON).</span><span class="sxs-lookup"><span data-stu-id="afa35-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="afa35-108">TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia.</span><span class="sxs-lookup"><span data-stu-id="afa35-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="afa35-109">A estrutura desse recurso segue o formato definido na [RFC 7517 seção 4](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="afa35-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="afa35-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afa35-110">Properties</span></span>

| <span data-ttu-id="afa35-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afa35-111">Property</span></span>     | <span data-ttu-id="afa35-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="afa35-112">Type</span></span>        | <span data-ttu-id="afa35-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="afa35-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="afa35-114">filho</span><span class="sxs-lookup"><span data-stu-id="afa35-114">kid</span></span> | <span data-ttu-id="afa35-115">string</span><span class="sxs-lookup"><span data-stu-id="afa35-115">string</span></span> | <span data-ttu-id="afa35-116">O identificador exclusivo da chave.</span><span class="sxs-lookup"><span data-stu-id="afa35-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="afa35-117">kty</span><span class="sxs-lookup"><span data-stu-id="afa35-117">kty</span></span> | <span data-ttu-id="afa35-118">string</span><span class="sxs-lookup"><span data-stu-id="afa35-118">string</span></span> | <span data-ttu-id="afa35-119">O parâmetro "KTY" (tipo de chave) identifica a família de algoritmos de criptografia usada com a chave, os valores válidos são RSA, Oct.</span><span class="sxs-lookup"><span data-stu-id="afa35-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="afa35-120">Use</span><span class="sxs-lookup"><span data-stu-id="afa35-120">use</span></span> | <span data-ttu-id="afa35-121">string</span><span class="sxs-lookup"><span data-stu-id="afa35-121">string</span></span> | <span data-ttu-id="afa35-122">O parâmetro "Use" (uso de chave pública) identifica o uso pretendido da chave pública.</span><span class="sxs-lookup"><span data-stu-id="afa35-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="afa35-123">O parâmetro "Use" é empregado para indicar se uma chave pública é usada para criptografar os dados ou para verificar a assinatura dos dados.</span><span class="sxs-lookup"><span data-stu-id="afa35-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="afa35-124">Os valores possíveis são 1.</span><span class="sxs-lookup"><span data-stu-id="afa35-124">Possible values are    1.</span></span> <span data-ttu-id="afa35-125">"SIG" (assinatura) 2.</span><span class="sxs-lookup"><span data-stu-id="afa35-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="afa35-126">"Enc" (criptografia)</span><span class="sxs-lookup"><span data-stu-id="afa35-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="afa35-127">x5c</span><span class="sxs-lookup"><span data-stu-id="afa35-127">x5c</span></span> | <span data-ttu-id="afa35-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="afa35-128">string collection</span></span> | <span data-ttu-id="afa35-129">O parâmetro "x5c" (cadeia de certificados X. 509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="afa35-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="afa35-130">x5t</span><span class="sxs-lookup"><span data-stu-id="afa35-130">x5t</span></span> | <span data-ttu-id="afa35-131">string</span><span class="sxs-lookup"><span data-stu-id="afa35-131">string</span></span> | <span data-ttu-id="afa35-132">O parâmetro "x5t" (impressão digital SHA-1 do certificado 509) é uma impressão digital SHA-1 codificada por base64url (conhecida</span><span class="sxs-lookup"><span data-stu-id="afa35-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="afa35-133">Digest) da codificação DER de um certificado X. 509 [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="afa35-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="afa35-134">minúscula</span><span class="sxs-lookup"><span data-stu-id="afa35-134">e</span></span> | <span data-ttu-id="afa35-135">string</span><span class="sxs-lookup"><span data-stu-id="afa35-135">string</span></span> | <span data-ttu-id="afa35-136">Chave RSA – expoente público</span><span class="sxs-lookup"><span data-stu-id="afa35-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="afa35-137">d</span><span class="sxs-lookup"><span data-stu-id="afa35-137">d</span></span>| <span data-ttu-id="afa35-138">string</span><span class="sxs-lookup"><span data-stu-id="afa35-138">string</span></span> | <span data-ttu-id="afa35-139">Chave RSA-expoente privado.</span><span class="sxs-lookup"><span data-stu-id="afa35-139">RSA Key - private exponent.</span></span> <span data-ttu-id="afa35-140">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="afa35-141">n</span><span class="sxs-lookup"><span data-stu-id="afa35-141">n</span></span> | <span data-ttu-id="afa35-142">string</span><span class="sxs-lookup"><span data-stu-id="afa35-142">string</span></span> | <span data-ttu-id="afa35-143">Chave RSA-módulo</span><span class="sxs-lookup"><span data-stu-id="afa35-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="afa35-144">p</span><span class="sxs-lookup"><span data-stu-id="afa35-144">p</span></span> | <span data-ttu-id="afa35-145">string</span><span class="sxs-lookup"><span data-stu-id="afa35-145">string</span></span> | <span data-ttu-id="afa35-146">Chave RSA-primeira linha.</span><span class="sxs-lookup"><span data-stu-id="afa35-146">RSA Key - first prime.</span></span> <span data-ttu-id="afa35-147">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="afa35-148">q</span><span class="sxs-lookup"><span data-stu-id="afa35-148">q</span></span> | <span data-ttu-id="afa35-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afa35-149">string</span></span> | <span data-ttu-id="afa35-150">Chave RSA-segundo primo.</span><span class="sxs-lookup"><span data-stu-id="afa35-150">RSA Key - second prime.</span></span> <span data-ttu-id="afa35-151">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="afa35-152">distribuição</span><span class="sxs-lookup"><span data-stu-id="afa35-152">dp</span></span> | <span data-ttu-id="afa35-153">string</span><span class="sxs-lookup"><span data-stu-id="afa35-153">string</span></span> | <span data-ttu-id="afa35-154">Expoente da chave RSA-First.</span><span class="sxs-lookup"><span data-stu-id="afa35-154">RSA Key - first exponent.</span></span> <span data-ttu-id="afa35-155">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="afa35-156">DQ</span><span class="sxs-lookup"><span data-stu-id="afa35-156">dq</span></span> | <span data-ttu-id="afa35-157">string</span><span class="sxs-lookup"><span data-stu-id="afa35-157">string</span></span> | <span data-ttu-id="afa35-158">Expoente da chave RSA-segundo.</span><span class="sxs-lookup"><span data-stu-id="afa35-158">RSA Key - second exponent.</span></span> <span data-ttu-id="afa35-159">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="afa35-160">QI</span><span class="sxs-lookup"><span data-stu-id="afa35-160">qi</span></span> | <span data-ttu-id="afa35-161">string</span><span class="sxs-lookup"><span data-stu-id="afa35-161">string</span></span> | <span data-ttu-id="afa35-162">O coeficiente de chave RSA.</span><span class="sxs-lookup"><span data-stu-id="afa35-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="afa35-163">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="afa35-164">f</span><span class="sxs-lookup"><span data-stu-id="afa35-164">k</span></span> | <span data-ttu-id="afa35-165">string</span><span class="sxs-lookup"><span data-stu-id="afa35-165">string</span></span> | <span data-ttu-id="afa35-166">Chave simétrica para tipo de chave Oct.</span><span class="sxs-lookup"><span data-stu-id="afa35-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="afa35-167">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="afa35-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="afa35-168">nbf</span><span class="sxs-lookup"><span data-stu-id="afa35-168">nbf</span></span> | <span data-ttu-id="afa35-169">int</span><span class="sxs-lookup"><span data-stu-id="afa35-169">int</span></span> | <span data-ttu-id="afa35-170">Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.)</span><span class="sxs-lookup"><span data-stu-id="afa35-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="afa35-171">exp</span><span class="sxs-lookup"><span data-stu-id="afa35-171">exp</span></span> | <span data-ttu-id="afa35-172">int</span><span class="sxs-lookup"><span data-stu-id="afa35-172">int</span></span> | <span data-ttu-id="afa35-173">Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.)</span><span class="sxs-lookup"><span data-stu-id="afa35-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="afa35-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afa35-174">JSON representation</span></span>

<span data-ttu-id="afa35-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afa35-175">The following is a JSON representation of the resource.</span></span>

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
