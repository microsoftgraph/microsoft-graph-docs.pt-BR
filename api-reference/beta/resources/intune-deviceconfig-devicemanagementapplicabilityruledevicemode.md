---
title: tipo de recurso deviceManagementApplicabilityRuleDeviceMode
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6e85a8f634085442a02b47747c508266279e5cc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283592"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="3bd37-103">tipo de recurso deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bd37-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="3bd37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bd37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bd37-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bd37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bd37-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bd37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bd37-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3bd37-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3bd37-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bd37-108">Properties</span></span>
|<span data-ttu-id="3bd37-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bd37-109">Property</span></span>|<span data-ttu-id="3bd37-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bd37-110">Type</span></span>|<span data-ttu-id="3bd37-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bd37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bd37-112">devicemode</span><span class="sxs-lookup"><span data-stu-id="3bd37-112">deviceMode</span></span>|[<span data-ttu-id="3bd37-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="3bd37-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="3bd37-114">Regra de aplicabilidade para o modo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3bd37-114">Applicability rule for device mode.</span></span> <span data-ttu-id="3bd37-115">Os valores possíveis são: `standardConfiguration` e `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="3bd37-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="3bd37-116">nome</span><span class="sxs-lookup"><span data-stu-id="3bd37-116">name</span></span>|<span data-ttu-id="3bd37-117">String</span><span class="sxs-lookup"><span data-stu-id="3bd37-117">String</span></span>|<span data-ttu-id="3bd37-118">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="3bd37-118">Name for object.</span></span>|
|<span data-ttu-id="3bd37-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="3bd37-119">ruleType</span></span>|[<span data-ttu-id="3bd37-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="3bd37-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="3bd37-121">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="3bd37-121">Applicability Rule type.</span></span> <span data-ttu-id="3bd37-122">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="3bd37-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bd37-123">Relações</span><span class="sxs-lookup"><span data-stu-id="3bd37-123">Relationships</span></span>
<span data-ttu-id="3bd37-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bd37-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bd37-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bd37-125">JSON Representation</span></span>
<span data-ttu-id="3bd37-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bd37-126">Here is a JSON representation of the resource.</span></span>
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




