---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f90cbc46ca4bc9476ad5d9386581385ae7354261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159021"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="65096-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="65096-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="65096-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65096-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65096-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65096-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65096-106">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="65096-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="65096-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65096-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65096-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65096-108">Properties</span></span>
|<span data-ttu-id="65096-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65096-109">Property</span></span>|<span data-ttu-id="65096-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65096-110">Type</span></span>|<span data-ttu-id="65096-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65096-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65096-112">actionName</span><span class="sxs-lookup"><span data-stu-id="65096-112">actionName</span></span>|<span data-ttu-id="65096-113">String</span><span class="sxs-lookup"><span data-stu-id="65096-113">String</span></span>|<span data-ttu-id="65096-114">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65096-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="65096-115">actionState</span><span class="sxs-lookup"><span data-stu-id="65096-115">actionState</span></span>|[<span data-ttu-id="65096-116">actionState</span><span class="sxs-lookup"><span data-stu-id="65096-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="65096-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="65096-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="65096-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="65096-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="65096-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="65096-119">startDateTime</span></span>|<span data-ttu-id="65096-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65096-120">DateTimeOffset</span></span>|<span data-ttu-id="65096-121">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65096-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="65096-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="65096-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="65096-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65096-123">DateTimeOffset</span></span>|<span data-ttu-id="65096-124">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65096-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="65096-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="65096-125">unlockPin</span></span>|<span data-ttu-id="65096-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65096-126">String</span></span>|<span data-ttu-id="65096-127">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="65096-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="65096-128">Relações</span><span class="sxs-lookup"><span data-stu-id="65096-128">Relationships</span></span>
<span data-ttu-id="65096-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65096-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65096-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65096-130">JSON Representation</span></span>
<span data-ttu-id="65096-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65096-131">Here is a JSON representation of the resource.</span></span>
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




