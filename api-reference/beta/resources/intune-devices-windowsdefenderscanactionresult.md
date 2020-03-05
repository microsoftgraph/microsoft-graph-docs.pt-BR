---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e26904504d882af0ed253b547709a29e075954c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528427"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="28e3d-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="28e3d-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="28e3d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="28e3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28e3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28e3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28e3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28e3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28e3d-107">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="28e3d-107">Windows Defender last scan result</span></span>


<span data-ttu-id="28e3d-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="28e3d-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28e3d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28e3d-109">Properties</span></span>
|<span data-ttu-id="28e3d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28e3d-110">Property</span></span>|<span data-ttu-id="28e3d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="28e3d-111">Type</span></span>|<span data-ttu-id="28e3d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e3d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28e3d-113">actionName</span><span class="sxs-lookup"><span data-stu-id="28e3d-113">actionName</span></span>|<span data-ttu-id="28e3d-114">String</span><span class="sxs-lookup"><span data-stu-id="28e3d-114">String</span></span>|<span data-ttu-id="28e3d-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="28e3d-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="28e3d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="28e3d-116">actionState</span></span>|[<span data-ttu-id="28e3d-117">actionState</span><span class="sxs-lookup"><span data-stu-id="28e3d-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="28e3d-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="28e3d-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="28e3d-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="28e3d-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="28e3d-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="28e3d-120">startDateTime</span></span>|<span data-ttu-id="28e3d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e3d-121">DateTimeOffset</span></span>|<span data-ttu-id="28e3d-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="28e3d-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="28e3d-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="28e3d-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="28e3d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e3d-124">DateTimeOffset</span></span>|<span data-ttu-id="28e3d-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="28e3d-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="28e3d-126">scanType</span><span class="sxs-lookup"><span data-stu-id="28e3d-126">scanType</span></span>|<span data-ttu-id="28e3d-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e3d-127">String</span></span>|<span data-ttu-id="28e3d-128">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="28e3d-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="28e3d-129">Relações</span><span class="sxs-lookup"><span data-stu-id="28e3d-129">Relationships</span></span>
<span data-ttu-id="28e3d-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28e3d-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28e3d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28e3d-131">JSON Representation</span></span>
<span data-ttu-id="28e3d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28e3d-132">Here is a JSON representation of the resource.</span></span>
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



