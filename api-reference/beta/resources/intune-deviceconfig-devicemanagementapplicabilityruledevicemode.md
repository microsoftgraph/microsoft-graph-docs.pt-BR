---
title: tipo de recurso deviceManagementApplicabilityRuleDeviceMode
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 040cf91d9733f0abca8c3d97a8955c915aa28bc4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526605"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="94d1b-103">tipo de recurso deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="94d1b-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="94d1b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94d1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94d1b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94d1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94d1b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94d1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94d1b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94d1b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="94d1b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94d1b-108">Properties</span></span>
|<span data-ttu-id="94d1b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94d1b-109">Property</span></span>|<span data-ttu-id="94d1b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="94d1b-110">Type</span></span>|<span data-ttu-id="94d1b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="94d1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94d1b-112">devicemode</span><span class="sxs-lookup"><span data-stu-id="94d1b-112">deviceMode</span></span>|[<span data-ttu-id="94d1b-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="94d1b-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="94d1b-114">Regra de aplicabilidade para o modo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94d1b-114">Applicability rule for device mode.</span></span> <span data-ttu-id="94d1b-115">Os valores possíveis são: `standardConfiguration` e `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="94d1b-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="94d1b-116">nome</span><span class="sxs-lookup"><span data-stu-id="94d1b-116">name</span></span>|<span data-ttu-id="94d1b-117">String</span><span class="sxs-lookup"><span data-stu-id="94d1b-117">String</span></span>|<span data-ttu-id="94d1b-118">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="94d1b-118">Name for object.</span></span>|
|<span data-ttu-id="94d1b-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="94d1b-119">ruleType</span></span>|[<span data-ttu-id="94d1b-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="94d1b-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="94d1b-121">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="94d1b-121">Applicability Rule type.</span></span> <span data-ttu-id="94d1b-122">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="94d1b-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94d1b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="94d1b-123">Relationships</span></span>
<span data-ttu-id="94d1b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94d1b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94d1b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94d1b-125">JSON Representation</span></span>
<span data-ttu-id="94d1b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94d1b-126">Here is a JSON representation of the resource.</span></span>
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



