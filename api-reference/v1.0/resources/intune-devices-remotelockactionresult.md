---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fcf663ad633f09a1198c901ffa1b82c2278b3ba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406823"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="d0447-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="d0447-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="d0447-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0447-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0447-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0447-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0447-106">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="d0447-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="d0447-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0447-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0447-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0447-108">Properties</span></span>
|<span data-ttu-id="d0447-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0447-109">Property</span></span>|<span data-ttu-id="d0447-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0447-110">Type</span></span>|<span data-ttu-id="d0447-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0447-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0447-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d0447-112">actionName</span></span>|<span data-ttu-id="d0447-113">String</span><span class="sxs-lookup"><span data-stu-id="d0447-113">String</span></span>|<span data-ttu-id="d0447-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0447-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0447-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d0447-115">actionState</span></span>|[<span data-ttu-id="d0447-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d0447-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="d0447-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d0447-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d0447-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d0447-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d0447-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d0447-119">startDateTime</span></span>|<span data-ttu-id="d0447-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0447-120">DateTimeOffset</span></span>|<span data-ttu-id="d0447-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0447-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0447-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0447-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d0447-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0447-123">DateTimeOffset</span></span>|<span data-ttu-id="d0447-124">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0447-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0447-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="d0447-125">unlockPin</span></span>|<span data-ttu-id="d0447-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0447-126">String</span></span>|<span data-ttu-id="d0447-127">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="d0447-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0447-128">Relações</span><span class="sxs-lookup"><span data-stu-id="d0447-128">Relationships</span></span>
<span data-ttu-id="d0447-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0447-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0447-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0447-130">JSON Representation</span></span>
<span data-ttu-id="d0447-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0447-131">Here is a JSON representation of the resource.</span></span>
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







