---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba60fc551a3f9de8b795b6521814d7899a1c3706
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755217"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="4e286-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4e286-103">deviceManagement resource type</span></span>

<span data-ttu-id="4e286-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e286-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e286-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e286-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4e286-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="4e286-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4e286-107">Methods</span></span>
|<span data-ttu-id="4e286-108">Método</span><span class="sxs-lookup"><span data-stu-id="4e286-108">Method</span></span>|<span data-ttu-id="4e286-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4e286-109">Return Type</span></span>|<span data-ttu-id="4e286-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e286-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e286-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4e286-111">Get deviceManagement</span></span>](../api/intune-deviceconfig-devicemanagement-get.md)|[<span data-ttu-id="4e286-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4e286-112">deviceManagement</span></span>](../resources/intune-deviceconfig-devicemanagement.md)|<span data-ttu-id="4e286-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4e286-113">Read properties and relationships of the [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="4e286-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4e286-114">Update deviceManagement</span></span>](../api/intune-deviceconfig-devicemanagement-update.md)|[<span data-ttu-id="4e286-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4e286-115">deviceManagement</span></span>](../resources/intune-deviceconfig-devicemanagement.md)|<span data-ttu-id="4e286-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4e286-116">Update the properties of a [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e286-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e286-117">Properties</span></span>
|<span data-ttu-id="4e286-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e286-118">Property</span></span>|<span data-ttu-id="4e286-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e286-119">Type</span></span>|<span data-ttu-id="4e286-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e286-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e286-121">id</span><span class="sxs-lookup"><span data-stu-id="4e286-121">id</span></span>|<span data-ttu-id="4e286-122">String</span><span class="sxs-lookup"><span data-stu-id="4e286-122">String</span></span>|<span data-ttu-id="4e286-123">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="4e286-123">Unique Identifier</span></span>|
|<span data-ttu-id="4e286-124">settings</span><span class="sxs-lookup"><span data-stu-id="4e286-124">settings</span></span>|[<span data-ttu-id="4e286-125">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="4e286-125">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="4e286-126">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="4e286-126">Account level settings.</span></span>|
|<span data-ttu-id="4e286-127">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="4e286-127">intuneAccountId</span></span>|<span data-ttu-id="4e286-128">Guid</span><span class="sxs-lookup"><span data-stu-id="4e286-128">Guid</span></span>|<span data-ttu-id="4e286-129">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="4e286-129">Intune Account Id for given tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e286-130">Relações</span><span class="sxs-lookup"><span data-stu-id="4e286-130">Relationships</span></span>
|<span data-ttu-id="4e286-131">Relação</span><span class="sxs-lookup"><span data-stu-id="4e286-131">Relationship</span></span>|<span data-ttu-id="4e286-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e286-132">Type</span></span>|<span data-ttu-id="4e286-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e286-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e286-134">deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="4e286-134">deviceConfigurations</span></span>|<span data-ttu-id="4e286-135">Coleção [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e286-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="4e286-136">As configurações de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4e286-136">The device configurations.</span></span>|
|<span data-ttu-id="4e286-137">deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="4e286-137">deviceCompliancePolicies</span></span>|<span data-ttu-id="4e286-138">Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e286-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="4e286-139">As políticas de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e286-139">The device compliance policies.</span></span>|
|<span data-ttu-id="4e286-140">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4e286-140">softwareUpdateStatusSummary</span></span>|[<span data-ttu-id="4e286-141">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4e286-141">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="4e286-142">O resumo do status de atualização do software.</span><span class="sxs-lookup"><span data-stu-id="4e286-142">The software update status summary.</span></span>|
|<span data-ttu-id="4e286-143">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="4e286-143">deviceCompliancePolicyDeviceStateSummary</span></span>|[<span data-ttu-id="4e286-144">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="4e286-144">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="4e286-145">O resumo do estado de conformidade dos dispositivos para esta conta.</span><span class="sxs-lookup"><span data-stu-id="4e286-145">The device compliance state summary for this account.</span></span>|
|<span data-ttu-id="4e286-146">deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="4e286-146">deviceCompliancePolicySettingStateSummaries</span></span>|<span data-ttu-id="4e286-147">Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4e286-147">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="4e286-148">Os estados resumidos das configurações da política de conformidade para esta conta.</span><span class="sxs-lookup"><span data-stu-id="4e286-148">The summary states of compliance policy settings for this account.</span></span>|
|<span data-ttu-id="4e286-149">deviceConfigurationDeviceStateSummaries</span><span class="sxs-lookup"><span data-stu-id="4e286-149">deviceConfigurationDeviceStateSummaries</span></span>|[<span data-ttu-id="4e286-150">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="4e286-150">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="4e286-151">O resumo do estado de configuração de dispositivos para esta conta.</span><span class="sxs-lookup"><span data-stu-id="4e286-151">The device configuration device state summary for this account.</span></span>|
|<span data-ttu-id="4e286-152">iosUpdateStatuses</span><span class="sxs-lookup"><span data-stu-id="4e286-152">iosUpdateStatuses</span></span>|<span data-ttu-id="4e286-153">Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="4e286-153">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) collection</span></span>|<span data-ttu-id="4e286-154">Os status de instalação de atualizações de software do iOS para esta conta.</span><span class="sxs-lookup"><span data-stu-id="4e286-154">The IOS software update installation statuses for this account.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e286-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e286-155">JSON Representation</span></span>
<span data-ttu-id="4e286-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e286-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "Guid"
}
```




