---
title: Tipo de recurso assignmentFilterStatusDetails
description: Representam detalhes de status para o dispositivo e a carga e todos os filtros aplicados associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a376b1ff3d554753120860f1d3541f7952dd6130
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160160"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a><span data-ttu-id="b9335-103">Tipo de recurso assignmentFilterStatusDetails</span><span class="sxs-lookup"><span data-stu-id="b9335-103">assignmentFilterStatusDetails resource type</span></span>

<span data-ttu-id="b9335-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9335-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9335-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9335-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9335-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9335-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9335-107">Representam detalhes de status para o dispositivo e a carga e todos os filtros aplicados associados.</span><span class="sxs-lookup"><span data-stu-id="b9335-107">Represent status details for device and payload and all associated applied filters.</span></span>

## <a name="properties"></a><span data-ttu-id="b9335-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9335-108">Properties</span></span>
|<span data-ttu-id="b9335-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9335-109">Property</span></span>|<span data-ttu-id="b9335-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9335-110">Type</span></span>|<span data-ttu-id="b9335-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9335-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9335-112">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b9335-112">managedDeviceId</span></span>|<span data-ttu-id="b9335-113">String</span><span class="sxs-lookup"><span data-stu-id="b9335-113">String</span></span>|<span data-ttu-id="b9335-114">Identificador exclusivo do objeto de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9335-114">Unique identifier for the device object.</span></span>|
|<span data-ttu-id="b9335-115">payloadId</span><span class="sxs-lookup"><span data-stu-id="b9335-115">payloadId</span></span>|<span data-ttu-id="b9335-116">String</span><span class="sxs-lookup"><span data-stu-id="b9335-116">String</span></span>|<span data-ttu-id="b9335-117">Identificador exclusivo do objeto de carga.</span><span class="sxs-lookup"><span data-stu-id="b9335-117">Unique identifier for payload object.</span></span>|
|<span data-ttu-id="b9335-118">userId</span><span class="sxs-lookup"><span data-stu-id="b9335-118">userId</span></span>|<span data-ttu-id="b9335-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9335-119">String</span></span>|<span data-ttu-id="b9335-120">Identificador exclusivo do objeto UserId.</span><span class="sxs-lookup"><span data-stu-id="b9335-120">Unique identifier for UserId object.</span></span> <span data-ttu-id="b9335-121">Pode ser nulo</span><span class="sxs-lookup"><span data-stu-id="b9335-121">Can be null</span></span>|
|<span data-ttu-id="b9335-122">deviceProperties</span><span class="sxs-lookup"><span data-stu-id="b9335-122">deviceProperties</span></span>|<span data-ttu-id="b9335-123">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b9335-123">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b9335-124">Propriedades do dispositivo usadas para avaliação de filtro durante o tempo de check-in do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9335-124">Device properties used for filter evaluation during device check-in time.</span></span>|
|<span data-ttu-id="b9335-125">evalutionSummaries</span><span class="sxs-lookup"><span data-stu-id="b9335-125">evalutionSummaries</span></span>|<span data-ttu-id="b9335-126">[Coleção assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b9335-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection</span></span>|<span data-ttu-id="b9335-127">Resumos de resultados de avaliação para cada filtro associado ao dispositivo e ao conteúdo</span><span class="sxs-lookup"><span data-stu-id="b9335-127">Evaluation result summaries for each filter associated to device and payload</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9335-128">Relações</span><span class="sxs-lookup"><span data-stu-id="b9335-128">Relationships</span></span>
<span data-ttu-id="b9335-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9335-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9335-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9335-130">JSON Representation</span></span>
<span data-ttu-id="b9335-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9335-131">Here is a JSON representation of the resource.</span></span>
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
      "assignmentFilterType": "String"
    }
  ]
}
```




