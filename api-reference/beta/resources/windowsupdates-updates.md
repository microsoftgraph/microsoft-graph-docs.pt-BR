---
title: atualiza tipo de recurso
description: Entidade que atua como um contêiner para todas as Windows de implantação do Update for Business.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0306dbadd815bdd8ff0ffde5719a950bcdff4683
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067228"
---
# <a name="updates-resource-type"></a><span data-ttu-id="457d9-103">atualiza tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="457d9-103">updates resource type</span></span>

<span data-ttu-id="457d9-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="457d9-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="457d9-105">Entidade que atua como um contêiner para todas as Windows de implantação do Update for Business.</span><span class="sxs-lookup"><span data-stu-id="457d9-105">Entity that acts as a container for all Windows Update for Business deployment service functionality.</span></span>

## <a name="properties"></a><span data-ttu-id="457d9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="457d9-106">Properties</span></span>
|<span data-ttu-id="457d9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="457d9-107">Property</span></span>|<span data-ttu-id="457d9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="457d9-108">Type</span></span>|<span data-ttu-id="457d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="457d9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457d9-110">id</span><span class="sxs-lookup"><span data-stu-id="457d9-110">id</span></span>|<span data-ttu-id="457d9-111">String</span><span class="sxs-lookup"><span data-stu-id="457d9-111">String</span></span>|<span data-ttu-id="457d9-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="457d9-112">Read-only.</span></span> <span data-ttu-id="457d9-113">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="457d9-113">Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="457d9-114">Relações</span><span class="sxs-lookup"><span data-stu-id="457d9-114">Relationships</span></span>
|<span data-ttu-id="457d9-115">Relação</span><span class="sxs-lookup"><span data-stu-id="457d9-115">Relationship</span></span>|<span data-ttu-id="457d9-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="457d9-116">Type</span></span>|<span data-ttu-id="457d9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="457d9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457d9-118">catalog</span><span class="sxs-lookup"><span data-stu-id="457d9-118">catalog</span></span>|[<span data-ttu-id="457d9-119">microsoft.graph.windowsUpdates.catalog</span><span class="sxs-lookup"><span data-stu-id="457d9-119">microsoft.graph.windowsUpdates.catalog</span></span>](../resources/windowsupdates-catalog.md)|<span data-ttu-id="457d9-120">Catálogo de conteúdo que pode ser aprovado para implantação pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="457d9-120">Catalog of content that can be approved for deployment by the deployment service.</span></span> <span data-ttu-id="457d9-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="457d9-121">Read-only.</span></span>|
|<span data-ttu-id="457d9-122">implantações</span><span class="sxs-lookup"><span data-stu-id="457d9-122">deployments</span></span>|<span data-ttu-id="457d9-123">[coleção microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="457d9-123">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) collection</span></span>|<span data-ttu-id="457d9-124">Implantações criadas usando o serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="457d9-124">Deployments created using the deployment service.</span></span> <span data-ttu-id="457d9-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="457d9-125">Read-only.</span></span>|
|<span data-ttu-id="457d9-126">updatableAssets</span><span class="sxs-lookup"><span data-stu-id="457d9-126">updatableAssets</span></span>|<span data-ttu-id="457d9-127">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="457d9-127">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="457d9-128">Ativos registrados no serviço de implantação que podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="457d9-128">Assets registered with the deployment service that can receive updates.</span></span> <span data-ttu-id="457d9-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="457d9-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="457d9-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="457d9-130">JSON representation</span></span>
<span data-ttu-id="457d9-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="457d9-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

