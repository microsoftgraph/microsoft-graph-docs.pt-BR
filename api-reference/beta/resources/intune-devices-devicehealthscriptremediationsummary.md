---
title: tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06e48973305dbbdf7ae276e4d14d3307da74c36e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060284"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="e1325-103">tipo de recurso deviceHealthScriptRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="e1325-103">deviceHealthScriptRemediationSummary resource type</span></span>

<span data-ttu-id="e1325-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1325-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1325-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1325-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1325-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1325-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1325-107">O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.</span><span class="sxs-lookup"><span data-stu-id="e1325-107">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="e1325-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1325-108">Properties</span></span>
|<span data-ttu-id="e1325-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1325-109">Property</span></span>|<span data-ttu-id="e1325-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1325-110">Type</span></span>|<span data-ttu-id="e1325-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1325-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1325-112">scriptCount</span><span class="sxs-lookup"><span data-stu-id="e1325-112">scriptCount</span></span>|<span data-ttu-id="e1325-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e1325-113">Int32</span></span>|<span data-ttu-id="e1325-114">O número de scripts de integridade do dispositivo implantados.</span><span class="sxs-lookup"><span data-stu-id="e1325-114">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="e1325-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1325-115">remediatedDeviceCount</span></span>|<span data-ttu-id="e1325-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e1325-116">Int32</span></span>|<span data-ttu-id="e1325-117">O número de dispositivos corrigidos por scripts de integridade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1325-117">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1325-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e1325-118">Relationships</span></span>
<span data-ttu-id="e1325-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1325-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1325-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1325-120">JSON Representation</span></span>
<span data-ttu-id="e1325-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1325-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```






