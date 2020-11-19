---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a171eac7d10d20fd67629147babc5df73633c845
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267324"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="ec0db-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="ec0db-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="ec0db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec0db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec0db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec0db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec0db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec0db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec0db-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="ec0db-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="ec0db-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ec0db-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec0db-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec0db-109">Properties</span></span>
|<span data-ttu-id="ec0db-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec0db-110">Property</span></span>|<span data-ttu-id="ec0db-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec0db-111">Type</span></span>|<span data-ttu-id="ec0db-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec0db-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec0db-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ec0db-113">actionName</span></span>|<span data-ttu-id="ec0db-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec0db-114">String</span></span>|<span data-ttu-id="ec0db-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ec0db-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ec0db-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ec0db-116">actionState</span></span>|[<span data-ttu-id="ec0db-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ec0db-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ec0db-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ec0db-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ec0db-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ec0db-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ec0db-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ec0db-120">startDateTime</span></span>|<span data-ttu-id="ec0db-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec0db-121">DateTimeOffset</span></span>|<span data-ttu-id="ec0db-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ec0db-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ec0db-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec0db-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ec0db-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec0db-124">DateTimeOffset</span></span>|<span data-ttu-id="ec0db-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ec0db-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ec0db-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="ec0db-126">unlockPin</span></span>|<span data-ttu-id="ec0db-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec0db-127">String</span></span>|<span data-ttu-id="ec0db-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="ec0db-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec0db-129">Relações</span><span class="sxs-lookup"><span data-stu-id="ec0db-129">Relationships</span></span>
<span data-ttu-id="ec0db-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec0db-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec0db-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec0db-131">JSON Representation</span></span>
<span data-ttu-id="ec0db-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec0db-132">Here is a JSON representation of the resource.</span></span>
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




