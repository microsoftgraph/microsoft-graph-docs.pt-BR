---
title: Tipo de recurso configurationManagerActionResult
description: Resultado da ação ConfigurationManager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fbe2827194403c8295e9ef59a1089c698f14092
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611976"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="6f69e-103">Tipo de recurso configurationManagerActionResult</span><span class="sxs-lookup"><span data-stu-id="6f69e-103">configurationManagerActionResult resource type</span></span>

<span data-ttu-id="6f69e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f69e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f69e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f69e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f69e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f69e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f69e-107">Resultado da ação ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="6f69e-107">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="6f69e-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f69e-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f69e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f69e-109">Properties</span></span>
|<span data-ttu-id="6f69e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f69e-110">Property</span></span>|<span data-ttu-id="6f69e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f69e-111">Type</span></span>|<span data-ttu-id="6f69e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f69e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f69e-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6f69e-113">actionName</span></span>|<span data-ttu-id="6f69e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f69e-114">String</span></span>|<span data-ttu-id="6f69e-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f69e-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6f69e-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6f69e-116">actionState</span></span>|[<span data-ttu-id="6f69e-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6f69e-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="6f69e-118">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6f69e-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6f69e-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6f69e-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6f69e-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6f69e-120">startDateTime</span></span>|<span data-ttu-id="6f69e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f69e-121">DateTimeOffset</span></span>|<span data-ttu-id="6f69e-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f69e-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6f69e-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f69e-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6f69e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f69e-124">DateTimeOffset</span></span>|<span data-ttu-id="6f69e-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f69e-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6f69e-126">actionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="6f69e-126">actionDeliveryStatus</span></span>|[<span data-ttu-id="6f69e-127">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="6f69e-127">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="6f69e-128">Estado da ação que está sendo entregue ao servidor local.</span><span class="sxs-lookup"><span data-stu-id="6f69e-128">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="6f69e-129">Os valores possíveis são: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="6f69e-129">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="6f69e-130">errorCode</span><span class="sxs-lookup"><span data-stu-id="6f69e-130">errorCode</span></span>|<span data-ttu-id="6f69e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6f69e-131">Int32</span></span>|<span data-ttu-id="6f69e-132">Código de erro da ação do Configuration Manager do cliente</span><span class="sxs-lookup"><span data-stu-id="6f69e-132">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f69e-133">Relações</span><span class="sxs-lookup"><span data-stu-id="6f69e-133">Relationships</span></span>
<span data-ttu-id="6f69e-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f69e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f69e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f69e-135">JSON Representation</span></span>
<span data-ttu-id="6f69e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f69e-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "actionDeliveryStatus": "String",
  "errorCode": 1024
}
```




