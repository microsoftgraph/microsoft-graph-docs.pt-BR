---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3892bab420a72acfe1a02c7fe4886c936eec0281
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691334"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="b9b8f-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="b9b8f-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="b9b8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9b8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9b8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9b8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9b8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9b8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9b8f-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="b9b8f-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="b9b8f-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b9b8f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9b8f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9b8f-109">Properties</span></span>
|<span data-ttu-id="b9b8f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9b8f-110">Property</span></span>|<span data-ttu-id="b9b8f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9b8f-111">Type</span></span>|<span data-ttu-id="b9b8f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9b8f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9b8f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b9b8f-113">actionName</span></span>|<span data-ttu-id="b9b8f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9b8f-114">String</span></span>|<span data-ttu-id="b9b8f-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b9b8f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b9b8f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b9b8f-116">actionState</span></span>|[<span data-ttu-id="b9b8f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b9b8f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b9b8f-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b9b8f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b9b8f-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b9b8f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b9b8f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b9b8f-120">startDateTime</span></span>|<span data-ttu-id="b9b8f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9b8f-121">DateTimeOffset</span></span>|<span data-ttu-id="b9b8f-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b9b8f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b9b8f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9b8f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b9b8f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9b8f-124">DateTimeOffset</span></span>|<span data-ttu-id="b9b8f-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b9b8f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b9b8f-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="b9b8f-126">unlockPin</span></span>|<span data-ttu-id="b9b8f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9b8f-127">String</span></span>|<span data-ttu-id="b9b8f-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="b9b8f-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9b8f-129">Relações</span><span class="sxs-lookup"><span data-stu-id="b9b8f-129">Relationships</span></span>
<span data-ttu-id="b9b8f-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9b8f-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9b8f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9b8f-131">JSON Representation</span></span>
<span data-ttu-id="b9b8f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9b8f-132">Here is a JSON representation of the resource.</span></span>
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





