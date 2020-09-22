---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f6de49d6a87a2f385b4d6c29f3442286c63beb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091009"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="abad6-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="abad6-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="abad6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abad6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abad6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abad6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abad6-106">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="abad6-106">Windows Defender last scan result</span></span>


<span data-ttu-id="abad6-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="abad6-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="abad6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abad6-108">Properties</span></span>
|<span data-ttu-id="abad6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abad6-109">Property</span></span>|<span data-ttu-id="abad6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="abad6-110">Type</span></span>|<span data-ttu-id="abad6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="abad6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abad6-112">actionName</span><span class="sxs-lookup"><span data-stu-id="abad6-112">actionName</span></span>|<span data-ttu-id="abad6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abad6-113">String</span></span>|<span data-ttu-id="abad6-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="abad6-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="abad6-115">actionState</span><span class="sxs-lookup"><span data-stu-id="abad6-115">actionState</span></span>|[<span data-ttu-id="abad6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="abad6-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="abad6-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="abad6-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="abad6-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="abad6-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="abad6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="abad6-119">startDateTime</span></span>|<span data-ttu-id="abad6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abad6-120">DateTimeOffset</span></span>|<span data-ttu-id="abad6-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="abad6-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="abad6-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="abad6-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="abad6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abad6-123">DateTimeOffset</span></span>|<span data-ttu-id="abad6-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="abad6-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="abad6-125">scanType</span><span class="sxs-lookup"><span data-stu-id="abad6-125">scanType</span></span>|<span data-ttu-id="abad6-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abad6-126">String</span></span>|<span data-ttu-id="abad6-127">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="abad6-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="abad6-128">Relações</span><span class="sxs-lookup"><span data-stu-id="abad6-128">Relationships</span></span>
<span data-ttu-id="abad6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="abad6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="abad6-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abad6-130">JSON Representation</span></span>
<span data-ttu-id="abad6-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abad6-131">Here is a JSON representation of the resource.</span></span>
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









