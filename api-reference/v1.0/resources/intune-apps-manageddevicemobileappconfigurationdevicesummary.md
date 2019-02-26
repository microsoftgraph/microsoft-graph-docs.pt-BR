---
title: Tipo de recurso managedDeviceMobileAppConfigurationDeviceSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do dispositivo de configuração de aplicativo móvel de MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e62d02b5b702b56d72a0c75f9e5da1f6ad9dbdc3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259637"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="061ed-103">Tipo de recurso managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="061ed-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="061ed-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="061ed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="061ed-105">Contém propriedades, propriedades herdadas e ações para um resumo de status do dispositivo de configuração de aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="061ed-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="061ed-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="061ed-106">Methods</span></span>
|<span data-ttu-id="061ed-107">Método</span><span class="sxs-lookup"><span data-stu-id="061ed-107">Method</span></span>|<span data-ttu-id="061ed-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="061ed-108">Return Type</span></span>|<span data-ttu-id="061ed-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="061ed-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="061ed-110">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="061ed-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="061ed-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="061ed-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="061ed-112">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="061ed-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="061ed-113">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="061ed-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="061ed-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="061ed-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="061ed-115">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="061ed-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="061ed-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="061ed-116">Properties</span></span>
|<span data-ttu-id="061ed-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="061ed-117">Property</span></span>|<span data-ttu-id="061ed-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="061ed-118">Type</span></span>|<span data-ttu-id="061ed-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="061ed-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="061ed-120">id</span><span class="sxs-lookup"><span data-stu-id="061ed-120">id</span></span>|<span data-ttu-id="061ed-121">String</span><span class="sxs-lookup"><span data-stu-id="061ed-121">String</span></span>|<span data-ttu-id="061ed-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="061ed-122">Key of the entity.</span></span>|
|<span data-ttu-id="061ed-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="061ed-123">pendingCount</span></span>|<span data-ttu-id="061ed-124">Int32</span><span class="sxs-lookup"><span data-stu-id="061ed-124">Int32</span></span>|<span data-ttu-id="061ed-125">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="061ed-125">Number of pending devices</span></span>|
|<span data-ttu-id="061ed-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="061ed-126">notApplicableCount</span></span>|<span data-ttu-id="061ed-127">Int32</span><span class="sxs-lookup"><span data-stu-id="061ed-127">Int32</span></span>|<span data-ttu-id="061ed-128">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="061ed-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="061ed-129">successCount</span><span class="sxs-lookup"><span data-stu-id="061ed-129">successCount</span></span>|<span data-ttu-id="061ed-130">Int32</span><span class="sxs-lookup"><span data-stu-id="061ed-130">Int32</span></span>|<span data-ttu-id="061ed-131">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="061ed-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="061ed-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="061ed-132">errorCount</span></span>|<span data-ttu-id="061ed-133">Int32</span><span class="sxs-lookup"><span data-stu-id="061ed-133">Int32</span></span>|<span data-ttu-id="061ed-134">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="061ed-134">Number of error devices</span></span>|
|<span data-ttu-id="061ed-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="061ed-135">failedCount</span></span>|<span data-ttu-id="061ed-136">Int32</span><span class="sxs-lookup"><span data-stu-id="061ed-136">Int32</span></span>|<span data-ttu-id="061ed-137">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="061ed-137">Number of failed devices</span></span>|
|<span data-ttu-id="061ed-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="061ed-138">lastUpdateDateTime</span></span>|<span data-ttu-id="061ed-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061ed-139">DateTimeOffset</span></span>|<span data-ttu-id="061ed-140">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="061ed-140">Last update time</span></span>|
|<span data-ttu-id="061ed-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="061ed-141">configurationVersion</span></span>|<span data-ttu-id="061ed-142">Int32</span><span class="sxs-lookup"><span data-stu-id="061ed-142">Int32</span></span>|<span data-ttu-id="061ed-143">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="061ed-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="061ed-144">Relações</span><span class="sxs-lookup"><span data-stu-id="061ed-144">Relationships</span></span>
<span data-ttu-id="061ed-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="061ed-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="061ed-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="061ed-146">JSON Representation</span></span>
<span data-ttu-id="061ed-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="061ed-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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



