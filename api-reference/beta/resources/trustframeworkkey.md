---
title: Tipo de recurso trustFrameworkKey
description: Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica. A estrutura desse recurso segue o formato definido na RFC 7517 Seção 4.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3de9ce67298f31b3c40682040da69f5c2f6ba007
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135853"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="92dbf-105">Tipo de recurso trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="92dbf-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="92dbf-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92dbf-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92dbf-107">Representa um JWK (chave Web JSON).</span><span class="sxs-lookup"><span data-stu-id="92dbf-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="92dbf-108">TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica.</span><span class="sxs-lookup"><span data-stu-id="92dbf-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="92dbf-109">A estrutura desse recurso segue o formato definido na [RFC 7517 Seção 4](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="92dbf-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="92dbf-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92dbf-110">Properties</span></span>

| <span data-ttu-id="92dbf-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92dbf-111">Property</span></span>     | <span data-ttu-id="92dbf-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="92dbf-112">Type</span></span>        | <span data-ttu-id="92dbf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="92dbf-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="92dbf-114">olh</span><span class="sxs-lookup"><span data-stu-id="92dbf-114">kid</span></span> | <span data-ttu-id="92dbf-115">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-115">string</span></span> | <span data-ttu-id="92dbf-116">O identificador exclusivo da chave.</span><span class="sxs-lookup"><span data-stu-id="92dbf-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="92dbf-117">kty</span><span class="sxs-lookup"><span data-stu-id="92dbf-117">kty</span></span> | <span data-ttu-id="92dbf-118">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-118">string</span></span> | <span data-ttu-id="92dbf-119">O parâmetro "kty" (tipo de chave) identifica a família de algoritmos criptográficos usada com a chave, os valores válidos são rsa, oct.</span><span class="sxs-lookup"><span data-stu-id="92dbf-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="92dbf-120">use</span><span class="sxs-lookup"><span data-stu-id="92dbf-120">use</span></span> | <span data-ttu-id="92dbf-121">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-121">string</span></span> | <span data-ttu-id="92dbf-122">O parâmetro "use" (uso de chave pública) identifica o uso pretendido da chave pública.</span><span class="sxs-lookup"><span data-stu-id="92dbf-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="92dbf-123">O parâmetro "use" é empregado para indicar se uma chave pública é usada para criptografar dados ou verificar a assinatura nos dados.</span><span class="sxs-lookup"><span data-stu-id="92dbf-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="92dbf-124">Os valores possíveis são 1.</span><span class="sxs-lookup"><span data-stu-id="92dbf-124">Possible values are    1.</span></span> <span data-ttu-id="92dbf-125">"sig" (assinatura) 2.</span><span class="sxs-lookup"><span data-stu-id="92dbf-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="92dbf-126">"enc" (criptografia)</span><span class="sxs-lookup"><span data-stu-id="92dbf-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="92dbf-127">x5c</span><span class="sxs-lookup"><span data-stu-id="92dbf-127">x5c</span></span> | <span data-ttu-id="92dbf-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dbf-128">string collection</span></span> | <span data-ttu-id="92dbf-129">O parâmetro "x5c" (cadeia de certificados X.509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280.](https://tools.ietf.org/html/rfc5280)</span><span class="sxs-lookup"><span data-stu-id="92dbf-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="92dbf-130">x5t</span><span class="sxs-lookup"><span data-stu-id="92dbf-130">x5t</span></span> | <span data-ttu-id="92dbf-131">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-131">string</span></span> | <span data-ttu-id="92dbf-132">O parâmetro "x5t" (certificado X.509 SHA-1 thumbprint) é uma impressão digital SHA-1 codificada em base64url (ou seja,</span><span class="sxs-lookup"><span data-stu-id="92dbf-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="92dbf-133">digest) da codificação DER de um certificado X.509 [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="92dbf-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="92dbf-134">e</span><span class="sxs-lookup"><span data-stu-id="92dbf-134">e</span></span> | <span data-ttu-id="92dbf-135">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-135">string</span></span> | <span data-ttu-id="92dbf-136">Chave RSA - expoente público</span><span class="sxs-lookup"><span data-stu-id="92dbf-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="92dbf-137">d</span><span class="sxs-lookup"><span data-stu-id="92dbf-137">d</span></span>| <span data-ttu-id="92dbf-138">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-138">string</span></span> | <span data-ttu-id="92dbf-139">Chave RSA - expoente privado.</span><span class="sxs-lookup"><span data-stu-id="92dbf-139">RSA Key - private exponent.</span></span> <span data-ttu-id="92dbf-140">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="92dbf-141">n</span><span class="sxs-lookup"><span data-stu-id="92dbf-141">n</span></span> | <span data-ttu-id="92dbf-142">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-142">string</span></span> | <span data-ttu-id="92dbf-143">Chave RSA - módulo</span><span class="sxs-lookup"><span data-stu-id="92dbf-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="92dbf-144">p</span><span class="sxs-lookup"><span data-stu-id="92dbf-144">p</span></span> | <span data-ttu-id="92dbf-145">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-145">string</span></span> | <span data-ttu-id="92dbf-146">Chave RSA - primeiro prime.</span><span class="sxs-lookup"><span data-stu-id="92dbf-146">RSA Key - first prime.</span></span> <span data-ttu-id="92dbf-147">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="92dbf-148">q</span><span class="sxs-lookup"><span data-stu-id="92dbf-148">q</span></span> | <span data-ttu-id="92dbf-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dbf-149">string</span></span> | <span data-ttu-id="92dbf-150">Chave RSA - segundo prime.</span><span class="sxs-lookup"><span data-stu-id="92dbf-150">RSA Key - second prime.</span></span> <span data-ttu-id="92dbf-151">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="92dbf-152">dp</span><span class="sxs-lookup"><span data-stu-id="92dbf-152">dp</span></span> | <span data-ttu-id="92dbf-153">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-153">string</span></span> | <span data-ttu-id="92dbf-154">Chave RSA - primeiro expoente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-154">RSA Key - first exponent.</span></span> <span data-ttu-id="92dbf-155">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="92dbf-156">dq</span><span class="sxs-lookup"><span data-stu-id="92dbf-156">dq</span></span> | <span data-ttu-id="92dbf-157">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-157">string</span></span> | <span data-ttu-id="92dbf-158">Chave RSA - segundo expoente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-158">RSA Key - second exponent.</span></span> <span data-ttu-id="92dbf-159">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="92dbf-160">2013</span><span class="sxs-lookup"><span data-stu-id="92dbf-160">qi</span></span> | <span data-ttu-id="92dbf-161">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-161">string</span></span> | <span data-ttu-id="92dbf-162">Chave RSA - Coeficiente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="92dbf-163">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="92dbf-164">k</span><span class="sxs-lookup"><span data-stu-id="92dbf-164">k</span></span> | <span data-ttu-id="92dbf-165">string</span><span class="sxs-lookup"><span data-stu-id="92dbf-165">string</span></span> | <span data-ttu-id="92dbf-166">Chave simétrica para o tipo de chave de oct.</span><span class="sxs-lookup"><span data-stu-id="92dbf-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="92dbf-167">O campo não pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="92dbf-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="92dbf-168">nbf</span><span class="sxs-lookup"><span data-stu-id="92dbf-168">nbf</span></span> | <span data-ttu-id="92dbf-169">int</span><span class="sxs-lookup"><span data-stu-id="92dbf-169">int</span></span> | <span data-ttu-id="92dbf-170">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="92dbf-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="92dbf-171">exp</span><span class="sxs-lookup"><span data-stu-id="92dbf-171">exp</span></span> | <span data-ttu-id="92dbf-172">int</span><span class="sxs-lookup"><span data-stu-id="92dbf-172">int</span></span> | <span data-ttu-id="92dbf-173">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="92dbf-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="92dbf-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92dbf-174">JSON representation</span></span>

<span data-ttu-id="92dbf-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92dbf-175">The following is a JSON representation of the resource.</span></span>

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


