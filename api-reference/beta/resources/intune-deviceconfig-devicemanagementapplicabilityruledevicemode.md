---
title: tipo de recurso deviceManagementApplicabilityRuleDeviceMode
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 099f6081366187e240bf8510fca30a548fea4fe3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792035"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="235df-103">tipo de recurso deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="235df-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="235df-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="235df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="235df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="235df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="235df-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="235df-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="235df-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="235df-107">Properties</span></span>
|<span data-ttu-id="235df-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="235df-108">Property</span></span>|<span data-ttu-id="235df-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="235df-109">Type</span></span>|<span data-ttu-id="235df-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="235df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="235df-111">devicemode</span><span class="sxs-lookup"><span data-stu-id="235df-111">deviceMode</span></span>|[<span data-ttu-id="235df-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="235df-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="235df-113">Regra de aplicabilidade para o modo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="235df-113">Applicability rule for device mode.</span></span> <span data-ttu-id="235df-114">Os valores possíveis são: `standardConfiguration` e `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="235df-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="235df-115">nome</span><span class="sxs-lookup"><span data-stu-id="235df-115">name</span></span>|<span data-ttu-id="235df-116">String</span><span class="sxs-lookup"><span data-stu-id="235df-116">String</span></span>|<span data-ttu-id="235df-117">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="235df-117">Name for object.</span></span>|
|<span data-ttu-id="235df-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="235df-118">ruleType</span></span>|[<span data-ttu-id="235df-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="235df-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="235df-120">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="235df-120">Applicability Rule type.</span></span> <span data-ttu-id="235df-121">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="235df-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="235df-122">Relações</span><span class="sxs-lookup"><span data-stu-id="235df-122">Relationships</span></span>
<span data-ttu-id="235df-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="235df-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="235df-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="235df-124">JSON Representation</span></span>
<span data-ttu-id="235df-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="235df-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
  "deviceMode": "String",
  "name": "String",
  "ruleType": "String"
}
```



