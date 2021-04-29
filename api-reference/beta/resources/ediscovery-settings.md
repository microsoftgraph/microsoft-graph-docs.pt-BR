---
title: tipo de recurso de configurações (Descoberta eDiscovery)
description: Configurações para um caso de Descoberta E
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9f0248fa0c6080a143272d997b9d6125e0ccb5a2
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080712"
---
# <a name="settings-resource-type-ediscovery"></a><span data-ttu-id="7aeb0-103">tipo de recurso de configurações (Descoberta eDiscovery)</span><span class="sxs-lookup"><span data-stu-id="7aeb0-103">settings resource type (eDiscovery)</span></span>

<span data-ttu-id="7aeb0-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7aeb0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aeb0-105">Configurações para um caso de Descoberta E.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-105">Settings for an eDiscovery case.</span></span> <span data-ttu-id="7aeb0-106">Para obter detalhes, consulte [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-106">For details, see [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span></span>

<span data-ttu-id="7aeb0-107">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-107">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7aeb0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7aeb0-108">Methods</span></span>

|<span data-ttu-id="7aeb0-109">Método</span><span class="sxs-lookup"><span data-stu-id="7aeb0-109">Method</span></span>|<span data-ttu-id="7aeb0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7aeb0-110">Return type</span></span>|<span data-ttu-id="7aeb0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aeb0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7aeb0-112">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="7aeb0-112">Get settings</span></span>](../api/ediscovery-settings-get.md)|[<span data-ttu-id="7aeb0-113">microsoft.graph.ediscovery.settings</span><span class="sxs-lookup"><span data-stu-id="7aeb0-113">microsoft.graph.ediscovery.settings</span></span>](../resources/ediscovery-settings.md)|<span data-ttu-id="7aeb0-114">Leia as propriedades e as relações de um [objeto microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="7aeb0-114">Read the properties and relationships of a [microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md) object.</span></span>|
|[<span data-ttu-id="7aeb0-115">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="7aeb0-115">Update settings</span></span>](../api/ediscovery-settings-update.md)|[<span data-ttu-id="7aeb0-116">microsoft.graph.ediscovery.settings</span><span class="sxs-lookup"><span data-stu-id="7aeb0-116">microsoft.graph.ediscovery.settings</span></span>](../resources/ediscovery-settings.md)|<span data-ttu-id="7aeb0-117">Atualize as propriedades de [um objeto microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="7aeb0-117">Update the properties of a [microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md) object.</span></span>|
|[<span data-ttu-id="7aeb0-118">resetToDefault</span><span class="sxs-lookup"><span data-stu-id="7aeb0-118">resetToDefault</span></span>](../api/ediscovery-settings-resettodefault.md)|<span data-ttu-id="7aeb0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7aeb0-119">None</span></span>|<span data-ttu-id="7aeb0-120">Redefinir todas as configurações para os valores padrão.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-120">Reset all settings to the default values.</span></span>|

## <a name="properties"></a><span data-ttu-id="7aeb0-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7aeb0-121">Properties</span></span>

|<span data-ttu-id="7aeb0-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aeb0-122">Property</span></span>|<span data-ttu-id="7aeb0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aeb0-123">Type</span></span>|<span data-ttu-id="7aeb0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aeb0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aeb0-125">Id</span><span class="sxs-lookup"><span data-stu-id="7aeb0-125">Id</span></span>|<span data-ttu-id="7aeb0-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7aeb0-126">String</span></span>|<span data-ttu-id="7aeb0-127">A ID do caso de Descoberta e.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-127">The ID of the eDiscovery case.</span></span> <span data-ttu-id="7aeb0-128">Herdado da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-128">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="7aeb0-129">ocr</span><span class="sxs-lookup"><span data-stu-id="7aeb0-129">ocr</span></span>|[<span data-ttu-id="7aeb0-130">microsoft.graph.ediscovery.ocrSettings</span><span class="sxs-lookup"><span data-stu-id="7aeb0-130">microsoft.graph.ediscovery.ocrSettings</span></span>](../resources/ediscovery-ocrsettings.md)|<span data-ttu-id="7aeb0-131">As configurações OCR (Reconhecimento Óptico de Caracteres) para a ocorrência.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-131">The OCR (Optical Character Recognition) settings for the case.</span></span>|
|<span data-ttu-id="7aeb0-132">redundancyDetection</span><span class="sxs-lookup"><span data-stu-id="7aeb0-132">redundancyDetection</span></span>|[<span data-ttu-id="7aeb0-133">microsoft.graph.ediscovery.redundancyDetectionSettings</span><span class="sxs-lookup"><span data-stu-id="7aeb0-133">microsoft.graph.ediscovery.redundancyDetectionSettings</span></span>](../resources/ediscovery-redundancydetectionsettings.md)|<span data-ttu-id="7aeb0-134">As configurações de detecção de redundância (quase duplicata e threading de email) para o caso.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-134">The redundancy (near duplicate and email threading) detection settings for the case.</span></span>|
|<span data-ttu-id="7aeb0-135">topicModeling</span><span class="sxs-lookup"><span data-stu-id="7aeb0-135">topicModeling</span></span>|[<span data-ttu-id="7aeb0-136">microsoft.graph.ediscovery.topicModelingSettings</span><span class="sxs-lookup"><span data-stu-id="7aeb0-136">microsoft.graph.ediscovery.topicModelingSettings</span></span>](../resources/ediscovery-topicmodelingsettings.md)|<span data-ttu-id="7aeb0-137">As configurações de Modelagem de Tópicos (Temas) para o caso.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-137">The Topic Modeling (Themes) settings for the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7aeb0-138">Relações</span><span class="sxs-lookup"><span data-stu-id="7aeb0-138">Relationships</span></span>

<span data-ttu-id="7aeb0-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7aeb0-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7aeb0-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7aeb0-140">JSON representation</span></span>

<span data-ttu-id="7aeb0-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.settings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.settings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
  }
}
```
