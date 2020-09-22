---
title: tipo de recurso deviceHealthScriptRemediationHistory
description: O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data com o horário da última modificação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51f85549ecceb1a867bd08f5ef21b223a22c3f67
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060304"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a><span data-ttu-id="e6c5d-103">tipo de recurso deviceHealthScriptRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="e6c5d-103">deviceHealthScriptRemediationHistory resource type</span></span>

<span data-ttu-id="e6c5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6c5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6c5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6c5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6c5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6c5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6c5d-107">O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data com o horário da última modificação.</span><span class="sxs-lookup"><span data-stu-id="e6c5d-107">The number of devices remediated by a device health script on a given date with the last modified time.</span></span>

## <a name="properties"></a><span data-ttu-id="e6c5d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6c5d-108">Properties</span></span>
|<span data-ttu-id="e6c5d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6c5d-109">Property</span></span>|<span data-ttu-id="e6c5d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6c5d-110">Type</span></span>|<span data-ttu-id="e6c5d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6c5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6c5d-112">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6c5d-112">lastModifiedDateTime</span></span>|<span data-ttu-id="e6c5d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6c5d-113">DateTimeOffset</span></span>|<span data-ttu-id="e6c5d-114">A data na qual o histórico de resultados é calculado para o healthscript.</span><span class="sxs-lookup"><span data-stu-id="e6c5d-114">The date on which the results history is calculated for the healthscript.</span></span>|
|<span data-ttu-id="e6c5d-115">historyData</span><span class="sxs-lookup"><span data-stu-id="e6c5d-115">historyData</span></span>|<span data-ttu-id="e6c5d-116">coleção [deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md)</span><span class="sxs-lookup"><span data-stu-id="e6c5d-116">[deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md) collection</span></span>|<span data-ttu-id="e6c5d-117">O número de dispositivos corrigidos pelo script de integridade do dispositivo na data especificada.</span><span class="sxs-lookup"><span data-stu-id="e6c5d-117">The number of devices remediated by the device health script on the given date.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6c5d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e6c5d-118">Relationships</span></span>
<span data-ttu-id="e6c5d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6c5d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6c5d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6c5d-120">JSON Representation</span></span>
<span data-ttu-id="e6c5d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6c5d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
      "date": "String (Date)",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```






