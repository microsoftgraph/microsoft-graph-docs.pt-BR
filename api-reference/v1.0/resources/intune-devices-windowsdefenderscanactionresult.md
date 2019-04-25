---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20d30ebda6e24f26406d189ebd980e558bf74e83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523347"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="91a16-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="91a16-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="91a16-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91a16-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91a16-105">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="91a16-105">Windows Defender last scan result</span></span>


<span data-ttu-id="91a16-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="91a16-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91a16-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91a16-107">Properties</span></span>
|<span data-ttu-id="91a16-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91a16-108">Property</span></span>|<span data-ttu-id="91a16-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="91a16-109">Type</span></span>|<span data-ttu-id="91a16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="91a16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a16-111">actionName</span><span class="sxs-lookup"><span data-stu-id="91a16-111">actionName</span></span>|<span data-ttu-id="91a16-112">String</span><span class="sxs-lookup"><span data-stu-id="91a16-112">String</span></span>|<span data-ttu-id="91a16-113">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="91a16-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="91a16-114">actionState</span><span class="sxs-lookup"><span data-stu-id="91a16-114">actionState</span></span>|[<span data-ttu-id="91a16-115">actionState</span><span class="sxs-lookup"><span data-stu-id="91a16-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="91a16-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="91a16-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="91a16-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="91a16-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="91a16-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="91a16-118">startDateTime</span></span>|<span data-ttu-id="91a16-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91a16-119">DateTimeOffset</span></span>|<span data-ttu-id="91a16-120">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="91a16-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="91a16-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="91a16-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="91a16-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91a16-122">DateTimeOffset</span></span>|<span data-ttu-id="91a16-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="91a16-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="91a16-124">scanType</span><span class="sxs-lookup"><span data-stu-id="91a16-124">scanType</span></span>|<span data-ttu-id="91a16-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91a16-125">String</span></span>|<span data-ttu-id="91a16-126">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="91a16-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="91a16-127">Relações</span><span class="sxs-lookup"><span data-stu-id="91a16-127">Relationships</span></span>
<span data-ttu-id="91a16-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91a16-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91a16-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91a16-129">JSON Representation</span></span>
<span data-ttu-id="91a16-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91a16-130">Here is a JSON representation of the resource.</span></span>
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



