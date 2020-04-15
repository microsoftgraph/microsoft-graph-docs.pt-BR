---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb96d3ff8dee50413b36cf70e8cfaf4b6f418cb0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448888"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="9ee6c-104">Tipo de recurso deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9ee6c-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="9ee6c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ee6c-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ee6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ee6c-107">Esta é a classe base para a política de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="9ee6c-108">Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="9ee6c-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ee6c-109">Methods</span></span>
|<span data-ttu-id="9ee6c-110">Método</span><span class="sxs-lookup"><span data-stu-id="9ee6c-110">Method</span></span>|<span data-ttu-id="9ee6c-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ee6c-111">Return Type</span></span>|<span data-ttu-id="9ee6c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ee6c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ee6c-113">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="9ee6c-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="9ee6c-114">Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="9ee6c-115">Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ee6c-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="9ee6c-116">Obter deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9ee6c-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="9ee6c-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9ee6c-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="9ee6c-118">Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ee6c-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="9ee6c-119">ação assign</span><span class="sxs-lookup"><span data-stu-id="9ee6c-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="9ee6c-120">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="9ee6c-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9ee6c-121">Not yet documented</span></span>|
|[<span data-ttu-id="9ee6c-122">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="9ee6c-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="9ee6c-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9ee6c-123">None</span></span>|<span data-ttu-id="9ee6c-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9ee6c-124">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9ee6c-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ee6c-125">Properties</span></span>
|<span data-ttu-id="9ee6c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ee6c-126">Property</span></span>|<span data-ttu-id="9ee6c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ee6c-127">Type</span></span>|<span data-ttu-id="9ee6c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ee6c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee6c-129">id</span><span class="sxs-lookup"><span data-stu-id="9ee6c-129">id</span></span>|<span data-ttu-id="9ee6c-130">String</span><span class="sxs-lookup"><span data-stu-id="9ee6c-130">String</span></span>|<span data-ttu-id="9ee6c-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-131">Key of the entity.</span></span>|
|<span data-ttu-id="9ee6c-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee6c-132">createdDateTime</span></span>|<span data-ttu-id="9ee6c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee6c-133">DateTimeOffset</span></span>|<span data-ttu-id="9ee6c-134">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="9ee6c-135">description</span><span class="sxs-lookup"><span data-stu-id="9ee6c-135">description</span></span>|<span data-ttu-id="9ee6c-136">String</span><span class="sxs-lookup"><span data-stu-id="9ee6c-136">String</span></span>|<span data-ttu-id="9ee6c-137">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-137">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="9ee6c-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee6c-138">lastModifiedDateTime</span></span>|<span data-ttu-id="9ee6c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee6c-139">DateTimeOffset</span></span>|<span data-ttu-id="9ee6c-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9ee6c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="9ee6c-141">displayName</span></span>|<span data-ttu-id="9ee6c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ee6c-142">String</span></span>|<span data-ttu-id="9ee6c-143">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-143">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="9ee6c-144">versão</span><span class="sxs-lookup"><span data-stu-id="9ee6c-144">version</span></span>|<span data-ttu-id="9ee6c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9ee6c-145">Int32</span></span>|<span data-ttu-id="9ee6c-146">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-146">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ee6c-147">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="9ee6c-147">Relationships</span></span>
|<span data-ttu-id="9ee6c-148">Relação</span><span class="sxs-lookup"><span data-stu-id="9ee6c-148">Relationship</span></span>|<span data-ttu-id="9ee6c-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ee6c-149">Type</span></span>|<span data-ttu-id="9ee6c-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ee6c-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee6c-151">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="9ee6c-151">scheduledActionsForRule</span></span>|<span data-ttu-id="9ee6c-152">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="9ee6c-153">A lista de ações agendadas para essa regra</span><span class="sxs-lookup"><span data-stu-id="9ee6c-153">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="9ee6c-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="9ee6c-154">deviceStatuses</span></span>|<span data-ttu-id="9ee6c-155">Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="9ee6c-156">Lista de DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-156">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="9ee6c-157">userStatuses</span><span class="sxs-lookup"><span data-stu-id="9ee6c-157">userStatuses</span></span>|<span data-ttu-id="9ee6c-158">Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="9ee6c-159">Lista de DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-159">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="9ee6c-160">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="9ee6c-160">deviceStatusOverview</span></span>|[<span data-ttu-id="9ee6c-161">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9ee6c-161">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="9ee6c-162">Visão geral de status de dispositivos para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9ee6c-162">Device compliance devices status overview</span></span>|
|<span data-ttu-id="9ee6c-163">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="9ee6c-163">userStatusOverview</span></span>|[<span data-ttu-id="9ee6c-164">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="9ee6c-164">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="9ee6c-165">Visão geral de status de usuários para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9ee6c-165">Device compliance users status overview</span></span>|
|<span data-ttu-id="9ee6c-166">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="9ee6c-166">deviceSettingStateSummaries</span></span>|<span data-ttu-id="9ee6c-167">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="9ee6c-168">Resumo do dispositivo para estado de configuração de conformidade</span><span class="sxs-lookup"><span data-stu-id="9ee6c-168">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="9ee6c-169">assignments</span><span class="sxs-lookup"><span data-stu-id="9ee6c-169">assignments</span></span>|<span data-ttu-id="9ee6c-170">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="9ee6c-171">A coleção de atribuições para essa política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-171">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ee6c-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ee6c-172">JSON Representation</span></span>
<span data-ttu-id="9ee6c-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-173">Here is a JSON representation of the resource.</span></span>
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







