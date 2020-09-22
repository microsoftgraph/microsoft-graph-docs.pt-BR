---
title: tipo de recurso configurationManagerActionResult
description: Resultado da ação ConfigurationManager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8512f383396b235d80fa16b7bc122e42b89c041a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060675"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="23d5b-103">tipo de recurso configurationManagerActionResult</span><span class="sxs-lookup"><span data-stu-id="23d5b-103">configurationManagerActionResult resource type</span></span>

<span data-ttu-id="23d5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23d5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23d5b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23d5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23d5b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23d5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23d5b-107">Resultado da ação ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="23d5b-107">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="23d5b-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23d5b-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23d5b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23d5b-109">Properties</span></span>
|<span data-ttu-id="23d5b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23d5b-110">Property</span></span>|<span data-ttu-id="23d5b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="23d5b-111">Type</span></span>|<span data-ttu-id="23d5b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="23d5b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23d5b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="23d5b-113">actionName</span></span>|<span data-ttu-id="23d5b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23d5b-114">String</span></span>|<span data-ttu-id="23d5b-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23d5b-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23d5b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="23d5b-116">actionState</span></span>|[<span data-ttu-id="23d5b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="23d5b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="23d5b-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="23d5b-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="23d5b-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="23d5b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="23d5b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="23d5b-120">startDateTime</span></span>|<span data-ttu-id="23d5b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d5b-121">DateTimeOffset</span></span>|<span data-ttu-id="23d5b-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23d5b-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23d5b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="23d5b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="23d5b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d5b-124">DateTimeOffset</span></span>|<span data-ttu-id="23d5b-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23d5b-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23d5b-126">actionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="23d5b-126">actionDeliveryStatus</span></span>|[<span data-ttu-id="23d5b-127">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="23d5b-127">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="23d5b-128">Estado da ação que está sendo entregue ao servidor local.</span><span class="sxs-lookup"><span data-stu-id="23d5b-128">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="23d5b-129">Os valores possíveis são: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="23d5b-129">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="23d5b-130">errorCode</span><span class="sxs-lookup"><span data-stu-id="23d5b-130">errorCode</span></span>|<span data-ttu-id="23d5b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="23d5b-131">Int32</span></span>|<span data-ttu-id="23d5b-132">Código de erro da ação do Gerenciador de configurações do cliente</span><span class="sxs-lookup"><span data-stu-id="23d5b-132">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="23d5b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="23d5b-133">Relationships</span></span>
<span data-ttu-id="23d5b-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23d5b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23d5b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23d5b-135">JSON Representation</span></span>
<span data-ttu-id="23d5b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23d5b-136">Here is a JSON representation of the resource.</span></span>
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






