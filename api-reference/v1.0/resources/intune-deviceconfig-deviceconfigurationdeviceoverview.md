---
title: Tipo de recurso deviceConfigurationDeviceOverview
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 1936b8256c5755c44e613c1626664cef3f7a0ccc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324427"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="48547-103">Tipo de recurso deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="48547-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="48547-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48547-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48547-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48547-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="48547-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="48547-106">Methods</span></span>
|<span data-ttu-id="48547-107">Método</span><span class="sxs-lookup"><span data-stu-id="48547-107">Method</span></span>|<span data-ttu-id="48547-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48547-108">Return Type</span></span>|<span data-ttu-id="48547-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="48547-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48547-110">Obter deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="48547-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="48547-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="48547-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="48547-112">Ler propriedades e relações de objetos de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="48547-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="48547-113">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="48547-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="48547-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="48547-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="48547-115">Atualizar as propriedades de um objeto de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="48547-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="48547-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48547-116">Properties</span></span>
|<span data-ttu-id="48547-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48547-117">Property</span></span>|<span data-ttu-id="48547-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="48547-118">Type</span></span>|<span data-ttu-id="48547-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="48547-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48547-120">id</span><span class="sxs-lookup"><span data-stu-id="48547-120">id</span></span>|<span data-ttu-id="48547-121">String</span><span class="sxs-lookup"><span data-stu-id="48547-121">String</span></span>|<span data-ttu-id="48547-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48547-122">Key of the entity.</span></span>|
|<span data-ttu-id="48547-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="48547-123">pendingCount</span></span>|<span data-ttu-id="48547-124">Int32</span><span class="sxs-lookup"><span data-stu-id="48547-124">Int32</span></span>|<span data-ttu-id="48547-125">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="48547-125">Number of pending devices</span></span>|
|<span data-ttu-id="48547-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="48547-126">notApplicableCount</span></span>|<span data-ttu-id="48547-127">Int32</span><span class="sxs-lookup"><span data-stu-id="48547-127">Int32</span></span>|<span data-ttu-id="48547-128">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="48547-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="48547-129">successCount</span><span class="sxs-lookup"><span data-stu-id="48547-129">successCount</span></span>|<span data-ttu-id="48547-130">Int32</span><span class="sxs-lookup"><span data-stu-id="48547-130">Int32</span></span>|<span data-ttu-id="48547-131">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="48547-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="48547-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="48547-132">errorCount</span></span>|<span data-ttu-id="48547-133">Int32</span><span class="sxs-lookup"><span data-stu-id="48547-133">Int32</span></span>|<span data-ttu-id="48547-134">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="48547-134">Number of error devices</span></span>|
|<span data-ttu-id="48547-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="48547-135">failedCount</span></span>|<span data-ttu-id="48547-136">Int32</span><span class="sxs-lookup"><span data-stu-id="48547-136">Int32</span></span>|<span data-ttu-id="48547-137">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="48547-137">Number of failed devices</span></span>|
|<span data-ttu-id="48547-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="48547-138">lastUpdateDateTime</span></span>|<span data-ttu-id="48547-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48547-139">DateTimeOffset</span></span>|<span data-ttu-id="48547-140">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="48547-140">Last update time</span></span>|
|<span data-ttu-id="48547-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="48547-141">configurationVersion</span></span>|<span data-ttu-id="48547-142">Int32</span><span class="sxs-lookup"><span data-stu-id="48547-142">Int32</span></span>|<span data-ttu-id="48547-143">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="48547-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="48547-144">Relações</span><span class="sxs-lookup"><span data-stu-id="48547-144">Relationships</span></span>
<span data-ttu-id="48547-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48547-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48547-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48547-146">JSON Representation</span></span>
<span data-ttu-id="48547-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48547-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



