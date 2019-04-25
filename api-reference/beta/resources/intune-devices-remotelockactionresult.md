---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b16a99c793d60de04201fc057a58da122c83fd6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526157"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="bc19d-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="bc19d-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="bc19d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc19d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc19d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc19d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc19d-106">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="bc19d-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="bc19d-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc19d-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc19d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc19d-108">Properties</span></span>
|<span data-ttu-id="bc19d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc19d-109">Property</span></span>|<span data-ttu-id="bc19d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc19d-110">Type</span></span>|<span data-ttu-id="bc19d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc19d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc19d-112">actionName</span><span class="sxs-lookup"><span data-stu-id="bc19d-112">actionName</span></span>|<span data-ttu-id="bc19d-113">String</span><span class="sxs-lookup"><span data-stu-id="bc19d-113">String</span></span>|<span data-ttu-id="bc19d-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc19d-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bc19d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bc19d-115">actionState</span></span>|[<span data-ttu-id="bc19d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bc19d-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bc19d-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bc19d-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bc19d-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bc19d-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bc19d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bc19d-119">startDateTime</span></span>|<span data-ttu-id="bc19d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc19d-120">DateTimeOffset</span></span>|<span data-ttu-id="bc19d-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc19d-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bc19d-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc19d-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="bc19d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc19d-123">DateTimeOffset</span></span>|<span data-ttu-id="bc19d-124">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc19d-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bc19d-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="bc19d-125">unlockPin</span></span>|<span data-ttu-id="bc19d-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc19d-126">String</span></span>|<span data-ttu-id="bc19d-127">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="bc19d-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc19d-128">Relações</span><span class="sxs-lookup"><span data-stu-id="bc19d-128">Relationships</span></span>
<span data-ttu-id="bc19d-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc19d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc19d-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc19d-130">JSON Representation</span></span>
<span data-ttu-id="bc19d-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc19d-131">Here is a JSON representation of the resource.</span></span>
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





