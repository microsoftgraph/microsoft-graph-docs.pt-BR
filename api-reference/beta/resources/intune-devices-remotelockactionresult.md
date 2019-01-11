---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0feb3c4474e543b4da462ddab499c4e8fff5f0cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875338"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="985d0-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="985d0-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="985d0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="985d0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="985d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="985d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="985d0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="985d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="985d0-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="985d0-107">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="985d0-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="985d0-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="985d0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="985d0-109">Properties</span></span>
|<span data-ttu-id="985d0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="985d0-110">Property</span></span>|<span data-ttu-id="985d0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="985d0-111">Type</span></span>|<span data-ttu-id="985d0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="985d0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="985d0-113">actionName</span><span class="sxs-lookup"><span data-stu-id="985d0-113">actionName</span></span>|<span data-ttu-id="985d0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="985d0-114">String</span></span>|<span data-ttu-id="985d0-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="985d0-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="985d0-116">actionState</span><span class="sxs-lookup"><span data-stu-id="985d0-116">actionState</span></span>|[<span data-ttu-id="985d0-117">actionState</span><span class="sxs-lookup"><span data-stu-id="985d0-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="985d0-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="985d0-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="985d0-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="985d0-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="985d0-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="985d0-120">startDateTime</span></span>|<span data-ttu-id="985d0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985d0-121">DateTimeOffset</span></span>|<span data-ttu-id="985d0-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="985d0-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="985d0-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="985d0-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="985d0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985d0-124">DateTimeOffset</span></span>|<span data-ttu-id="985d0-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="985d0-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="985d0-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="985d0-126">unlockPin</span></span>|<span data-ttu-id="985d0-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="985d0-127">String</span></span>|<span data-ttu-id="985d0-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="985d0-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="985d0-129">Relações</span><span class="sxs-lookup"><span data-stu-id="985d0-129">Relationships</span></span>
<span data-ttu-id="985d0-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="985d0-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="985d0-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="985d0-131">JSON Representation</span></span>
<span data-ttu-id="985d0-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="985d0-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```





