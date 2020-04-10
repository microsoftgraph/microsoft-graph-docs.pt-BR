---
title: tipo de recurso trustFrameworkKeySet
description: Representa um conjunto de chaves/diretivas de política de confiança.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0784bffd1682f59e94d728c2311ffaaa01681c5
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218048"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="8cadd-103">tipo de recurso trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="8cadd-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="8cadd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cadd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cadd-105">Representa um conjunto de chaves/diretivas de política de confiança.</span><span class="sxs-lookup"><span data-stu-id="8cadd-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="8cadd-106">A estrutura de experiência de identidade armazena os segredos, que podem ser usados nas políticas.</span><span class="sxs-lookup"><span data-stu-id="8cadd-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="8cadd-107">Os segredos podem ser senhas, certificados ou outros arquivos.</span><span class="sxs-lookup"><span data-stu-id="8cadd-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="8cadd-108">No portal, essas entidades são mostradas como `Policy keys`.</span><span class="sxs-lookup"><span data-stu-id="8cadd-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="8cadd-109">A estrutura de experiência de identidade usa o padrão JWK (JSON Web Key) para os conjuntos de chaves.</span><span class="sxs-lookup"><span data-stu-id="8cadd-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="8cadd-110">Esta entidade segue o formato especificado na [RFC 7517 seção 5](https://tools.ietf.org/html/rfc7517#section-5).</span><span class="sxs-lookup"><span data-stu-id="8cadd-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="8cadd-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="8cadd-111">Methods</span></span>

| <span data-ttu-id="8cadd-112">Método</span><span class="sxs-lookup"><span data-stu-id="8cadd-112">Method</span></span>       | <span data-ttu-id="8cadd-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8cadd-113">Return Type</span></span> | <span data-ttu-id="8cadd-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cadd-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8cadd-115">List</span><span class="sxs-lookup"><span data-stu-id="8cadd-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="8cadd-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Coletânea</span><span class="sxs-lookup"><span data-stu-id="8cadd-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="8cadd-117">Listar trustFrameworkKeySets.</span><span class="sxs-lookup"><span data-stu-id="8cadd-117">List trustFrameworkKeySets.</span></span> |
| [<span data-ttu-id="8cadd-118">Create</span><span class="sxs-lookup"><span data-stu-id="8cadd-118">Create</span></span>](../api/trustframework-post-keysets.md) | [<span data-ttu-id="8cadd-119">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="8cadd-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="8cadd-120">Criar trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="8cadd-120">Create  trustFrameworkKeySet.</span></span> |
| [<span data-ttu-id="8cadd-121">Get</span><span class="sxs-lookup"><span data-stu-id="8cadd-121">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="8cadd-122">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="8cadd-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="8cadd-123">Leia as propriedades e os relacionamentos do objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="8cadd-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="8cadd-124">Update</span><span class="sxs-lookup"><span data-stu-id="8cadd-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="8cadd-125">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="8cadd-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="8cadd-126">Atualize o objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="8cadd-126">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="8cadd-127">Delete</span><span class="sxs-lookup"><span data-stu-id="8cadd-127">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="8cadd-128">None</span><span class="sxs-lookup"><span data-stu-id="8cadd-128">None</span></span> | <span data-ttu-id="8cadd-129">Exclua o objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="8cadd-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="8cadd-130">Gerar chave</span><span class="sxs-lookup"><span data-stu-id="8cadd-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="8cadd-131">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="8cadd-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="8cadd-132">Gerar uma chave no conjunto de chaves.</span><span class="sxs-lookup"><span data-stu-id="8cadd-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="8cadd-133">Obter chave ativa</span><span class="sxs-lookup"><span data-stu-id="8cadd-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="8cadd-134">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="8cadd-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="8cadd-135">Obtém a chave ativa atualmente no conjunto de chaves.</span><span class="sxs-lookup"><span data-stu-id="8cadd-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="8cadd-136">Carregar certificado</span><span class="sxs-lookup"><span data-stu-id="8cadd-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="8cadd-137">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="8cadd-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="8cadd-138">Carregar um certificado X. 509.</span><span class="sxs-lookup"><span data-stu-id="8cadd-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="8cadd-139">Carregar PKCS12</span><span class="sxs-lookup"><span data-stu-id="8cadd-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="8cadd-140">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="8cadd-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="8cadd-141">Carregar um certificado no formato PKCS12.</span><span class="sxs-lookup"><span data-stu-id="8cadd-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="8cadd-142">Carregar segredo</span><span class="sxs-lookup"><span data-stu-id="8cadd-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="8cadd-143">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="8cadd-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="8cadd-144">Carregar um segredo baseado em cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="8cadd-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="8cadd-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cadd-145">Properties</span></span>

| <span data-ttu-id="8cadd-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cadd-146">Property</span></span>     | <span data-ttu-id="8cadd-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cadd-147">Type</span></span>        | <span data-ttu-id="8cadd-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cadd-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cadd-149">id</span><span class="sxs-lookup"><span data-stu-id="8cadd-149">id</span></span>|<span data-ttu-id="8cadd-150">String</span><span class="sxs-lookup"><span data-stu-id="8cadd-150">String</span></span>| <span data-ttu-id="8cadd-151">Identificador exclusivo do conjunto de chaves trustframework</span><span class="sxs-lookup"><span data-stu-id="8cadd-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="8cadd-152">as</span><span class="sxs-lookup"><span data-stu-id="8cadd-152">keys</span></span>|<span data-ttu-id="8cadd-153">coleção [trustFrameworkKey](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="8cadd-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="8cadd-154">Uma coleção das chaves.</span><span class="sxs-lookup"><span data-stu-id="8cadd-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8cadd-155">Relações</span><span class="sxs-lookup"><span data-stu-id="8cadd-155">Relationships</span></span>

<span data-ttu-id="8cadd-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cadd-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cadd-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cadd-157">JSON representation</span></span>

<span data-ttu-id="8cadd-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cadd-158">The following is a JSON representation of the resource.</span></span>

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
