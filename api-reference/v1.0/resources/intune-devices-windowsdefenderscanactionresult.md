---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 407db79fa0caf333dfb092620320aeb339e1b195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812149"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="3bc20-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="3bc20-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="3bc20-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3bc20-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bc20-105">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="3bc20-105">Windows Defender last scan result</span></span>

<span data-ttu-id="3bc20-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc20-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3bc20-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bc20-107">Properties</span></span>
|<span data-ttu-id="3bc20-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bc20-108">Property</span></span>|<span data-ttu-id="3bc20-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bc20-109">Type</span></span>|<span data-ttu-id="3bc20-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bc20-111">actionName</span><span class="sxs-lookup"><span data-stu-id="3bc20-111">actionName</span></span>|<span data-ttu-id="3bc20-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bc20-112">String</span></span>|<span data-ttu-id="3bc20-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc20-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3bc20-114">actionState</span><span class="sxs-lookup"><span data-stu-id="3bc20-114">actionState</span></span>|[<span data-ttu-id="3bc20-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3bc20-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3bc20-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3bc20-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3bc20-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3bc20-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3bc20-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc20-118">startDateTime</span></span>|<span data-ttu-id="3bc20-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc20-119">DateTimeOffset</span></span>|<span data-ttu-id="3bc20-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc20-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3bc20-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc20-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="3bc20-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc20-122">DateTimeOffset</span></span>|<span data-ttu-id="3bc20-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc20-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3bc20-124">scanType</span><span class="sxs-lookup"><span data-stu-id="3bc20-124">scanType</span></span>|<span data-ttu-id="3bc20-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bc20-125">String</span></span>|<span data-ttu-id="3bc20-126">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3bc20-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bc20-127">Relações</span><span class="sxs-lookup"><span data-stu-id="3bc20-127">Relationships</span></span>
<span data-ttu-id="3bc20-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bc20-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3bc20-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bc20-129">JSON Representation</span></span>
<span data-ttu-id="3bc20-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bc20-130">Here is a JSON representation of the resource.</span></span>
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



