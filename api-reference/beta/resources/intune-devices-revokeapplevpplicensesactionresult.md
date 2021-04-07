---
title: Tipo de recurso revokeAppleVppLicensesActionResult
description: Resultado da ação Revogar licenças do Apple Vpp
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56fce51fb5de4066136199a99670c4767b6ad724
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611857"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="f0989-103">Tipo de recurso revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="f0989-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="f0989-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0989-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0989-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0989-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0989-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0989-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0989-107">Resultado da ação Revogar licenças do Apple Vpp</span><span class="sxs-lookup"><span data-stu-id="f0989-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="f0989-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f0989-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0989-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0989-109">Properties</span></span>
|<span data-ttu-id="f0989-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0989-110">Property</span></span>|<span data-ttu-id="f0989-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0989-111">Type</span></span>|<span data-ttu-id="f0989-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0989-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0989-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f0989-113">actionName</span></span>|<span data-ttu-id="f0989-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0989-114">String</span></span>|<span data-ttu-id="f0989-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f0989-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f0989-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f0989-116">actionState</span></span>|[<span data-ttu-id="f0989-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f0989-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="f0989-118">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f0989-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f0989-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f0989-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f0989-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f0989-120">startDateTime</span></span>|<span data-ttu-id="f0989-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0989-121">DateTimeOffset</span></span>|<span data-ttu-id="f0989-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f0989-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f0989-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0989-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f0989-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0989-124">DateTimeOffset</span></span>|<span data-ttu-id="f0989-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f0989-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f0989-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="f0989-126">totalLicensesCount</span></span>|<span data-ttu-id="f0989-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f0989-127">Int32</span></span>|<span data-ttu-id="f0989-128">Número total de licenças do Apple Vpp associadas</span><span class="sxs-lookup"><span data-stu-id="f0989-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="f0989-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="f0989-129">failedLicensesCount</span></span>|<span data-ttu-id="f0989-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f0989-130">Int32</span></span>|<span data-ttu-id="f0989-131">Número total de licenças do Apple Vpp que falharam ao revogar</span><span class="sxs-lookup"><span data-stu-id="f0989-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0989-132">Relações</span><span class="sxs-lookup"><span data-stu-id="f0989-132">Relationships</span></span>
<span data-ttu-id="f0989-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0989-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0989-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0989-134">JSON Representation</span></span>
<span data-ttu-id="f0989-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0989-135">Here is a JSON representation of the resource.</span></span>
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




