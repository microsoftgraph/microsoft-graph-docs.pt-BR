---
title: Tipo de recurso trustFrameworkKeySet
description: Representa um keyset/policy da estrutura de confiança.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4bd20bd3b9df4656a3bbc73a52511d64ad463bf5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442765"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="2d889-103">Tipo de recurso trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="2d889-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="2d889-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d889-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d889-105">Representa um keyset/policy da estrutura de confiança.</span><span class="sxs-lookup"><span data-stu-id="2d889-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="2d889-106">A estrutura da Experiência de Identidade armazena os segredos, que podem ser usados nas políticas.</span><span class="sxs-lookup"><span data-stu-id="2d889-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="2d889-107">Os segredos podem ser senhas, certificados ou outros arquivos.</span><span class="sxs-lookup"><span data-stu-id="2d889-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="2d889-108">No portal, essas entidades são mostradas como `Policy keys` .</span><span class="sxs-lookup"><span data-stu-id="2d889-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="2d889-109">A estrutura de Experiência de Identidade usa o padrão JSON Web Key (JWK) para os keysets.</span><span class="sxs-lookup"><span data-stu-id="2d889-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="2d889-110">Esta entidade segue o formato especificado na [RFC 7517 Seção 5](https://tools.ietf.org/html/rfc7517#section-5).</span><span class="sxs-lookup"><span data-stu-id="2d889-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="2d889-111">Methods</span><span class="sxs-lookup"><span data-stu-id="2d889-111">Methods</span></span>

| <span data-ttu-id="2d889-112">Método</span><span class="sxs-lookup"><span data-stu-id="2d889-112">Method</span></span>       | <span data-ttu-id="2d889-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d889-113">Return Type</span></span> | <span data-ttu-id="2d889-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d889-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2d889-115">List</span><span class="sxs-lookup"><span data-stu-id="2d889-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="2d889-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Coleção</span><span class="sxs-lookup"><span data-stu-id="2d889-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="2d889-117">Listar trustFrameworkKeySets.</span><span class="sxs-lookup"><span data-stu-id="2d889-117">List trustFrameworkKeySets.</span></span> |
| [<span data-ttu-id="2d889-118">Create</span><span class="sxs-lookup"><span data-stu-id="2d889-118">Create</span></span>](../api/trustframework-post-keysets.md) | [<span data-ttu-id="2d889-119">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="2d889-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="2d889-120">Crie trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="2d889-120">Create  trustFrameworkKeySet.</span></span> |
| [<span data-ttu-id="2d889-121">Get</span><span class="sxs-lookup"><span data-stu-id="2d889-121">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="2d889-122">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="2d889-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="2d889-123">Leia propriedades e relações do objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="2d889-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="2d889-124">Atualização</span><span class="sxs-lookup"><span data-stu-id="2d889-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="2d889-125">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="2d889-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="2d889-126">Atualizar o objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="2d889-126">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="2d889-127">Delete</span><span class="sxs-lookup"><span data-stu-id="2d889-127">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="2d889-128">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2d889-128">None</span></span> | <span data-ttu-id="2d889-129">Exclua o objeto trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="2d889-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="2d889-130">Gerar chave</span><span class="sxs-lookup"><span data-stu-id="2d889-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="2d889-131">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="2d889-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="2d889-132">Gere uma chave no keyset.</span><span class="sxs-lookup"><span data-stu-id="2d889-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="2d889-133">Obter chave ativa</span><span class="sxs-lookup"><span data-stu-id="2d889-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="2d889-134">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="2d889-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="2d889-135">Obter chave ativa no momento no keyset.</span><span class="sxs-lookup"><span data-stu-id="2d889-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="2d889-136">Carregar certificado</span><span class="sxs-lookup"><span data-stu-id="2d889-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="2d889-137">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="2d889-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="2d889-138">Carregue um certificado X.509.</span><span class="sxs-lookup"><span data-stu-id="2d889-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="2d889-139">Carregar PKCS12</span><span class="sxs-lookup"><span data-stu-id="2d889-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="2d889-140">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="2d889-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="2d889-141">Carregue um certificado de formato PKCS12.</span><span class="sxs-lookup"><span data-stu-id="2d889-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="2d889-142">Carregar segredo</span><span class="sxs-lookup"><span data-stu-id="2d889-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="2d889-143">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="2d889-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="2d889-144">Carregar um segredo baseado em cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="2d889-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d889-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d889-145">Properties</span></span>

| <span data-ttu-id="2d889-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d889-146">Property</span></span>     | <span data-ttu-id="2d889-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d889-147">Type</span></span>        | <span data-ttu-id="2d889-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d889-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d889-149">id</span><span class="sxs-lookup"><span data-stu-id="2d889-149">id</span></span>|<span data-ttu-id="2d889-150">String</span><span class="sxs-lookup"><span data-stu-id="2d889-150">String</span></span>| <span data-ttu-id="2d889-151">Identificador exclusivo do keyset trustframework</span><span class="sxs-lookup"><span data-stu-id="2d889-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="2d889-152">keys</span><span class="sxs-lookup"><span data-stu-id="2d889-152">keys</span></span>|<span data-ttu-id="2d889-153">[Coleção trustFrameworkKey](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="2d889-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="2d889-154">Uma coleção de chaves.</span><span class="sxs-lookup"><span data-stu-id="2d889-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2d889-155">Relações</span><span class="sxs-lookup"><span data-stu-id="2d889-155">Relationships</span></span>

<span data-ttu-id="2d889-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d889-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d889-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d889-157">JSON representation</span></span>

<span data-ttu-id="2d889-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d889-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
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


