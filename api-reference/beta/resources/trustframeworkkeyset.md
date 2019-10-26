---
title: tipo de recurso trustFrameworkKeySet
description: Representa um conjunto de chaves/diretivas de política de confiança.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ecc644e09f7e57433c263e883513dfbb6294465
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734508"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="6c6d4-103">tipo de recurso trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="6c6d4-103">trustFrameworkKeySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c6d4-104">Representa um conjunto de chaves/diretivas de política de confiança.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-104">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="6c6d4-105">A estrutura de experiência de identidade armazena os segredos, que podem ser usados nas políticas.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-105">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="6c6d4-106">Os segredos podem ser senhas, certificados ou outros arquivos.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-106">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="6c6d4-107">No portal, essas entidades são mostradas como `Policy keys`.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-107">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="6c6d4-108">A estrutura de experiência de identidade usa o padrão JWK (JSON Web Key) para os conjuntos de chaves.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-108">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="6c6d4-109">Esta entidade segue o formato especificado na [RFC 7517 seção 5](https://tools.ietf.org/html/rfc7517#section-5).</span><span class="sxs-lookup"><span data-stu-id="6c6d4-109">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="6c6d4-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c6d4-110">Methods</span></span>

| <span data-ttu-id="6c6d4-111">Método</span><span class="sxs-lookup"><span data-stu-id="6c6d4-111">Method</span></span>       | <span data-ttu-id="6c6d4-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c6d4-112">Return Type</span></span> | <span data-ttu-id="6c6d4-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c6d4-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6c6d4-114">Get</span><span class="sxs-lookup"><span data-stu-id="6c6d4-114">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="6c6d4-115">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="6c6d4-115">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="6c6d4-116">Leia as propriedades e os relacionamentos do objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-116">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="6c6d4-117">Update</span><span class="sxs-lookup"><span data-stu-id="6c6d4-117">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="6c6d4-118">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="6c6d4-118">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="6c6d4-119">Atualize o objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-119">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="6c6d4-120">Delete</span><span class="sxs-lookup"><span data-stu-id="6c6d4-120">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="6c6d4-121">None</span><span class="sxs-lookup"><span data-stu-id="6c6d4-121">None</span></span> | <span data-ttu-id="6c6d4-122">Exclua o objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-122">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="6c6d4-123">Generatekey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-123">Generatekey</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="6c6d4-124">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-124">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="6c6d4-125">Gerar uma chave no conjunto de chaves.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-125">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="6c6d4-126">Getactivekey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-126">Getactivekey</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="6c6d4-127">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-127">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="6c6d4-128">Obtém a chave ativa atualmente no conjunto de chaves.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-128">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="6c6d4-129">Uploadcertificate</span><span class="sxs-lookup"><span data-stu-id="6c6d4-129">Uploadcertificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="6c6d4-130">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-130">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="6c6d4-131">Carregar um certificado X. 509.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-131">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="6c6d4-132">Uploadpkcs12</span><span class="sxs-lookup"><span data-stu-id="6c6d4-132">Uploadpkcs12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="6c6d4-133">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-133">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="6c6d4-134">Carregar um certificado no formato PKCS12.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-134">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="6c6d4-135">Uploadsecret</span><span class="sxs-lookup"><span data-stu-id="6c6d4-135">Uploadsecret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="6c6d4-136">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="6c6d4-136">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="6c6d4-137">Carregar um segredo baseado em cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-137">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="6c6d4-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c6d4-138">Properties</span></span>

| <span data-ttu-id="6c6d4-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c6d4-139">Property</span></span>     | <span data-ttu-id="6c6d4-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c6d4-140">Type</span></span>        | <span data-ttu-id="6c6d4-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c6d4-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c6d4-142">id</span><span class="sxs-lookup"><span data-stu-id="6c6d4-142">id</span></span>|<span data-ttu-id="6c6d4-143">String</span><span class="sxs-lookup"><span data-stu-id="6c6d4-143">String</span></span>| <span data-ttu-id="6c6d4-144">Identificador exclusivo do conjunto de chaves trustframework</span><span class="sxs-lookup"><span data-stu-id="6c6d4-144">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="6c6d4-145">as</span><span class="sxs-lookup"><span data-stu-id="6c6d4-145">keys</span></span>|<span data-ttu-id="6c6d4-146">coleção [trustFrameworkKey](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="6c6d4-146">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="6c6d4-147">Uma coleção das chaves.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-147">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c6d4-148">Relações</span><span class="sxs-lookup"><span data-stu-id="6c6d4-148">Relationships</span></span>

<span data-ttu-id="6c6d4-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c6d4-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c6d4-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c6d4-150">JSON representation</span></span>

<span data-ttu-id="6c6d4-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "keys": [{"@odata.type": "microsoft.graph.trustFrameworkKey"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
