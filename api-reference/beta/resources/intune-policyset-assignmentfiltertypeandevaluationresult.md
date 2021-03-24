---
title: Tipo de recurso assignmentFilterTypeAndEvaluationResult
description: Representa o tipo de filtro e o resultado de avaliação do filtro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f969660fed52d3bdc3c37643d4502ff722cbee0d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146731"
---
# <a name="assignmentfiltertypeandevaluationresult-resource-type"></a><span data-ttu-id="7bfc8-103">Tipo de recurso assignmentFilterTypeAndEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="7bfc8-103">assignmentFilterTypeAndEvaluationResult resource type</span></span>

<span data-ttu-id="7bfc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bfc8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bfc8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bfc8-107">Representa o tipo de filtro e o resultado de avaliação do filtro.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-107">Represents the filter type and evalaution result of the filter.</span></span>

## <a name="properties"></a><span data-ttu-id="7bfc8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bfc8-108">Properties</span></span>
|<span data-ttu-id="7bfc8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bfc8-109">Property</span></span>|<span data-ttu-id="7bfc8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bfc8-110">Type</span></span>|<span data-ttu-id="7bfc8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bfc8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bfc8-112">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="7bfc8-112">assignmentFilterType</span></span>|[<span data-ttu-id="7bfc8-113">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="7bfc8-113">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="7bfc8-114">Representa o tipo de filtro.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-114">Represents the filter type.</span></span> <span data-ttu-id="7bfc8-115">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-115">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="7bfc8-116">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="7bfc8-116">evaluationResult</span></span>|[<span data-ttu-id="7bfc8-117">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="7bfc8-117">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="7bfc8-118">Representa o resultado de evalaution do filtro.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-118">Represents the evalaution result of the filter.</span></span> <span data-ttu-id="7bfc8-119">Os possíveis valores são: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-119">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bfc8-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7bfc8-120">Relationships</span></span>
<span data-ttu-id="7bfc8-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bfc8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bfc8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bfc8-122">JSON Representation</span></span>
<span data-ttu-id="7bfc8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bfc8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterTypeAndEvaluationResult",
  "assignmentFilterType": "String",
  "evaluationResult": "String"
}
```




