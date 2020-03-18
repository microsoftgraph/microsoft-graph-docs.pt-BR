---
title: tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b59f2d057f258e60a8182194c1ac930e95012b93
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784941"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="78e23-103">tipo de recurso deviceHealthScriptRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="78e23-103">deviceHealthScriptRemediationSummary resource type</span></span>

> <span data-ttu-id="78e23-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78e23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78e23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e23-106">O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.</span><span class="sxs-lookup"><span data-stu-id="78e23-106">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="78e23-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78e23-107">Properties</span></span>
|<span data-ttu-id="78e23-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78e23-108">Property</span></span>|<span data-ttu-id="78e23-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="78e23-109">Type</span></span>|<span data-ttu-id="78e23-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e23-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e23-111">scriptCount</span><span class="sxs-lookup"><span data-stu-id="78e23-111">scriptCount</span></span>|<span data-ttu-id="78e23-112">Int32</span><span class="sxs-lookup"><span data-stu-id="78e23-112">Int32</span></span>|<span data-ttu-id="78e23-113">O número de scripts de integridade do dispositivo implantados.</span><span class="sxs-lookup"><span data-stu-id="78e23-113">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="78e23-114">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78e23-114">remediatedDeviceCount</span></span>|<span data-ttu-id="78e23-115">Int32</span><span class="sxs-lookup"><span data-stu-id="78e23-115">Int32</span></span>|<span data-ttu-id="78e23-116">O número de dispositivos corrigidos por scripts de integridade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="78e23-116">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e23-117">Relações</span><span class="sxs-lookup"><span data-stu-id="78e23-117">Relationships</span></span>
<span data-ttu-id="78e23-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78e23-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78e23-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78e23-119">JSON Representation</span></span>
<span data-ttu-id="78e23-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78e23-120">Here is a JSON representation of the resource.</span></span>
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



