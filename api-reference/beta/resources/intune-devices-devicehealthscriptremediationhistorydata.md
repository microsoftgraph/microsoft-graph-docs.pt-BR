---
title: tipo de recurso deviceHealthScriptRemediationHistoryData
description: O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d1940328e9690414dc9ce4b4958f6f5e34751b1b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259988"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a><span data-ttu-id="b32da-103">tipo de recurso deviceHealthScriptRemediationHistoryData</span><span class="sxs-lookup"><span data-stu-id="b32da-103">deviceHealthScriptRemediationHistoryData resource type</span></span>

<span data-ttu-id="b32da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b32da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b32da-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b32da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b32da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b32da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b32da-107">O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data.</span><span class="sxs-lookup"><span data-stu-id="b32da-107">The number of devices remediated by a device health script on a given date.</span></span>

## <a name="properties"></a><span data-ttu-id="b32da-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b32da-108">Properties</span></span>
|<span data-ttu-id="b32da-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b32da-109">Property</span></span>|<span data-ttu-id="b32da-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b32da-110">Type</span></span>|<span data-ttu-id="b32da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b32da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b32da-112">data</span><span class="sxs-lookup"><span data-stu-id="b32da-112">date</span></span>|<span data-ttu-id="b32da-113">Data</span><span class="sxs-lookup"><span data-stu-id="b32da-113">Date</span></span>|<span data-ttu-id="b32da-114">A data em que os dispositivos foram corrigidos pelo script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b32da-114">The date on which devices were remediated by the device health script.</span></span>|
|<span data-ttu-id="b32da-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b32da-115">remediatedDeviceCount</span></span>|<span data-ttu-id="b32da-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b32da-116">Int32</span></span>|<span data-ttu-id="b32da-117">O número de dispositivos corrigidos pelo script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b32da-117">The number of devices remediated by the device health script.</span></span>|
|<span data-ttu-id="b32da-118">noIssueDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b32da-118">noIssueDeviceCount</span></span>|<span data-ttu-id="b32da-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b32da-119">Int32</span></span>|<span data-ttu-id="b32da-120">O número de dispositivos que foram encontrados não têm problema pelo script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b32da-120">The number of devices that were found to have no issue by the device health script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b32da-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b32da-121">Relationships</span></span>
<span data-ttu-id="b32da-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b32da-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b32da-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b32da-123">JSON Representation</span></span>
<span data-ttu-id="b32da-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b32da-124">Here is a JSON representation of the resource.</span></span>
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




