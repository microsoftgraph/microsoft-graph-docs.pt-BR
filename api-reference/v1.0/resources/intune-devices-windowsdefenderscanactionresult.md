---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 857494e6c4e08fe2f659bf26ae63a0be19c17c3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755004"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="3cd55-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="3cd55-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="3cd55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cd55-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cd55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cd55-106">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="3cd55-106">Windows Defender last scan result</span></span>


<span data-ttu-id="3cd55-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3cd55-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3cd55-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cd55-108">Properties</span></span>
|<span data-ttu-id="3cd55-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cd55-109">Property</span></span>|<span data-ttu-id="3cd55-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd55-110">Type</span></span>|<span data-ttu-id="3cd55-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd55-112">actionName</span><span class="sxs-lookup"><span data-stu-id="3cd55-112">actionName</span></span>|<span data-ttu-id="3cd55-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cd55-113">String</span></span>|<span data-ttu-id="3cd55-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3cd55-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3cd55-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3cd55-115">actionState</span></span>|[<span data-ttu-id="3cd55-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3cd55-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3cd55-117">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3cd55-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3cd55-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3cd55-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3cd55-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd55-119">startDateTime</span></span>|<span data-ttu-id="3cd55-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd55-120">DateTimeOffset</span></span>|<span data-ttu-id="3cd55-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3cd55-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3cd55-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd55-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="3cd55-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd55-123">DateTimeOffset</span></span>|<span data-ttu-id="3cd55-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3cd55-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3cd55-125">scanType</span><span class="sxs-lookup"><span data-stu-id="3cd55-125">scanType</span></span>|<span data-ttu-id="3cd55-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cd55-126">String</span></span>|<span data-ttu-id="3cd55-127">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3cd55-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cd55-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3cd55-128">Relationships</span></span>
<span data-ttu-id="3cd55-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3cd55-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cd55-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cd55-130">JSON Representation</span></span>
<span data-ttu-id="3cd55-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cd55-131">Here is a JSON representation of the resource.</span></span>
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




