---
title: tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7dd3a1b1ab22c2ac834150d1e1ad09938ed27550
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299426"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="ebdd9-103">tipo de recurso deviceHealthScriptRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="ebdd9-103">deviceHealthScriptRemediationSummary resource type</span></span>

<span data-ttu-id="ebdd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebdd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebdd9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebdd9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebdd9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebdd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebdd9-107">O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.</span><span class="sxs-lookup"><span data-stu-id="ebdd9-107">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="ebdd9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebdd9-108">Properties</span></span>
|<span data-ttu-id="ebdd9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebdd9-109">Property</span></span>|<span data-ttu-id="ebdd9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebdd9-110">Type</span></span>|<span data-ttu-id="ebdd9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebdd9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebdd9-112">scriptCount</span><span class="sxs-lookup"><span data-stu-id="ebdd9-112">scriptCount</span></span>|<span data-ttu-id="ebdd9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdd9-113">Int32</span></span>|<span data-ttu-id="ebdd9-114">O número de scripts de integridade do dispositivo implantados.</span><span class="sxs-lookup"><span data-stu-id="ebdd9-114">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="ebdd9-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebdd9-115">remediatedDeviceCount</span></span>|<span data-ttu-id="ebdd9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdd9-116">Int32</span></span>|<span data-ttu-id="ebdd9-117">O número de dispositivos corrigidos por scripts de integridade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebdd9-117">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebdd9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ebdd9-118">Relationships</span></span>
<span data-ttu-id="ebdd9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebdd9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebdd9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebdd9-120">JSON Representation</span></span>
<span data-ttu-id="ebdd9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebdd9-121">Here is a JSON representation of the resource.</span></span>
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




