---
title: tipo de recurso deviceManagementApplicabilityRuleDeviceMode
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f53d9f676dd50c49fc5222f50c24c2c9a6d08e22
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332859"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="b5f9b-103">tipo de recurso deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5f9b-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="b5f9b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5f9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5f9b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5f9b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b5f9b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5f9b-107">Properties</span></span>
|<span data-ttu-id="b5f9b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5f9b-108">Property</span></span>|<span data-ttu-id="b5f9b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5f9b-109">Type</span></span>|<span data-ttu-id="b5f9b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f9b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5f9b-111">devicemode</span><span class="sxs-lookup"><span data-stu-id="b5f9b-111">deviceMode</span></span>|[<span data-ttu-id="b5f9b-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="b5f9b-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="b5f9b-113">Regra de aplicabilidade para o modo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-113">Applicability rule for device mode.</span></span> <span data-ttu-id="b5f9b-114">Os valores possíveis são: `standardConfiguration` e `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="b5f9b-115">name</span><span class="sxs-lookup"><span data-stu-id="b5f9b-115">name</span></span>|<span data-ttu-id="b5f9b-116">String</span><span class="sxs-lookup"><span data-stu-id="b5f9b-116">String</span></span>|<span data-ttu-id="b5f9b-117">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-117">Name for object.</span></span>|
|<span data-ttu-id="b5f9b-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="b5f9b-118">ruleType</span></span>|[<span data-ttu-id="b5f9b-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="b5f9b-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="b5f9b-120">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-120">Applicability Rule type.</span></span> <span data-ttu-id="b5f9b-121">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5f9b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b5f9b-122">Relationships</span></span>
<span data-ttu-id="b5f9b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5f9b-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5f9b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5f9b-124">JSON Representation</span></span>
<span data-ttu-id="b5f9b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5f9b-125">Here is a JSON representation of the resource.</span></span>
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



