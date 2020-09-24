---
title: tipo de recurso Store
description: Representa um repositório de termos de taxonomia.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de8b0c004da804a4d9a617eec20de22c51e98108
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258421"
---
# <a name="store-resource-type"></a><span data-ttu-id="f7386-103">tipo de recurso Store</span><span class="sxs-lookup"><span data-stu-id="f7386-103">store resource type</span></span>

<span data-ttu-id="f7386-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="f7386-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7386-105">Representa um repositório de termos de taxonomia.</span><span class="sxs-lookup"><span data-stu-id="f7386-105">Represents a taxonomy term store.</span></span>

<span data-ttu-id="f7386-106">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="f7386-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f7386-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f7386-107">Methods</span></span>
|<span data-ttu-id="f7386-108">Método</span><span class="sxs-lookup"><span data-stu-id="f7386-108">Method</span></span>|<span data-ttu-id="f7386-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f7386-109">Return type</span></span>|<span data-ttu-id="f7386-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7386-110">Description</span></span>
|:---|:---|:---
|[<span data-ttu-id="f7386-111">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="f7386-111">List groups</span></span>](../api/termstore-list-groups.md)|<span data-ttu-id="f7386-112">coleção [Microsoft. Graph. termos. Group](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="f7386-112">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span>| <span data-ttu-id="f7386-113">Obtenha os grupos de disponíveis no objeto do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-113">Get the groups from available in the term store object.</span></span>|
|[<span data-ttu-id="f7386-114">Obter repositório</span><span class="sxs-lookup"><span data-stu-id="f7386-114">Get store</span></span>](../api/termstore-store-get.md) | [<span data-ttu-id="f7386-115">Microsoft. Graph. termos. Store</span><span class="sxs-lookup"><span data-stu-id="f7386-115">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="f7386-116">Leia as propriedades e os relacionamentos de um objeto do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-116">Read the properties and relationships of a term store object.</span></span>
|[<span data-ttu-id="f7386-117">Atualizar repositório</span><span class="sxs-lookup"><span data-stu-id="f7386-117">Update store</span></span>](../api/termstore-store-update.md) | [<span data-ttu-id="f7386-118">Microsoft. Graph. termos. Store</span><span class="sxs-lookup"><span data-stu-id="f7386-118">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="f7386-119">Atualizar as propriedades de um objeto do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-119">Update the properties of a term store object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7386-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7386-120">Properties</span></span>
|<span data-ttu-id="f7386-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7386-121">Property</span></span>|<span data-ttu-id="f7386-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7386-122">Type</span></span>|<span data-ttu-id="f7386-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7386-123">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="f7386-124">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="f7386-124">defaultLanguageTag</span></span> | <span data-ttu-id="f7386-125">String</span><span class="sxs-lookup"><span data-stu-id="f7386-125">String</span></span> | <span data-ttu-id="f7386-126">Idioma padrão do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-126">Default language of the term store.</span></span>
|<span data-ttu-id="f7386-127">id</span><span class="sxs-lookup"><span data-stu-id="f7386-127">id</span></span>|<span data-ttu-id="f7386-128">String</span><span class="sxs-lookup"><span data-stu-id="f7386-128">String</span></span> | <span data-ttu-id="f7386-129">Identificador exclusivo do repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-129">Unique identifier of the term store.</span></span> <span data-ttu-id="f7386-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7386-130">Read-only.</span></span>
|<span data-ttu-id="f7386-131">languageTags</span><span class="sxs-lookup"><span data-stu-id="f7386-131">languageTags</span></span> | <span data-ttu-id="f7386-132">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f7386-132">String collection</span></span> | <span data-ttu-id="f7386-133">Lista de idiomas para o repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-133">List of languages for the term store.</span></span>

## <a name="relationships"></a><span data-ttu-id="f7386-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f7386-134">Relationships</span></span>
|<span data-ttu-id="f7386-135">Relação</span><span class="sxs-lookup"><span data-stu-id="f7386-135">Relationship</span></span>|<span data-ttu-id="f7386-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7386-136">Type</span></span>|<span data-ttu-id="f7386-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7386-137">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="f7386-138">grupos</span><span class="sxs-lookup"><span data-stu-id="f7386-138">groups</span></span> |<span data-ttu-id="f7386-139">coleção [Microsoft. Graph. termos. Group](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="f7386-139">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span> | <span data-ttu-id="f7386-140">Coleção de todos os grupos disponíveis no repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-140">Collection of all groups available in the term store.</span></span>
|<span data-ttu-id="f7386-141">jogos</span><span class="sxs-lookup"><span data-stu-id="f7386-141">sets</span></span> | <span data-ttu-id="f7386-142">coleção [Microsoft. Graph. termos. Set](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="f7386-142">[microsoft.graph.termStore.set](../resources/termstore-set.md) collection</span></span> | <span data-ttu-id="f7386-143">Coleção de todos os conjuntos disponíveis no repositório de termos.</span><span class="sxs-lookup"><span data-stu-id="f7386-143">Collection of all sets available in the term store.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f7386-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7386-144">JSON representation</span></span>
<span data-ttu-id="f7386-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7386-145">The following is a JSON representation of the resource.</span></span>
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



