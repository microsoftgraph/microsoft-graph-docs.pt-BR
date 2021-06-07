---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eba57eb675fdc73ede027611ba181d9f863c2fc0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751346"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="6f1c4-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="6f1c4-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="6f1c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f1c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f1c4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f1c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f1c4-106">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="6f1c4-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="6f1c4-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f1c4-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f1c4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f1c4-108">Properties</span></span>
|<span data-ttu-id="6f1c4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f1c4-109">Property</span></span>|<span data-ttu-id="6f1c4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f1c4-110">Type</span></span>|<span data-ttu-id="6f1c4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f1c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f1c4-112">actionName</span><span class="sxs-lookup"><span data-stu-id="6f1c4-112">actionName</span></span>|<span data-ttu-id="6f1c4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f1c4-113">String</span></span>|<span data-ttu-id="6f1c4-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f1c4-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6f1c4-115">actionState</span><span class="sxs-lookup"><span data-stu-id="6f1c4-115">actionState</span></span>|[<span data-ttu-id="6f1c4-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6f1c4-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="6f1c4-117">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6f1c4-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6f1c4-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6f1c4-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6f1c4-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6f1c4-119">startDateTime</span></span>|<span data-ttu-id="6f1c4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f1c4-120">DateTimeOffset</span></span>|<span data-ttu-id="6f1c4-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f1c4-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6f1c4-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f1c4-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="6f1c4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f1c4-123">DateTimeOffset</span></span>|<span data-ttu-id="6f1c4-124">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f1c4-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6f1c4-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="6f1c4-125">unlockPin</span></span>|<span data-ttu-id="6f1c4-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f1c4-126">String</span></span>|<span data-ttu-id="6f1c4-127">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="6f1c4-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f1c4-128">Relações</span><span class="sxs-lookup"><span data-stu-id="6f1c4-128">Relationships</span></span>
<span data-ttu-id="6f1c4-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6f1c4-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f1c4-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f1c4-130">JSON Representation</span></span>
<span data-ttu-id="6f1c4-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f1c4-131">Here is a JSON representation of the resource.</span></span>
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




