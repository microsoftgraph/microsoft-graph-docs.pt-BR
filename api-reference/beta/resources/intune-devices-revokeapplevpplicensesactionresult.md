---
title: tipo de recurso revokeAppleVppLicensesActionResult
description: Cancelar o resultado da ação de licenças VPP da Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe831c36af1cfbe29d4b5bcc0dd2daa2a148a01a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963825"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="12ed5-103">tipo de recurso revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="12ed5-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="12ed5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12ed5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12ed5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12ed5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12ed5-106">Cancelar o resultado da ação de licenças VPP da Apple</span><span class="sxs-lookup"><span data-stu-id="12ed5-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="12ed5-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="12ed5-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="12ed5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12ed5-108">Properties</span></span>
|<span data-ttu-id="12ed5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12ed5-109">Property</span></span>|<span data-ttu-id="12ed5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="12ed5-110">Type</span></span>|<span data-ttu-id="12ed5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ed5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ed5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="12ed5-112">actionName</span></span>|<span data-ttu-id="12ed5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12ed5-113">String</span></span>|<span data-ttu-id="12ed5-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="12ed5-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="12ed5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="12ed5-115">actionState</span></span>|[<span data-ttu-id="12ed5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="12ed5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="12ed5-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="12ed5-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="12ed5-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="12ed5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="12ed5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="12ed5-119">startDateTime</span></span>|<span data-ttu-id="12ed5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12ed5-120">DateTimeOffset</span></span>|<span data-ttu-id="12ed5-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="12ed5-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="12ed5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="12ed5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="12ed5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12ed5-123">DateTimeOffset</span></span>|<span data-ttu-id="12ed5-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="12ed5-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="12ed5-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="12ed5-125">totalLicensesCount</span></span>|<span data-ttu-id="12ed5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="12ed5-126">Int32</span></span>|<span data-ttu-id="12ed5-127">Número total de licenças VPP da Apple associadas</span><span class="sxs-lookup"><span data-stu-id="12ed5-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="12ed5-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="12ed5-128">failedLicensesCount</span></span>|<span data-ttu-id="12ed5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="12ed5-129">Int32</span></span>|<span data-ttu-id="12ed5-130">Número total de licenças VPP da Apple que falharam ao revogar</span><span class="sxs-lookup"><span data-stu-id="12ed5-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="12ed5-131">Relações</span><span class="sxs-lookup"><span data-stu-id="12ed5-131">Relationships</span></span>
<span data-ttu-id="12ed5-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12ed5-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12ed5-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12ed5-133">JSON Representation</span></span>
<span data-ttu-id="12ed5-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12ed5-134">Here is a JSON representation of the resource.</span></span>
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





