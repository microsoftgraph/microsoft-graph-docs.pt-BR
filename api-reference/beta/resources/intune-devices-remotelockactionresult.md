---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 49131d0ba78a37a33879ad29d2f01a78835d8b2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081087"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="faa69-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="faa69-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="faa69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faa69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="faa69-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="faa69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faa69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faa69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa69-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="faa69-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="faa69-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="faa69-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="faa69-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa69-109">Properties</span></span>
|<span data-ttu-id="faa69-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa69-110">Property</span></span>|<span data-ttu-id="faa69-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa69-111">Type</span></span>|<span data-ttu-id="faa69-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa69-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa69-113">actionName</span><span class="sxs-lookup"><span data-stu-id="faa69-113">actionName</span></span>|<span data-ttu-id="faa69-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faa69-114">String</span></span>|<span data-ttu-id="faa69-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="faa69-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="faa69-116">actionState</span><span class="sxs-lookup"><span data-stu-id="faa69-116">actionState</span></span>|[<span data-ttu-id="faa69-117">actionState</span><span class="sxs-lookup"><span data-stu-id="faa69-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="faa69-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="faa69-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="faa69-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="faa69-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="faa69-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="faa69-120">startDateTime</span></span>|<span data-ttu-id="faa69-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faa69-121">DateTimeOffset</span></span>|<span data-ttu-id="faa69-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="faa69-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="faa69-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="faa69-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="faa69-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faa69-124">DateTimeOffset</span></span>|<span data-ttu-id="faa69-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="faa69-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="faa69-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="faa69-126">unlockPin</span></span>|<span data-ttu-id="faa69-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faa69-127">String</span></span>|<span data-ttu-id="faa69-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="faa69-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa69-129">Relações</span><span class="sxs-lookup"><span data-stu-id="faa69-129">Relationships</span></span>
<span data-ttu-id="faa69-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa69-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faa69-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faa69-131">JSON Representation</span></span>
<span data-ttu-id="faa69-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faa69-132">Here is a JSON representation of the resource.</span></span>
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






