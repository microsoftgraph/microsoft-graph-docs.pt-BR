---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f0d0296442ebb9c67dea8dc87b1a42bd980c92c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406816"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="3c2a6-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="3c2a6-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="3c2a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c2a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c2a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c2a6-106">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="3c2a6-106">Windows Defender last scan result</span></span>


<span data-ttu-id="3c2a6-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3c2a6-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3c2a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c2a6-108">Properties</span></span>
|<span data-ttu-id="3c2a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c2a6-109">Property</span></span>|<span data-ttu-id="3c2a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c2a6-110">Type</span></span>|<span data-ttu-id="3c2a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c2a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c2a6-112">actionName</span><span class="sxs-lookup"><span data-stu-id="3c2a6-112">actionName</span></span>|<span data-ttu-id="3c2a6-113">String</span><span class="sxs-lookup"><span data-stu-id="3c2a6-113">String</span></span>|<span data-ttu-id="3c2a6-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3c2a6-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3c2a6-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3c2a6-115">actionState</span></span>|[<span data-ttu-id="3c2a6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3c2a6-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3c2a6-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3c2a6-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3c2a6-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3c2a6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2a6-119">startDateTime</span></span>|<span data-ttu-id="3c2a6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c2a6-120">DateTimeOffset</span></span>|<span data-ttu-id="3c2a6-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3c2a6-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3c2a6-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2a6-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="3c2a6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c2a6-123">DateTimeOffset</span></span>|<span data-ttu-id="3c2a6-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3c2a6-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3c2a6-125">scanType</span><span class="sxs-lookup"><span data-stu-id="3c2a6-125">scanType</span></span>|<span data-ttu-id="3c2a6-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c2a6-126">String</span></span>|<span data-ttu-id="3c2a6-127">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3c2a6-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c2a6-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3c2a6-128">Relationships</span></span>
<span data-ttu-id="3c2a6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c2a6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c2a6-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c2a6-130">JSON Representation</span></span>
<span data-ttu-id="3c2a6-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-131">Here is a JSON representation of the resource.</span></span>
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







