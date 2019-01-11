---
title: Tipo de recurso managedDeviceMobileAppConfigurationDeviceSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do dispositivo de configuração de aplicativo móvel de MDM.
localization_priority: Normal
ms.openlocfilehash: 47a323a074bd42d1e075a2a5ddd6aeb9181c98eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816342"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="f25ee-103">Tipo de recurso managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f25ee-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="f25ee-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f25ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f25ee-105">Contém propriedades, propriedades herdadas e ações para um resumo de status do dispositivo de configuração de aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="f25ee-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="f25ee-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f25ee-106">Methods</span></span>
|<span data-ttu-id="f25ee-107">Método</span><span class="sxs-lookup"><span data-stu-id="f25ee-107">Method</span></span>|<span data-ttu-id="f25ee-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f25ee-108">Return Type</span></span>|<span data-ttu-id="f25ee-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f25ee-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f25ee-110">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f25ee-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="f25ee-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f25ee-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f25ee-112">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f25ee-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="f25ee-113">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f25ee-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="f25ee-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f25ee-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f25ee-115">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f25ee-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f25ee-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f25ee-116">Properties</span></span>
|<span data-ttu-id="f25ee-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f25ee-117">Property</span></span>|<span data-ttu-id="f25ee-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f25ee-118">Type</span></span>|<span data-ttu-id="f25ee-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f25ee-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f25ee-120">id</span><span class="sxs-lookup"><span data-stu-id="f25ee-120">id</span></span>|<span data-ttu-id="f25ee-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f25ee-121">String</span></span>|<span data-ttu-id="f25ee-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f25ee-122">Key of the entity.</span></span>|
|<span data-ttu-id="f25ee-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f25ee-123">pendingCount</span></span>|<span data-ttu-id="f25ee-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f25ee-124">Int32</span></span>|<span data-ttu-id="f25ee-125">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="f25ee-125">Number of pending devices</span></span>|
|<span data-ttu-id="f25ee-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f25ee-126">notApplicableCount</span></span>|<span data-ttu-id="f25ee-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f25ee-127">Int32</span></span>|<span data-ttu-id="f25ee-128">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f25ee-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="f25ee-129">successCount</span><span class="sxs-lookup"><span data-stu-id="f25ee-129">successCount</span></span>|<span data-ttu-id="f25ee-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f25ee-130">Int32</span></span>|<span data-ttu-id="f25ee-131">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="f25ee-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="f25ee-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="f25ee-132">errorCount</span></span>|<span data-ttu-id="f25ee-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f25ee-133">Int32</span></span>|<span data-ttu-id="f25ee-134">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="f25ee-134">Number of error devices</span></span>|
|<span data-ttu-id="f25ee-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="f25ee-135">failedCount</span></span>|<span data-ttu-id="f25ee-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f25ee-136">Int32</span></span>|<span data-ttu-id="f25ee-137">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="f25ee-137">Number of failed devices</span></span>|
|<span data-ttu-id="f25ee-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f25ee-138">lastUpdateDateTime</span></span>|<span data-ttu-id="f25ee-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f25ee-139">DateTimeOffset</span></span>|<span data-ttu-id="f25ee-140">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="f25ee-140">Last update time</span></span>|
|<span data-ttu-id="f25ee-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f25ee-141">configurationVersion</span></span>|<span data-ttu-id="f25ee-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f25ee-142">Int32</span></span>|<span data-ttu-id="f25ee-143">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="f25ee-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f25ee-144">Relações</span><span class="sxs-lookup"><span data-stu-id="f25ee-144">Relationships</span></span>
<span data-ttu-id="f25ee-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f25ee-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f25ee-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f25ee-146">JSON Representation</span></span>
<span data-ttu-id="f25ee-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f25ee-147">Here is a JSON representation of the resource.</span></span>
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



