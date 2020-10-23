---
title: tipo de recurso deviceManagementApplicabilityRuleDeviceMode
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 882ad68b651faf1f0c53eb6851c9491d711426f4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724597"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="b1305-103">tipo de recurso deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1305-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="b1305-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1305-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1305-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1305-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1305-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1305-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1305-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1305-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b1305-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1305-108">Properties</span></span>
|<span data-ttu-id="b1305-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1305-109">Property</span></span>|<span data-ttu-id="b1305-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1305-110">Type</span></span>|<span data-ttu-id="b1305-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1305-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1305-112">devicemode</span><span class="sxs-lookup"><span data-stu-id="b1305-112">deviceMode</span></span>|[<span data-ttu-id="b1305-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="b1305-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="b1305-114">Regra de aplicabilidade para o modo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1305-114">Applicability rule for device mode.</span></span> <span data-ttu-id="b1305-115">Os valores possíveis são: `standardConfiguration` e `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="b1305-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="b1305-116">nome</span><span class="sxs-lookup"><span data-stu-id="b1305-116">name</span></span>|<span data-ttu-id="b1305-117">String</span><span class="sxs-lookup"><span data-stu-id="b1305-117">String</span></span>|<span data-ttu-id="b1305-118">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="b1305-118">Name for object.</span></span>|
|<span data-ttu-id="b1305-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="b1305-119">ruleType</span></span>|[<span data-ttu-id="b1305-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="b1305-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="b1305-121">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="b1305-121">Applicability Rule type.</span></span> <span data-ttu-id="b1305-122">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="b1305-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1305-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b1305-123">Relationships</span></span>
<span data-ttu-id="b1305-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1305-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1305-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1305-125">JSON Representation</span></span>
<span data-ttu-id="b1305-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1305-126">Here is a JSON representation of the resource.</span></span>
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





