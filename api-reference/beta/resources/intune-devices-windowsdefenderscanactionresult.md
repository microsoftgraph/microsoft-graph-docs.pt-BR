---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2774052035c99dc2616532d5a3997fb5f4e05906
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208167"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="ce880-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="ce880-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="ce880-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce880-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce880-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce880-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce880-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce880-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce880-107">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="ce880-107">Windows Defender last scan result</span></span>


<span data-ttu-id="ce880-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce880-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce880-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce880-109">Properties</span></span>
|<span data-ttu-id="ce880-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce880-110">Property</span></span>|<span data-ttu-id="ce880-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce880-111">Type</span></span>|<span data-ttu-id="ce880-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce880-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce880-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ce880-113">actionName</span></span>|<span data-ttu-id="ce880-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce880-114">String</span></span>|<span data-ttu-id="ce880-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce880-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ce880-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ce880-116">actionState</span></span>|[<span data-ttu-id="ce880-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ce880-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ce880-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ce880-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ce880-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ce880-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ce880-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ce880-120">startDateTime</span></span>|<span data-ttu-id="ce880-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce880-121">DateTimeOffset</span></span>|<span data-ttu-id="ce880-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce880-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ce880-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce880-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ce880-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce880-124">DateTimeOffset</span></span>|<span data-ttu-id="ce880-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce880-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ce880-126">scanType</span><span class="sxs-lookup"><span data-stu-id="ce880-126">scanType</span></span>|<span data-ttu-id="ce880-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce880-127">String</span></span>|<span data-ttu-id="ce880-128">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ce880-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce880-129">Relações</span><span class="sxs-lookup"><span data-stu-id="ce880-129">Relationships</span></span>
<span data-ttu-id="ce880-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce880-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce880-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce880-131">JSON Representation</span></span>
<span data-ttu-id="ce880-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce880-132">Here is a JSON representation of the resource.</span></span>
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




