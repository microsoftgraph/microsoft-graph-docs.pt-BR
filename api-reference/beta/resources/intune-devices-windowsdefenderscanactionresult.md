---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b54feb06e18e0ea772ab69e2ed3bd138564cfc08
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789007"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="16686-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="16686-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="16686-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16686-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16686-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16686-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16686-106">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="16686-106">Windows Defender last scan result</span></span>


<span data-ttu-id="16686-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="16686-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16686-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16686-108">Properties</span></span>
|<span data-ttu-id="16686-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16686-109">Property</span></span>|<span data-ttu-id="16686-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="16686-110">Type</span></span>|<span data-ttu-id="16686-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="16686-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16686-112">actionName</span><span class="sxs-lookup"><span data-stu-id="16686-112">actionName</span></span>|<span data-ttu-id="16686-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16686-113">String</span></span>|<span data-ttu-id="16686-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="16686-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="16686-115">actionState</span><span class="sxs-lookup"><span data-stu-id="16686-115">actionState</span></span>|[<span data-ttu-id="16686-116">actionState</span><span class="sxs-lookup"><span data-stu-id="16686-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="16686-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="16686-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="16686-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="16686-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="16686-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="16686-119">startDateTime</span></span>|<span data-ttu-id="16686-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16686-120">DateTimeOffset</span></span>|<span data-ttu-id="16686-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="16686-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="16686-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="16686-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="16686-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16686-123">DateTimeOffset</span></span>|<span data-ttu-id="16686-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="16686-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="16686-125">scanType</span><span class="sxs-lookup"><span data-stu-id="16686-125">scanType</span></span>|<span data-ttu-id="16686-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16686-126">String</span></span>|<span data-ttu-id="16686-127">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="16686-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="16686-128">Relações</span><span class="sxs-lookup"><span data-stu-id="16686-128">Relationships</span></span>
<span data-ttu-id="16686-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="16686-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16686-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16686-130">JSON Representation</span></span>
<span data-ttu-id="16686-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16686-131">Here is a JSON representation of the resource.</span></span>
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





