---
title: tipo de recurso deviceManagementApplicabilityRuleOsVersion
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a81e8d096e8c11d6e1b3dd5117af1b384268095
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332845"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="94461-103">tipo de recurso deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="94461-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="94461-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94461-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94461-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94461-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94461-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94461-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="94461-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94461-107">Properties</span></span>
|<span data-ttu-id="94461-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94461-108">Property</span></span>|<span data-ttu-id="94461-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94461-109">Type</span></span>|<span data-ttu-id="94461-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94461-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94461-111">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="94461-111">minOSVersion</span></span>|<span data-ttu-id="94461-112">String</span><span class="sxs-lookup"><span data-stu-id="94461-112">String</span></span>|<span data-ttu-id="94461-113">Versão mínima do sistema operacional para regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="94461-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="94461-114">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="94461-114">maxOSVersion</span></span>|<span data-ttu-id="94461-115">String</span><span class="sxs-lookup"><span data-stu-id="94461-115">String</span></span>|<span data-ttu-id="94461-116">Versão do sistema operacional máximo para a regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="94461-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="94461-117">name</span><span class="sxs-lookup"><span data-stu-id="94461-117">name</span></span>|<span data-ttu-id="94461-118">String</span><span class="sxs-lookup"><span data-stu-id="94461-118">String</span></span>|<span data-ttu-id="94461-119">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="94461-119">Name for object.</span></span>|
|<span data-ttu-id="94461-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="94461-120">ruleType</span></span>|[<span data-ttu-id="94461-121">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="94461-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="94461-122">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="94461-122">Applicability Rule type.</span></span> <span data-ttu-id="94461-123">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="94461-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94461-124">Relações</span><span class="sxs-lookup"><span data-stu-id="94461-124">Relationships</span></span>
<span data-ttu-id="94461-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94461-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94461-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94461-126">JSON Representation</span></span>
<span data-ttu-id="94461-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94461-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```



