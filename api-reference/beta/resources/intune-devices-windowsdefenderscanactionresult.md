---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9fcddceae21218978b121ae8b5749c739f3d105
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080744"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="ecbba-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="ecbba-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="ecbba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecbba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecbba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecbba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecbba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecbba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecbba-107">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="ecbba-107">Windows Defender last scan result</span></span>


<span data-ttu-id="ecbba-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecbba-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ecbba-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecbba-109">Properties</span></span>
|<span data-ttu-id="ecbba-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecbba-110">Property</span></span>|<span data-ttu-id="ecbba-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecbba-111">Type</span></span>|<span data-ttu-id="ecbba-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecbba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecbba-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ecbba-113">actionName</span></span>|<span data-ttu-id="ecbba-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecbba-114">String</span></span>|<span data-ttu-id="ecbba-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecbba-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ecbba-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ecbba-116">actionState</span></span>|[<span data-ttu-id="ecbba-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ecbba-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ecbba-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ecbba-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ecbba-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ecbba-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ecbba-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ecbba-120">startDateTime</span></span>|<span data-ttu-id="ecbba-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbba-121">DateTimeOffset</span></span>|<span data-ttu-id="ecbba-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecbba-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ecbba-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecbba-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ecbba-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbba-124">DateTimeOffset</span></span>|<span data-ttu-id="ecbba-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecbba-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ecbba-126">scanType</span><span class="sxs-lookup"><span data-stu-id="ecbba-126">scanType</span></span>|<span data-ttu-id="ecbba-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecbba-127">String</span></span>|<span data-ttu-id="ecbba-128">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ecbba-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecbba-129">Relações</span><span class="sxs-lookup"><span data-stu-id="ecbba-129">Relationships</span></span>
<span data-ttu-id="ecbba-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ecbba-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecbba-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecbba-131">JSON Representation</span></span>
<span data-ttu-id="ecbba-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ecbba-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```






