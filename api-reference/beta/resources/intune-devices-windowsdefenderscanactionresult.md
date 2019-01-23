---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 913c821b60feb4901d812f2055c72e028537dd12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405496"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="82589-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="82589-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="82589-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="82589-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82589-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82589-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82589-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="82589-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82589-107">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="82589-107">Windows Defender last scan result</span></span>


<span data-ttu-id="82589-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82589-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82589-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82589-109">Properties</span></span>
|<span data-ttu-id="82589-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82589-110">Property</span></span>|<span data-ttu-id="82589-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="82589-111">Type</span></span>|<span data-ttu-id="82589-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="82589-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82589-113">actionName</span><span class="sxs-lookup"><span data-stu-id="82589-113">actionName</span></span>|<span data-ttu-id="82589-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82589-114">String</span></span>|<span data-ttu-id="82589-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82589-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="82589-116">actionState</span><span class="sxs-lookup"><span data-stu-id="82589-116">actionState</span></span>|[<span data-ttu-id="82589-117">actionState</span><span class="sxs-lookup"><span data-stu-id="82589-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="82589-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="82589-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="82589-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="82589-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="82589-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="82589-120">startDateTime</span></span>|<span data-ttu-id="82589-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82589-121">DateTimeOffset</span></span>|<span data-ttu-id="82589-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82589-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="82589-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="82589-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="82589-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82589-124">DateTimeOffset</span></span>|<span data-ttu-id="82589-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82589-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="82589-126">scanType</span><span class="sxs-lookup"><span data-stu-id="82589-126">scanType</span></span>|<span data-ttu-id="82589-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82589-127">String</span></span>|<span data-ttu-id="82589-128">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="82589-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="82589-129">Relações</span><span class="sxs-lookup"><span data-stu-id="82589-129">Relationships</span></span>
<span data-ttu-id="82589-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82589-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82589-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82589-131">JSON Representation</span></span>
<span data-ttu-id="82589-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82589-132">Here is a JSON representation of the resource.</span></span>
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




