---
title: tipo de recurso deviceHealthScriptComplianceRule
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371451"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a><span data-ttu-id="6a1dd-103">tipo de recurso deviceHealthScriptComplianceRule</span><span class="sxs-lookup"><span data-stu-id="6a1dd-103">deviceHealthScriptComplianceRule resource type</span></span>

> <span data-ttu-id="6a1dd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a1dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a1dd-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6a1dd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6a1dd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a1dd-107">Properties</span></span>
|<span data-ttu-id="6a1dd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a1dd-108">Property</span></span>|<span data-ttu-id="6a1dd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a1dd-109">Type</span></span>|<span data-ttu-id="6a1dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a1dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a1dd-111">Detecção</span><span class="sxs-lookup"><span data-stu-id="6a1dd-111">detectionType</span></span>|[<span data-ttu-id="6a1dd-112">deviceHealthScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="6a1dd-112">deviceHealthScriptDetectionType</span></span>](../resources/intune-devices-devicehealthscriptdetectiontype.md)|<span data-ttu-id="6a1dd-113">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-113">Not yet documented.</span></span> <span data-ttu-id="6a1dd-114">Os valores possíveis são: `notConfigured` e `string`.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-114">Possible values are: `notConfigured`, `string`.</span></span>|
|<span data-ttu-id="6a1dd-115">operator</span><span class="sxs-lookup"><span data-stu-id="6a1dd-115">operator</span></span>|[<span data-ttu-id="6a1dd-116">deviceHealthScriptComplianceRuleOperator</span><span class="sxs-lookup"><span data-stu-id="6a1dd-116">deviceHealthScriptComplianceRuleOperator</span></span>](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|<span data-ttu-id="6a1dd-117">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-117">Not yet documented.</span></span> <span data-ttu-id="6a1dd-118">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-118">Possible values are: `notConfigured`, `equal`, `notEqual`.</span></span>|
|<span data-ttu-id="6a1dd-119">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="6a1dd-119">detectionValue</span></span>|<span data-ttu-id="6a1dd-120">String</span><span class="sxs-lookup"><span data-stu-id="6a1dd-120">String</span></span>|<span data-ttu-id="6a1dd-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6a1dd-121">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a1dd-122">Relações</span><span class="sxs-lookup"><span data-stu-id="6a1dd-122">Relationships</span></span>
<span data-ttu-id="6a1dd-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a1dd-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a1dd-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a1dd-124">JSON Representation</span></span>
<span data-ttu-id="6a1dd-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a1dd-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



