---
title: Tipo de recurso softwareUpdateCatalogEntry
description: Metadados para uma atualização de software que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3e6d0017860acbfc1371c1555279566e808da1eb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067808"
---
# <a name="softwareupdatecatalogentry-resource-type"></a><span data-ttu-id="7aa8d-103">Tipo de recurso softwareUpdateCatalogEntry</span><span class="sxs-lookup"><span data-stu-id="7aa8d-103">softwareUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="7aa8d-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="7aa8d-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa8d-105">Metadados para uma atualização de software que você pode aprovar para implantação.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-105">Metadata for a software update that you can approve for deployment.</span></span>

<span data-ttu-id="7aa8d-106">Herda de [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8d-106">Inherits from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span> <span data-ttu-id="7aa8d-107">Tipo base [para featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) e [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8d-107">Base type for [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) and [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>

<span data-ttu-id="7aa8d-108">Esse é um tipo abstrato.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-108">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="7aa8d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7aa8d-109">Properties</span></span>
|<span data-ttu-id="7aa8d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aa8d-110">Property</span></span>|<span data-ttu-id="7aa8d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aa8d-111">Type</span></span>|<span data-ttu-id="7aa8d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa8d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aa8d-113">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa8d-113">deployableUntilDateTime</span></span>|<span data-ttu-id="7aa8d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa8d-114">DateTimeOffset</span></span>|<span data-ttu-id="7aa8d-115">A data em que o conteúdo não está mais disponível para implantação usando o serviço.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-115">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="7aa8d-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-116">Read-only.</span></span> <span data-ttu-id="7aa8d-117">Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8d-117">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="7aa8d-118">displayName</span><span class="sxs-lookup"><span data-stu-id="7aa8d-118">displayName</span></span>|<span data-ttu-id="7aa8d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aa8d-119">String</span></span>|<span data-ttu-id="7aa8d-120">O nome de exibição do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-120">The display name of the content.</span></span> <span data-ttu-id="7aa8d-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-121">Read-only.</span></span> <span data-ttu-id="7aa8d-122">Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8d-122">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="7aa8d-123">id</span><span class="sxs-lookup"><span data-stu-id="7aa8d-123">id</span></span>|<span data-ttu-id="7aa8d-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aa8d-124">String</span></span>|<span data-ttu-id="7aa8d-125">O identificador exclusivo para a entrada do catálogo.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-125">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="7aa8d-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-126">Read-only.</span></span> <span data-ttu-id="7aa8d-127">Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8d-127">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="7aa8d-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa8d-128">releaseDateTime</span></span>|<span data-ttu-id="7aa8d-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa8d-129">DateTimeOffset</span></span>|<span data-ttu-id="7aa8d-130">A data de lançamento do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-130">The release date for the content.</span></span> <span data-ttu-id="7aa8d-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-131">Read-only.</span></span> <span data-ttu-id="7aa8d-132">Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8d-132">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7aa8d-133">Relações</span><span class="sxs-lookup"><span data-stu-id="7aa8d-133">Relationships</span></span>
<span data-ttu-id="7aa8d-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7aa8d-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7aa8d-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7aa8d-135">JSON representation</span></span>
<span data-ttu-id="7aa8d-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7aa8d-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

