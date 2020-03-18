---
title: tipo de recurso configurationManagerActionResult
description: Resultado da ação ConfigurationManager
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de187585e7e8dd74f4495d7143030e30acf46c4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785081"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="d90c7-103">tipo de recurso configurationManagerActionResult</span><span class="sxs-lookup"><span data-stu-id="d90c7-103">configurationManagerActionResult resource type</span></span>

> <span data-ttu-id="d90c7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d90c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d90c7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d90c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90c7-106">Resultado da ação ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="d90c7-106">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="d90c7-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d90c7-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d90c7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d90c7-108">Properties</span></span>
|<span data-ttu-id="d90c7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d90c7-109">Property</span></span>|<span data-ttu-id="d90c7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d90c7-110">Type</span></span>|<span data-ttu-id="d90c7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d90c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90c7-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d90c7-112">actionName</span></span>|<span data-ttu-id="d90c7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d90c7-113">String</span></span>|<span data-ttu-id="d90c7-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d90c7-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d90c7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d90c7-115">actionState</span></span>|[<span data-ttu-id="d90c7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d90c7-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d90c7-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d90c7-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d90c7-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d90c7-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d90c7-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d90c7-119">startDateTime</span></span>|<span data-ttu-id="d90c7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90c7-120">DateTimeOffset</span></span>|<span data-ttu-id="d90c7-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d90c7-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d90c7-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d90c7-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d90c7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90c7-123">DateTimeOffset</span></span>|<span data-ttu-id="d90c7-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d90c7-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d90c7-125">actionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="d90c7-125">actionDeliveryStatus</span></span>|[<span data-ttu-id="d90c7-126">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="d90c7-126">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="d90c7-127">Estado da ação que está sendo entregue ao servidor local.</span><span class="sxs-lookup"><span data-stu-id="d90c7-127">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="d90c7-128">Os valores possíveis são: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="d90c7-128">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="d90c7-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="d90c7-129">errorCode</span></span>|<span data-ttu-id="d90c7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d90c7-130">Int32</span></span>|<span data-ttu-id="d90c7-131">Código de erro da ação do Gerenciador de configurações do cliente</span><span class="sxs-lookup"><span data-stu-id="d90c7-131">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="d90c7-132">Relações</span><span class="sxs-lookup"><span data-stu-id="d90c7-132">Relationships</span></span>
<span data-ttu-id="d90c7-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d90c7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d90c7-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d90c7-134">JSON Representation</span></span>
<span data-ttu-id="d90c7-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d90c7-135">Here is a JSON representation of the resource.</span></span>
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



