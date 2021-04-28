---
title: tipo de recurso de catálogo
description: Entidade que representa o catálogo de conteúdo que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3fc0630a36d123e6c3e208838d81ee7c33c62853
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067828"
---
# <a name="catalog-resource-type"></a><span data-ttu-id="b5c55-103">tipo de recurso de catálogo</span><span class="sxs-lookup"><span data-stu-id="b5c55-103">catalog resource type</span></span>

<span data-ttu-id="b5c55-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b5c55-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5c55-105">Entidade que representa o catálogo de conteúdo que você pode aprovar para implantação.</span><span class="sxs-lookup"><span data-stu-id="b5c55-105">Entity representing the catalog of content that you can approve for deployment.</span></span>

## <a name="methods"></a><span data-ttu-id="b5c55-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b5c55-106">Methods</span></span>
|<span data-ttu-id="b5c55-107">Método</span><span class="sxs-lookup"><span data-stu-id="b5c55-107">Method</span></span>|<span data-ttu-id="b5c55-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b5c55-108">Return type</span></span>|<span data-ttu-id="b5c55-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5c55-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5c55-110">Listar entradas</span><span class="sxs-lookup"><span data-stu-id="b5c55-110">List entries</span></span>](../api/windowsupdates-catalog-list-entries.md)|<span data-ttu-id="b5c55-111">[coleção microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)</span><span class="sxs-lookup"><span data-stu-id="b5c55-111">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) collection</span></span>|<span data-ttu-id="b5c55-112">Obter os [recursos catalogEntry](../resources/windowsupdates-catalogentry.md) da propriedade de navegação de entradas.</span><span class="sxs-lookup"><span data-stu-id="b5c55-112">Get the [catalogEntry](../resources/windowsupdates-catalogentry.md) resources from the entries navigation property.</span></span> <span data-ttu-id="b5c55-113">Retorna **recursos catalogEntry** dos seguintes tipos derivados: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="b5c55-113">Returns **catalogEntry** resources of the following derived types: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="b5c55-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5c55-114">Properties</span></span>
|<span data-ttu-id="b5c55-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5c55-115">Property</span></span>|<span data-ttu-id="b5c55-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5c55-116">Type</span></span>|<span data-ttu-id="b5c55-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5c55-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5c55-118">id</span><span class="sxs-lookup"><span data-stu-id="b5c55-118">id</span></span>|<span data-ttu-id="b5c55-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5c55-119">String</span></span>|<span data-ttu-id="b5c55-120">Um identificador para o catálogo.</span><span class="sxs-lookup"><span data-stu-id="b5c55-120">An identifier for the catalog.</span></span> <span data-ttu-id="b5c55-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5c55-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5c55-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b5c55-122">Relationships</span></span>
|<span data-ttu-id="b5c55-123">Relação</span><span class="sxs-lookup"><span data-stu-id="b5c55-123">Relationship</span></span>|<span data-ttu-id="b5c55-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5c55-124">Type</span></span>|<span data-ttu-id="b5c55-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5c55-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5c55-126">entradas</span><span class="sxs-lookup"><span data-stu-id="b5c55-126">entries</span></span>|<span data-ttu-id="b5c55-127">[coleção microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)</span><span class="sxs-lookup"><span data-stu-id="b5c55-127">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) collection</span></span>|<span data-ttu-id="b5c55-128">Lista o conteúdo que você pode aprovar para implantação.</span><span class="sxs-lookup"><span data-stu-id="b5c55-128">Lists the content that you can approve for deployment.</span></span> <span data-ttu-id="b5c55-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5c55-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5c55-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5c55-130">JSON representation</span></span>
<span data-ttu-id="b5c55-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5c55-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalog",
  "id": "String (identifier)"
}
```

