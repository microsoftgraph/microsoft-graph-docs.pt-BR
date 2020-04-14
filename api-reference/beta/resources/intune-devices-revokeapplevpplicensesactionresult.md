---
title: tipo de recurso revokeAppleVppLicensesActionResult
description: Cancelar o resultado da ação de licenças VPP da Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68a01df03814ea2fd0b52ecfc681490777b46d54
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383148"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="ba118-103">tipo de recurso revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="ba118-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="ba118-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba118-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba118-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba118-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba118-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba118-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba118-107">Cancelar o resultado da ação de licenças VPP da Apple</span><span class="sxs-lookup"><span data-stu-id="ba118-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="ba118-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ba118-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba118-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba118-109">Properties</span></span>
|<span data-ttu-id="ba118-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba118-110">Property</span></span>|<span data-ttu-id="ba118-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba118-111">Type</span></span>|<span data-ttu-id="ba118-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba118-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba118-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ba118-113">actionName</span></span>|<span data-ttu-id="ba118-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba118-114">String</span></span>|<span data-ttu-id="ba118-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ba118-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ba118-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ba118-116">actionState</span></span>|[<span data-ttu-id="ba118-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ba118-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ba118-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ba118-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ba118-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ba118-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ba118-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba118-120">startDateTime</span></span>|<span data-ttu-id="ba118-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba118-121">DateTimeOffset</span></span>|<span data-ttu-id="ba118-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ba118-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ba118-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba118-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ba118-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba118-124">DateTimeOffset</span></span>|<span data-ttu-id="ba118-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ba118-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ba118-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ba118-126">totalLicensesCount</span></span>|<span data-ttu-id="ba118-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ba118-127">Int32</span></span>|<span data-ttu-id="ba118-128">Número total de licenças VPP da Apple associadas</span><span class="sxs-lookup"><span data-stu-id="ba118-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="ba118-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ba118-129">failedLicensesCount</span></span>|<span data-ttu-id="ba118-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ba118-130">Int32</span></span>|<span data-ttu-id="ba118-131">Número total de licenças VPP da Apple que falharam ao revogar</span><span class="sxs-lookup"><span data-stu-id="ba118-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba118-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ba118-132">Relationships</span></span>
<span data-ttu-id="ba118-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba118-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba118-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba118-134">JSON Representation</span></span>
<span data-ttu-id="ba118-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba118-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```



