---
title: Tipo de recurso windowsDefenderScanActionResult
description: Resultado da última verificação do Windows Defender
author: tfitzmac
ms.openlocfilehash: fa988a971925cf61db0ab9f7e962162565e8a4b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323034"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="c7b5e-103">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="c7b5e-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="c7b5e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7b5e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7b5e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7b5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7b5e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7b5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7b5e-107">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="c7b5e-107">Windows Defender last scan result</span></span>

<span data-ttu-id="c7b5e-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7b5e-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7b5e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7b5e-109">Properties</span></span>
|<span data-ttu-id="c7b5e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7b5e-110">Property</span></span>|<span data-ttu-id="c7b5e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7b5e-111">Type</span></span>|<span data-ttu-id="c7b5e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7b5e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7b5e-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c7b5e-113">actionName</span></span>|<span data-ttu-id="c7b5e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7b5e-114">String</span></span>|<span data-ttu-id="c7b5e-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7b5e-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c7b5e-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c7b5e-116">actionState</span></span>|[<span data-ttu-id="c7b5e-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c7b5e-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c7b5e-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c7b5e-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c7b5e-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c7b5e-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c7b5e-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7b5e-120">startDateTime</span></span>|<span data-ttu-id="c7b5e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7b5e-121">DateTimeOffset</span></span>|<span data-ttu-id="c7b5e-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7b5e-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c7b5e-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7b5e-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c7b5e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7b5e-124">DateTimeOffset</span></span>|<span data-ttu-id="c7b5e-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7b5e-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c7b5e-126">scanType</span><span class="sxs-lookup"><span data-stu-id="c7b5e-126">scanType</span></span>|<span data-ttu-id="c7b5e-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7b5e-127">String</span></span>|<span data-ttu-id="c7b5e-128">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="c7b5e-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7b5e-129">Relações</span><span class="sxs-lookup"><span data-stu-id="c7b5e-129">Relationships</span></span>
<span data-ttu-id="c7b5e-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7b5e-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7b5e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7b5e-131">JSON Representation</span></span>
<span data-ttu-id="c7b5e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7b5e-132">Here is a JSON representation of the resource.</span></span>
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





