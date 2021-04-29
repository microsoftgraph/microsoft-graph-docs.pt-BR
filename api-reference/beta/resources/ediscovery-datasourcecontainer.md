---
title: Tipo de recurso dataSourceContainer
description: Classe base para custodiantes e fontes de dados não custodiais.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e2d7d88a3d747817858853ebc6f2909b2edde65b
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080719"
---
# <a name="datasourcecontainer-resource-type"></a><span data-ttu-id="235fa-103">Tipo de recurso dataSourceContainer</span><span class="sxs-lookup"><span data-stu-id="235fa-103">dataSourceContainer resource type</span></span>

<span data-ttu-id="235fa-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="235fa-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="235fa-105">Classe base [para custodiante](../resources/ediscovery-custodian.md) [e nãocustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="235fa-105">Base class for [custodian](../resources/ediscovery-custodian.md) and [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

<span data-ttu-id="235fa-106">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="235fa-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="235fa-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="235fa-107">Methods</span></span>

<span data-ttu-id="235fa-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="235fa-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="235fa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="235fa-109">Properties</span></span>

|<span data-ttu-id="235fa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="235fa-110">Property</span></span>|<span data-ttu-id="235fa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="235fa-111">Type</span></span>|<span data-ttu-id="235fa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="235fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="235fa-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="235fa-113">createdDateTime</span></span>|<span data-ttu-id="235fa-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="235fa-114">DateTimeOffset</span></span>|<span data-ttu-id="235fa-115">Data e hora criadas da entidade dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="235fa-115">Created date and time of the dataSourceContainer entity.</span></span>|
|<span data-ttu-id="235fa-116">displayName</span><span class="sxs-lookup"><span data-stu-id="235fa-116">displayName</span></span>|<span data-ttu-id="235fa-117">String</span><span class="sxs-lookup"><span data-stu-id="235fa-117">String</span></span>|<span data-ttu-id="235fa-118">Nome de exibição da entidade dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="235fa-118">Display name of the dataSourceContainer entity.</span></span>|
|<span data-ttu-id="235fa-119">id</span><span class="sxs-lookup"><span data-stu-id="235fa-119">id</span></span>|<span data-ttu-id="235fa-120">String</span><span class="sxs-lookup"><span data-stu-id="235fa-120">String</span></span>|<span data-ttu-id="235fa-121">Identificador exclusivo do dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="235fa-121">Unique identifier of the dataSourceContainer.</span></span> <span data-ttu-id="235fa-122">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="235fa-122">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="235fa-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="235fa-123">lastModifiedDateTime</span></span>|<span data-ttu-id="235fa-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="235fa-124">DateTimeOffset</span></span>|<span data-ttu-id="235fa-125">Data e hora da última modificação do dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="235fa-125">Last modified date and time of the dataSourceContainer.</span></span>|
|<span data-ttu-id="235fa-126">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="235fa-126">releasedDateTime</span></span>|<span data-ttu-id="235fa-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="235fa-127">DateTimeOffset</span></span>|<span data-ttu-id="235fa-128">Data e hora em que o dataSourceContainer foi liberado do caso.</span><span class="sxs-lookup"><span data-stu-id="235fa-128">Date and time that the dataSourceContainer was released from the case.</span></span>|
|<span data-ttu-id="235fa-129">status</span><span class="sxs-lookup"><span data-stu-id="235fa-129">status</span></span>|<span data-ttu-id="235fa-130">microsoft.graph.ediscovery.dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="235fa-130">microsoft.graph.ediscovery.dataSourceContainerStatus</span></span>|<span data-ttu-id="235fa-131">Status mais recente do dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="235fa-131">Latest status of the dataSourceContainer.</span></span> <span data-ttu-id="235fa-132">Os valores possíveis são: `Active` e `Released`.</span><span class="sxs-lookup"><span data-stu-id="235fa-132">Possible values are: `Active`, `Released`.</span></span>|

### <a name="datasourcecontainerstatus-values"></a><span data-ttu-id="235fa-133">valores dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="235fa-133">dataSourceContainerStatus values</span></span>

|<span data-ttu-id="235fa-134">Member</span><span class="sxs-lookup"><span data-stu-id="235fa-134">Member</span></span>|<span data-ttu-id="235fa-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="235fa-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="235fa-136">Ativo</span><span class="sxs-lookup"><span data-stu-id="235fa-136">Active</span></span>|<span data-ttu-id="235fa-137">O dataSourceContainer está em espera no caso.</span><span class="sxs-lookup"><span data-stu-id="235fa-137">The dataSourceContainer is on hold in the case.</span></span>|
|<span data-ttu-id="235fa-138">Lançado</span><span class="sxs-lookup"><span data-stu-id="235fa-138">Released</span></span>|<span data-ttu-id="235fa-139">O dataSourceContainer foi liberado de espera no caso.</span><span class="sxs-lookup"><span data-stu-id="235fa-139">The dataSourceContainer was released from hold in the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="235fa-140">Relações</span><span class="sxs-lookup"><span data-stu-id="235fa-140">Relationships</span></span>

<span data-ttu-id="235fa-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="235fa-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="235fa-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="235fa-142">JSON representation</span></span>

<span data-ttu-id="235fa-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="235fa-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
