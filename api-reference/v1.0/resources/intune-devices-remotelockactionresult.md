---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cba3a5ab51f5283ce6f3ca61f7cda992eeca5b8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855150"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="4e91c-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="4e91c-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="4e91c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4e91c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e91c-105">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="4e91c-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="4e91c-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e91c-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e91c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e91c-107">Properties</span></span>
|<span data-ttu-id="4e91c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e91c-108">Property</span></span>|<span data-ttu-id="4e91c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e91c-109">Type</span></span>|<span data-ttu-id="4e91c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e91c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e91c-111">actionName</span><span class="sxs-lookup"><span data-stu-id="4e91c-111">actionName</span></span>|<span data-ttu-id="4e91c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e91c-112">String</span></span>|<span data-ttu-id="4e91c-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e91c-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e91c-114">actionState</span><span class="sxs-lookup"><span data-stu-id="4e91c-114">actionState</span></span>|[<span data-ttu-id="4e91c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4e91c-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="4e91c-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4e91c-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4e91c-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4e91c-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4e91c-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e91c-118">startDateTime</span></span>|<span data-ttu-id="4e91c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e91c-119">DateTimeOffset</span></span>|<span data-ttu-id="4e91c-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e91c-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e91c-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e91c-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="4e91c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e91c-122">DateTimeOffset</span></span>|<span data-ttu-id="4e91c-123">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e91c-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e91c-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="4e91c-124">unlockPin</span></span>|<span data-ttu-id="4e91c-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e91c-125">String</span></span>|<span data-ttu-id="4e91c-126">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="4e91c-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e91c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="4e91c-127">Relationships</span></span>
<span data-ttu-id="4e91c-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e91c-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e91c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e91c-129">JSON Representation</span></span>
<span data-ttu-id="4e91c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e91c-130">Here is a JSON representation of the resource.</span></span>
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



