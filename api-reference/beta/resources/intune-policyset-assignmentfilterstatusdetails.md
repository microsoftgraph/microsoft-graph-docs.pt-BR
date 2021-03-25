---
title: Tipo de recurso assignmentFilterStatusDetails
description: Represente detalhes de status para dispositivo e carga e todos os filtros aplicados associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be36fae74e412395bd74a24b11b36b48cbf165ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155971"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a><span data-ttu-id="3edc4-103">Tipo de recurso assignmentFilterStatusDetails</span><span class="sxs-lookup"><span data-stu-id="3edc4-103">assignmentFilterStatusDetails resource type</span></span>

<span data-ttu-id="3edc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3edc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3edc4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3edc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3edc4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3edc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3edc4-107">Represente detalhes de status para dispositivo e carga e todos os filtros aplicados associados.</span><span class="sxs-lookup"><span data-stu-id="3edc4-107">Represent status details for device and payload and all associated applied filters.</span></span>

## <a name="properties"></a><span data-ttu-id="3edc4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3edc4-108">Properties</span></span>
|<span data-ttu-id="3edc4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3edc4-109">Property</span></span>|<span data-ttu-id="3edc4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3edc4-110">Type</span></span>|<span data-ttu-id="3edc4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3edc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3edc4-112">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="3edc4-112">managedDeviceId</span></span>|<span data-ttu-id="3edc4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3edc4-113">String</span></span>|<span data-ttu-id="3edc4-114">Identificador exclusivo do objeto device.</span><span class="sxs-lookup"><span data-stu-id="3edc4-114">Unique identifier for the device object.</span></span>|
|<span data-ttu-id="3edc4-115">payloadId</span><span class="sxs-lookup"><span data-stu-id="3edc4-115">payloadId</span></span>|<span data-ttu-id="3edc4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3edc4-116">String</span></span>|<span data-ttu-id="3edc4-117">Identificador exclusivo do objeto de carga.</span><span class="sxs-lookup"><span data-stu-id="3edc4-117">Unique identifier for payload object.</span></span>|
|<span data-ttu-id="3edc4-118">userId</span><span class="sxs-lookup"><span data-stu-id="3edc4-118">userId</span></span>|<span data-ttu-id="3edc4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3edc4-119">String</span></span>|<span data-ttu-id="3edc4-120">Identificador exclusivo do objeto UserId.</span><span class="sxs-lookup"><span data-stu-id="3edc4-120">Unique identifier for UserId object.</span></span> <span data-ttu-id="3edc4-121">Pode ser nulo</span><span class="sxs-lookup"><span data-stu-id="3edc4-121">Can be null</span></span>|
|<span data-ttu-id="3edc4-122">deviceProperties</span><span class="sxs-lookup"><span data-stu-id="3edc4-122">deviceProperties</span></span>|<span data-ttu-id="3edc4-123">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3edc4-123">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3edc4-124">Propriedades do dispositivo usadas para avaliação de filtro durante o tempo de check-in do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3edc4-124">Device properties used for filter evaluation during device check-in time.</span></span>|
|<span data-ttu-id="3edc4-125">evalutionSummaries</span><span class="sxs-lookup"><span data-stu-id="3edc4-125">evalutionSummaries</span></span>|<span data-ttu-id="3edc4-126">[coleção assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md)</span><span class="sxs-lookup"><span data-stu-id="3edc4-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection</span></span>|<span data-ttu-id="3edc4-127">Resumos de resultados de avaliação para cada filtro associado ao dispositivo e à carga</span><span class="sxs-lookup"><span data-stu-id="3edc4-127">Evaluation result summaries for each filter associated to device and payload</span></span>|

## <a name="relationships"></a><span data-ttu-id="3edc4-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3edc4-128">Relationships</span></span>
<span data-ttu-id="3edc4-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3edc4-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3edc4-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3edc4-130">JSON Representation</span></span>
<span data-ttu-id="3edc4-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3edc4-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterStatusDetails",
  "managedDeviceId": "String",
  "payloadId": "String",
  "userId": "String",
  "deviceProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "evalutionSummaries": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
      "assignmentFilterId": "String",
      "assignmentFilterLastModifiedDateTime": "String (timestamp)",
      "assignmentFilterDisplayName": "String",
      "assignmentFilterPlatform": "String",
      "evaluationResult": "String",
      "evaluationDateTime": "String (timestamp)",
      "assignmentFilterType": "String",
      "assignmentFilterTypeAndEvaluationResults": [
        {
          "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
          "assignmentFilterType": "String",
          "evaluationResult": "String"
        }
      ]
    }
  ]
}
```




