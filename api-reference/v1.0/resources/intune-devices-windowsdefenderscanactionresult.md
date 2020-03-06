---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3fce56be7dcc0d1262bb65420d6ce3986cce1fe3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530268"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="e1b85-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="e1b85-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="e1b85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1b85-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b85-106">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="e1b85-106">Windows Defender last scan result</span></span>


<span data-ttu-id="e1b85-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1b85-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1b85-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1b85-108">Properties</span></span>
|<span data-ttu-id="e1b85-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1b85-109">Property</span></span>|<span data-ttu-id="e1b85-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1b85-110">Type</span></span>|<span data-ttu-id="e1b85-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b85-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e1b85-112">actionName</span></span>|<span data-ttu-id="e1b85-113">String</span><span class="sxs-lookup"><span data-stu-id="e1b85-113">String</span></span>|<span data-ttu-id="e1b85-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1b85-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e1b85-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e1b85-115">actionState</span></span>|[<span data-ttu-id="e1b85-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e1b85-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="e1b85-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="e1b85-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e1b85-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e1b85-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e1b85-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e1b85-119">startDateTime</span></span>|<span data-ttu-id="e1b85-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1b85-120">DateTimeOffset</span></span>|<span data-ttu-id="e1b85-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1b85-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e1b85-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1b85-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e1b85-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1b85-123">DateTimeOffset</span></span>|<span data-ttu-id="e1b85-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1b85-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e1b85-125">scanType</span><span class="sxs-lookup"><span data-stu-id="e1b85-125">scanType</span></span>|<span data-ttu-id="e1b85-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1b85-126">String</span></span>|<span data-ttu-id="e1b85-127">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="e1b85-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1b85-128">Relações</span><span class="sxs-lookup"><span data-stu-id="e1b85-128">Relationships</span></span>
<span data-ttu-id="e1b85-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1b85-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1b85-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1b85-130">JSON Representation</span></span>
<span data-ttu-id="e1b85-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1b85-131">Here is a JSON representation of the resource.</span></span>
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




