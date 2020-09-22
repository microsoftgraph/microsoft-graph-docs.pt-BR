---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6eae05e799394d37fa5c842b278f60251fbd47a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091037"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="92582-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="92582-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="92582-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92582-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92582-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92582-106">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="92582-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="92582-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="92582-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92582-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92582-108">Properties</span></span>
|<span data-ttu-id="92582-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92582-109">Property</span></span>|<span data-ttu-id="92582-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="92582-110">Type</span></span>|<span data-ttu-id="92582-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="92582-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92582-112">actionName</span><span class="sxs-lookup"><span data-stu-id="92582-112">actionName</span></span>|<span data-ttu-id="92582-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92582-113">String</span></span>|<span data-ttu-id="92582-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="92582-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="92582-115">actionState</span><span class="sxs-lookup"><span data-stu-id="92582-115">actionState</span></span>|[<span data-ttu-id="92582-116">actionState</span><span class="sxs-lookup"><span data-stu-id="92582-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="92582-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="92582-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="92582-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="92582-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="92582-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="92582-119">startDateTime</span></span>|<span data-ttu-id="92582-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92582-120">DateTimeOffset</span></span>|<span data-ttu-id="92582-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="92582-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="92582-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="92582-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="92582-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92582-123">DateTimeOffset</span></span>|<span data-ttu-id="92582-124">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="92582-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="92582-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="92582-125">unlockPin</span></span>|<span data-ttu-id="92582-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92582-126">String</span></span>|<span data-ttu-id="92582-127">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="92582-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="92582-128">Relações</span><span class="sxs-lookup"><span data-stu-id="92582-128">Relationships</span></span>
<span data-ttu-id="92582-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92582-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92582-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92582-130">JSON Representation</span></span>
<span data-ttu-id="92582-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92582-131">Here is a JSON representation of the resource.</span></span>
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









