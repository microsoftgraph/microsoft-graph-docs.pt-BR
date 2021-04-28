---
title: Tipo de recurso catalogEntry
description: Metadados para um conteúdo que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 5c9766fd93c0a550556cb7f47e3275f65c238de7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067248"
---
# <a name="catalogentry-resource-type"></a><span data-ttu-id="ab3ca-103">Tipo de recurso catalogEntry</span><span class="sxs-lookup"><span data-stu-id="ab3ca-103">catalogEntry resource type</span></span>

<span data-ttu-id="ab3ca-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ab3ca-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab3ca-105">Metadados para um conteúdo que você pode aprovar para implantação.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-105">Metadata for a piece of content that you can approve for deployment.</span></span>

<span data-ttu-id="ab3ca-106">Todas as entradas de catálogo existem como um dos seguintes tipos derivados: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) e [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ab3ca-106">All catalog entries exist as one of the following derived types: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) and [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>

<span data-ttu-id="ab3ca-107">Tipo base para [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ab3ca-107">Base type for [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

<span data-ttu-id="ab3ca-108">Esse é um tipo abstrato.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-108">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="ab3ca-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab3ca-109">Properties</span></span>
|<span data-ttu-id="ab3ca-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab3ca-110">Property</span></span>|<span data-ttu-id="ab3ca-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab3ca-111">Type</span></span>|<span data-ttu-id="ab3ca-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab3ca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab3ca-113">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3ca-113">deployableUntilDateTime</span></span>|<span data-ttu-id="ab3ca-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab3ca-114">DateTimeOffset</span></span>|<span data-ttu-id="ab3ca-115">A data em que o conteúdo não está mais disponível para implantação usando o serviço.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-115">The date on which the content is no longer available to deploy using the service.</span></span> <span data-ttu-id="ab3ca-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-116">Read-only.</span></span>|
|<span data-ttu-id="ab3ca-117">displayName</span><span class="sxs-lookup"><span data-stu-id="ab3ca-117">displayName</span></span>|<span data-ttu-id="ab3ca-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab3ca-118">String</span></span>|<span data-ttu-id="ab3ca-119">O nome de exibição do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-119">The display name of the content.</span></span> <span data-ttu-id="ab3ca-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-120">Read-only.</span></span>|
|<span data-ttu-id="ab3ca-121">id</span><span class="sxs-lookup"><span data-stu-id="ab3ca-121">id</span></span>|<span data-ttu-id="ab3ca-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab3ca-122">String</span></span>|<span data-ttu-id="ab3ca-123">O identificador exclusivo para a entrada do catálogo.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-123">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="ab3ca-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-124">Read-only.</span></span>|
|<span data-ttu-id="ab3ca-125">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3ca-125">releaseDateTime</span></span>|<span data-ttu-id="ab3ca-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab3ca-126">DateTimeOffset</span></span>|<span data-ttu-id="ab3ca-127">A data de lançamento do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-127">The release date for the content.</span></span> <span data-ttu-id="ab3ca-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab3ca-129">Relações</span><span class="sxs-lookup"><span data-stu-id="ab3ca-129">Relationships</span></span>
<span data-ttu-id="ab3ca-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab3ca-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab3ca-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab3ca-131">JSON representation</span></span>
<span data-ttu-id="ab3ca-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

