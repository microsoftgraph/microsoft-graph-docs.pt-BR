---
title: Tipo de recurso assignmentFilterEvaluationSummary
description: Representar resumo de resultados para avaliação de filtro de atribuição
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05c9a3eabd22e7e22a6d74229b7aa47901e05db6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155978"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a><span data-ttu-id="ee047-103">Tipo de recurso assignmentFilterEvaluationSummary</span><span class="sxs-lookup"><span data-stu-id="ee047-103">assignmentFilterEvaluationSummary resource type</span></span>

<span data-ttu-id="ee047-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee047-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee047-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee047-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee047-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee047-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee047-107">Representar resumo de resultados para avaliação de filtro de atribuição</span><span class="sxs-lookup"><span data-stu-id="ee047-107">Represent result summary for assignment filter evaluation</span></span>

## <a name="properties"></a><span data-ttu-id="ee047-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee047-108">Properties</span></span>
|<span data-ttu-id="ee047-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee047-109">Property</span></span>|<span data-ttu-id="ee047-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee047-110">Type</span></span>|<span data-ttu-id="ee047-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee047-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee047-112">assignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="ee047-112">assignmentFilterId</span></span>|<span data-ttu-id="ee047-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee047-113">String</span></span>|<span data-ttu-id="ee047-114">Identificador exclusivo do objeto de filtro de atribuição</span><span class="sxs-lookup"><span data-stu-id="ee047-114">Unique identifier for the assignment filter object</span></span>|
|<span data-ttu-id="ee047-115">assignmentFilterLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee047-115">assignmentFilterLastModifiedDateTime</span></span>|<span data-ttu-id="ee047-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee047-116">DateTimeOffset</span></span>|<span data-ttu-id="ee047-117">A hora em que o filtro de atribuição foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ee047-117">The time the assignment filter was last modified.</span></span>|
|<span data-ttu-id="ee047-118">assignmentFilterDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee047-118">assignmentFilterDisplayName</span></span>|<span data-ttu-id="ee047-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee047-119">String</span></span>|<span data-ttu-id="ee047-120">O nome definido pelo administrador para filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="ee047-120">The admin defined name for assignment filter.</span></span>|
|<span data-ttu-id="ee047-121">assignmentFilterPlatform</span><span class="sxs-lookup"><span data-stu-id="ee047-121">assignmentFilterPlatform</span></span>|[<span data-ttu-id="ee047-122">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="ee047-122">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="ee047-123">A plataforma para a qual esse filtro de atribuição é criado.</span><span class="sxs-lookup"><span data-stu-id="ee047-123">The platform for which this assignment filter is created.</span></span> <span data-ttu-id="ee047-124">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ee047-124">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="ee047-125">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="ee047-125">evaluationResult</span></span>|[<span data-ttu-id="ee047-126">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="ee047-126">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="ee047-127">Resultado da avaliação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="ee047-127">Assignment filter evaluation result.</span></span> <span data-ttu-id="ee047-128">Os possíveis valores são: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span><span class="sxs-lookup"><span data-stu-id="ee047-128">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|
|<span data-ttu-id="ee047-129">evaluationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee047-129">evaluationDateTime</span></span>|<span data-ttu-id="ee047-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee047-130">DateTimeOffset</span></span>|<span data-ttu-id="ee047-131">O filtro de atribuição de hora foi avaliado.</span><span class="sxs-lookup"><span data-stu-id="ee047-131">The time assignment filter was evaluated.</span></span>|
|<span data-ttu-id="ee047-132">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ee047-132">assignmentFilterType</span></span>|[<span data-ttu-id="ee047-133">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ee047-133">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="ee047-134">Indique o tipo de filtro incluir ou excluir.</span><span class="sxs-lookup"><span data-stu-id="ee047-134">Indicate filter type either include or exclude.</span></span> <span data-ttu-id="ee047-135">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="ee047-135">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="ee047-136">assignmentFilterTypeAndEvaluationResults</span><span class="sxs-lookup"><span data-stu-id="ee047-136">assignmentFilterTypeAndEvaluationResults</span></span>|<span data-ttu-id="ee047-137">[coleção assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee047-137">[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) collection</span></span>|<span data-ttu-id="ee047-138">Uma coleção de tipos de filtro e seus resultados de avaliação correspondentes.</span><span class="sxs-lookup"><span data-stu-id="ee047-138">A collection of filter types and their corresponding evaluation results.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee047-139">Relações</span><span class="sxs-lookup"><span data-stu-id="ee047-139">Relationships</span></span>
<span data-ttu-id="ee047-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee047-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee047-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee047-141">JSON Representation</span></span>
<span data-ttu-id="ee047-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee047-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
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
```




