---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3077d667c5661fd153b8cd165d926671663f07ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968185"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="8cec7-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="8cec7-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="8cec7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cec7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cec7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cec7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cec7-106">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="8cec7-106">Windows Defender last scan result</span></span>


<span data-ttu-id="8cec7-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8cec7-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cec7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cec7-108">Properties</span></span>
|<span data-ttu-id="8cec7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cec7-109">Property</span></span>|<span data-ttu-id="8cec7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cec7-110">Type</span></span>|<span data-ttu-id="8cec7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cec7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cec7-112">actionName</span><span class="sxs-lookup"><span data-stu-id="8cec7-112">actionName</span></span>|<span data-ttu-id="8cec7-113">String</span><span class="sxs-lookup"><span data-stu-id="8cec7-113">String</span></span>|<span data-ttu-id="8cec7-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8cec7-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8cec7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8cec7-115">actionState</span></span>|[<span data-ttu-id="8cec7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8cec7-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8cec7-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8cec7-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8cec7-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8cec7-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8cec7-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8cec7-119">startDateTime</span></span>|<span data-ttu-id="8cec7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cec7-120">DateTimeOffset</span></span>|<span data-ttu-id="8cec7-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8cec7-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8cec7-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cec7-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="8cec7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cec7-123">DateTimeOffset</span></span>|<span data-ttu-id="8cec7-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8cec7-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8cec7-125">scanType</span><span class="sxs-lookup"><span data-stu-id="8cec7-125">scanType</span></span>|<span data-ttu-id="8cec7-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cec7-126">String</span></span>|<span data-ttu-id="8cec7-127">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="8cec7-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cec7-128">Relações</span><span class="sxs-lookup"><span data-stu-id="8cec7-128">Relationships</span></span>
<span data-ttu-id="8cec7-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cec7-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cec7-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cec7-130">JSON Representation</span></span>
<span data-ttu-id="8cec7-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cec7-131">Here is a JSON representation of the resource.</span></span>
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





