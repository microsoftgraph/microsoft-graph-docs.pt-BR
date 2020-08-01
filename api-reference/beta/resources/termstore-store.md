---
title: tipo de recurso Store
description: Representa um repositório de termos de taxonomia.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 319e770ae4ec842d2f722b7beb1845f2449d58f8
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539126"
---
# <a name="store-resource-type"></a><span data-ttu-id="6e936-103">tipo de recurso Store</span><span class="sxs-lookup"><span data-stu-id="6e936-103">store resource type</span></span>

<span data-ttu-id="6e936-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="6e936-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e936-105">Representa um repositório de termos de taxonomia.</span><span class="sxs-lookup"><span data-stu-id="6e936-105">Represents a taxonomy term store.</span></span>

<span data-ttu-id="6e936-106">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="6e936-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6e936-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e936-107">Methods</span></span>
|<span data-ttu-id="6e936-108">Método</span><span class="sxs-lookup"><span data-stu-id="6e936-108">Method</span></span>|<span data-ttu-id="6e936-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e936-109">Return type</span></span>|<span data-ttu-id="6e936-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e936-110">Description</span></span>
|:---|:---|:---
|[<span data-ttu-id="6e936-111">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="6e936-111">List groups</span></span>](../api/termstore-list-groups.md)|<span data-ttu-id="6e936-112">coleção [Microsoft. Graph. termos. Group](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="6e936-112">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span>| <span data-ttu-id="6e936-113">Obtenha os grupos de disponíveis no objeto do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-113">Get the groups from available in the term store object.</span></span>|
|[<span data-ttu-id="6e936-114">Obter repositório</span><span class="sxs-lookup"><span data-stu-id="6e936-114">Get store</span></span>](../api/termstore-store-get.md) | [<span data-ttu-id="6e936-115">Microsoft. Graph. termos. Store</span><span class="sxs-lookup"><span data-stu-id="6e936-115">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="6e936-116">Leia as propriedades e os relacionamentos de um objeto do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-116">Read the properties and relationships of a term store object.</span></span>
|[<span data-ttu-id="6e936-117">Atualizar repositório</span><span class="sxs-lookup"><span data-stu-id="6e936-117">Update store</span></span>](../api/termstore-store-update.md) | [<span data-ttu-id="6e936-118">Microsoft. Graph. termos. Store</span><span class="sxs-lookup"><span data-stu-id="6e936-118">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="6e936-119">Atualizar as propriedades de um objeto do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-119">Update the properties of a term store object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e936-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e936-120">Properties</span></span>
|<span data-ttu-id="6e936-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e936-121">Property</span></span>|<span data-ttu-id="6e936-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e936-122">Type</span></span>|<span data-ttu-id="6e936-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e936-123">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="6e936-124">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="6e936-124">defaultLanguageTag</span></span> | <span data-ttu-id="6e936-125">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6e936-125">String</span></span> | <span data-ttu-id="6e936-126">Idioma padrão do termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-126">Default language of the termstore.</span></span>
|<span data-ttu-id="6e936-127">id</span><span class="sxs-lookup"><span data-stu-id="6e936-127">id</span></span>|<span data-ttu-id="6e936-128">String</span><span class="sxs-lookup"><span data-stu-id="6e936-128">String</span></span> | <span data-ttu-id="6e936-129">Identificador exclusivo do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-129">Unique identifier of the term store.</span></span> <span data-ttu-id="6e936-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e936-130">Read-only.</span></span>
|<span data-ttu-id="6e936-131">languageTags</span><span class="sxs-lookup"><span data-stu-id="6e936-131">languageTags</span></span> | <span data-ttu-id="6e936-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e936-132">String collection</span></span> | <span data-ttu-id="6e936-133">Lista de idiomas para o repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-133">List of languages for the term store.</span></span>

## <a name="relationships"></a><span data-ttu-id="6e936-134">Relações</span><span class="sxs-lookup"><span data-stu-id="6e936-134">Relationships</span></span>
|<span data-ttu-id="6e936-135">Relação</span><span class="sxs-lookup"><span data-stu-id="6e936-135">Relationship</span></span>|<span data-ttu-id="6e936-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e936-136">Type</span></span>|<span data-ttu-id="6e936-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e936-137">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="6e936-138">grupos</span><span class="sxs-lookup"><span data-stu-id="6e936-138">groups</span></span> |<span data-ttu-id="6e936-139">coleção [Microsoft. Graph. termos. Group](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="6e936-139">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span> | <span data-ttu-id="6e936-140">Coleção de todos os grupos disponíveis no repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-140">Collection of all groups available in the term store.</span></span>
|<span data-ttu-id="6e936-141">jogos</span><span class="sxs-lookup"><span data-stu-id="6e936-141">sets</span></span> | <span data-ttu-id="6e936-142">coleção [Microsoft. Graph. termos. Set](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="6e936-142">[microsoft.graph.termStore.set](../resources/termstore-set.md) collection</span></span> | <span data-ttu-id="6e936-143">Coleção de todos os conjuntos disponíveis no repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="6e936-143">Collection of all sets available in the term store.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e936-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e936-144">JSON representation</span></span>
<span data-ttu-id="6e936-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e936-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->

