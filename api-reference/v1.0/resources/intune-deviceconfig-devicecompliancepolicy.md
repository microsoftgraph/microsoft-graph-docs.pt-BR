---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68fdc729baae64790e19b6956653c45e64137332
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532606"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="7a047-104">Tipo de recurso deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7a047-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="7a047-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a047-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a047-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a047-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a047-107">Esta é a classe base para a política de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="7a047-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="7a047-108">Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui.</span><span class="sxs-lookup"><span data-stu-id="7a047-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="7a047-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="7a047-109">Methods</span></span>
|<span data-ttu-id="7a047-110">Método</span><span class="sxs-lookup"><span data-stu-id="7a047-110">Method</span></span>|<span data-ttu-id="7a047-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7a047-111">Return Type</span></span>|<span data-ttu-id="7a047-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a047-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a047-113">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="7a047-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="7a047-114">Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="7a047-115">Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7a047-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="7a047-116">Obter deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7a047-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="7a047-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7a047-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="7a047-118">Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7a047-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="7a047-119">ação assign</span><span class="sxs-lookup"><span data-stu-id="7a047-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="7a047-120">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7a047-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a047-121">Not yet documented</span></span>|
|[<span data-ttu-id="7a047-122">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="7a047-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="7a047-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7a047-123">None</span></span>|<span data-ttu-id="7a047-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a047-124">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7a047-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a047-125">Properties</span></span>
|<span data-ttu-id="7a047-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a047-126">Property</span></span>|<span data-ttu-id="7a047-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a047-127">Type</span></span>|<span data-ttu-id="7a047-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a047-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a047-129">id</span><span class="sxs-lookup"><span data-stu-id="7a047-129">id</span></span>|<span data-ttu-id="7a047-130">String</span><span class="sxs-lookup"><span data-stu-id="7a047-130">String</span></span>|<span data-ttu-id="7a047-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7a047-131">Key of the entity.</span></span>|
|<span data-ttu-id="7a047-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a047-132">createdDateTime</span></span>|<span data-ttu-id="7a047-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a047-133">DateTimeOffset</span></span>|<span data-ttu-id="7a047-134">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7a047-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="7a047-135">description</span><span class="sxs-lookup"><span data-stu-id="7a047-135">description</span></span>|<span data-ttu-id="7a047-136">String</span><span class="sxs-lookup"><span data-stu-id="7a047-136">String</span></span>|<span data-ttu-id="7a047-137">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7a047-137">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7a047-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a047-138">lastModifiedDateTime</span></span>|<span data-ttu-id="7a047-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a047-139">DateTimeOffset</span></span>|<span data-ttu-id="7a047-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7a047-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7a047-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7a047-141">displayName</span></span>|<span data-ttu-id="7a047-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a047-142">String</span></span>|<span data-ttu-id="7a047-143">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7a047-143">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7a047-144">versão</span><span class="sxs-lookup"><span data-stu-id="7a047-144">version</span></span>|<span data-ttu-id="7a047-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7a047-145">Int32</span></span>|<span data-ttu-id="7a047-146">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7a047-146">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a047-147">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="7a047-147">Relationships</span></span>
|<span data-ttu-id="7a047-148">Relação</span><span class="sxs-lookup"><span data-stu-id="7a047-148">Relationship</span></span>|<span data-ttu-id="7a047-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a047-149">Type</span></span>|<span data-ttu-id="7a047-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a047-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a047-151">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="7a047-151">scheduledActionsForRule</span></span>|<span data-ttu-id="7a047-152">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="7a047-153">A lista de ações agendadas para essa regra</span><span class="sxs-lookup"><span data-stu-id="7a047-153">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="7a047-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7a047-154">deviceStatuses</span></span>|<span data-ttu-id="7a047-155">Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="7a047-156">Lista de DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="7a047-156">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="7a047-157">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7a047-157">userStatuses</span></span>|<span data-ttu-id="7a047-158">Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="7a047-159">Lista de DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="7a047-159">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="7a047-160">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7a047-160">deviceStatusOverview</span></span>|[<span data-ttu-id="7a047-161">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7a047-161">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="7a047-162">Visão geral de status de dispositivos para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7a047-162">Device compliance devices status overview</span></span>|
|<span data-ttu-id="7a047-163">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7a047-163">userStatusOverview</span></span>|[<span data-ttu-id="7a047-164">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="7a047-164">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="7a047-165">Visão geral de status de usuários para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7a047-165">Device compliance users status overview</span></span>|
|<span data-ttu-id="7a047-166">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7a047-166">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7a047-167">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7a047-168">Resumo do dispositivo para estado de configuração de conformidade</span><span class="sxs-lookup"><span data-stu-id="7a047-168">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="7a047-169">assignments</span><span class="sxs-lookup"><span data-stu-id="7a047-169">assignments</span></span>|<span data-ttu-id="7a047-170">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7a047-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7a047-171">A coleção de atribuições para essa política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="7a047-171">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a047-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a047-172">JSON Representation</span></span>
<span data-ttu-id="7a047-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a047-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




