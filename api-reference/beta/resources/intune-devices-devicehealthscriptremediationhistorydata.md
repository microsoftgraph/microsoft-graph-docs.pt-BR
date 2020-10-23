---
title: tipo de recurso deviceHealthScriptRemediationHistoryData
description: O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9c04485659482d3f3ad28e3242bfb90b069a1d7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693735"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a><span data-ttu-id="44e4f-103">tipo de recurso deviceHealthScriptRemediationHistoryData</span><span class="sxs-lookup"><span data-stu-id="44e4f-103">deviceHealthScriptRemediationHistoryData resource type</span></span>

<span data-ttu-id="44e4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44e4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44e4f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44e4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44e4f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44e4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44e4f-107">O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data.</span><span class="sxs-lookup"><span data-stu-id="44e4f-107">The number of devices remediated by a device health script on a given date.</span></span>

## <a name="properties"></a><span data-ttu-id="44e4f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44e4f-108">Properties</span></span>
|<span data-ttu-id="44e4f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44e4f-109">Property</span></span>|<span data-ttu-id="44e4f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="44e4f-110">Type</span></span>|<span data-ttu-id="44e4f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="44e4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44e4f-112">data</span><span class="sxs-lookup"><span data-stu-id="44e4f-112">date</span></span>|<span data-ttu-id="44e4f-113">Data</span><span class="sxs-lookup"><span data-stu-id="44e4f-113">Date</span></span>|<span data-ttu-id="44e4f-114">A data em que os dispositivos foram corrigidos pelo script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44e4f-114">The date on which devices were remediated by the device health script.</span></span>|
|<span data-ttu-id="44e4f-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44e4f-115">remediatedDeviceCount</span></span>|<span data-ttu-id="44e4f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="44e4f-116">Int32</span></span>|<span data-ttu-id="44e4f-117">O número de dispositivos corrigidos pelo script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44e4f-117">The number of devices remediated by the device health script.</span></span>|
|<span data-ttu-id="44e4f-118">noIssueDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44e4f-118">noIssueDeviceCount</span></span>|<span data-ttu-id="44e4f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="44e4f-119">Int32</span></span>|<span data-ttu-id="44e4f-120">O número de dispositivos que foram encontrados não têm problema pelo script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44e4f-120">The number of devices that were found to have no issue by the device health script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44e4f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="44e4f-121">Relationships</span></span>
<span data-ttu-id="44e4f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44e4f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44e4f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44e4f-123">JSON Representation</span></span>
<span data-ttu-id="44e4f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44e4f-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```





