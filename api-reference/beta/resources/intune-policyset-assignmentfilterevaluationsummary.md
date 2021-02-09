---
title: Tipo de recurso assignmentFilterEvaluationSummary
description: Representar resumo de resultado para avaliação de filtro de atribuição
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f2e93f481f0b21689b1a83d63f4540c22f50cb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160161"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a><span data-ttu-id="3a84f-103">Tipo de recurso assignmentFilterEvaluationSummary</span><span class="sxs-lookup"><span data-stu-id="3a84f-103">assignmentFilterEvaluationSummary resource type</span></span>

<span data-ttu-id="3a84f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a84f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a84f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a84f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a84f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a84f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a84f-107">Representar resumo de resultado para avaliação de filtro de atribuição</span><span class="sxs-lookup"><span data-stu-id="3a84f-107">Represent result summary for assignment filter evaluation</span></span>

## <a name="properties"></a><span data-ttu-id="3a84f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a84f-108">Properties</span></span>
|<span data-ttu-id="3a84f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a84f-109">Property</span></span>|<span data-ttu-id="3a84f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a84f-110">Type</span></span>|<span data-ttu-id="3a84f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a84f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a84f-112">assignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="3a84f-112">assignmentFilterId</span></span>|<span data-ttu-id="3a84f-113">String</span><span class="sxs-lookup"><span data-stu-id="3a84f-113">String</span></span>|<span data-ttu-id="3a84f-114">Identificador exclusivo do objeto de filtro de atribuição</span><span class="sxs-lookup"><span data-stu-id="3a84f-114">Unique identifier for the assignment filter object</span></span>|
|<span data-ttu-id="3a84f-115">assignmentFilterLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a84f-115">assignmentFilterLastModifiedDateTime</span></span>|<span data-ttu-id="3a84f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a84f-116">DateTimeOffset</span></span>|<span data-ttu-id="3a84f-117">A hora em que o filtro de atribuição foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3a84f-117">The time the assignment filter was last modified.</span></span>|
|<span data-ttu-id="3a84f-118">assignmentFilterDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a84f-118">assignmentFilterDisplayName</span></span>|<span data-ttu-id="3a84f-119">String</span><span class="sxs-lookup"><span data-stu-id="3a84f-119">String</span></span>|<span data-ttu-id="3a84f-120">O nome definido pelo administrador para o filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3a84f-120">The admin defined name for assignment filter.</span></span>|
|<span data-ttu-id="3a84f-121">assignmentFilterPlatform</span><span class="sxs-lookup"><span data-stu-id="3a84f-121">assignmentFilterPlatform</span></span>|[<span data-ttu-id="3a84f-122">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="3a84f-122">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="3a84f-123">A plataforma para a qual esse filtro de atribuição é criado.</span><span class="sxs-lookup"><span data-stu-id="3a84f-123">The platform for which this assignment filter is created.</span></span> <span data-ttu-id="3a84f-124">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3a84f-124">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="3a84f-125">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="3a84f-125">evaluationResult</span></span>|[<span data-ttu-id="3a84f-126">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="3a84f-126">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="3a84f-127">Resultado da avaliação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3a84f-127">Assignment filter evaluation result.</span></span> <span data-ttu-id="3a84f-128">Os possíveis valores são: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span><span class="sxs-lookup"><span data-stu-id="3a84f-128">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|
|<span data-ttu-id="3a84f-129">evaluationDateTime</span><span class="sxs-lookup"><span data-stu-id="3a84f-129">evaluationDateTime</span></span>|<span data-ttu-id="3a84f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a84f-130">DateTimeOffset</span></span>|<span data-ttu-id="3a84f-131">O filtro de atribuição de tempo foi avaliado.</span><span class="sxs-lookup"><span data-stu-id="3a84f-131">The time assignment filter was evaluated.</span></span>|
|<span data-ttu-id="3a84f-132">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="3a84f-132">assignmentFilterType</span></span>|[<span data-ttu-id="3a84f-133">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="3a84f-133">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="3a84f-134">Indica o tipo de filtro incluir ou excluir.</span><span class="sxs-lookup"><span data-stu-id="3a84f-134">Indicate filter type either include or exclude.</span></span> <span data-ttu-id="3a84f-135">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="3a84f-135">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a84f-136">Relações</span><span class="sxs-lookup"><span data-stu-id="3a84f-136">Relationships</span></span>
<span data-ttu-id="3a84f-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a84f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a84f-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a84f-138">JSON Representation</span></span>
<span data-ttu-id="3a84f-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a84f-139">Here is a JSON representation of the resource.</span></span>
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
  "assignmentFilterType": "String"
}
```




