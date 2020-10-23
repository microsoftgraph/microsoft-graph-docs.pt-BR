---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9864efb295216ef338cc326a7244cbd90adc164e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684383"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="a72c6-104">Tipo de recurso deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a72c6-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="a72c6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a72c6-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a72c6-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a72c6-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a72c6-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a72c6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a72c6-108">Esta é a classe base para a política de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="a72c6-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="a72c6-109">Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui.</span><span class="sxs-lookup"><span data-stu-id="a72c6-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span>

## <a name="methods"></a><span data-ttu-id="a72c6-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="a72c6-110">Methods</span></span>
|<span data-ttu-id="a72c6-111">Método</span><span class="sxs-lookup"><span data-stu-id="a72c6-111">Method</span></span>|<span data-ttu-id="a72c6-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a72c6-112">Return Type</span></span>|<span data-ttu-id="a72c6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72c6-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a72c6-114">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="a72c6-114">List deviceCompliancePolicies</span></span>](../api/intune-shared-devicecompliancepolicy-list.md)|<span data-ttu-id="a72c6-115">Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="a72c6-116">Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a72c6-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="a72c6-117">Obter deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a72c6-117">Get deviceCompliancePolicy</span></span>](../api/intune-shared-devicecompliancepolicy-get.md)|[<span data-ttu-id="a72c6-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a72c6-118">deviceCompliancePolicy</span></span>](../resources/intune-shared-devicecompliancepolicy.md)|<span data-ttu-id="a72c6-119">Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a72c6-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>|
|<span data-ttu-id="a72c6-120">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="a72c6-120">**Device configuration**</span></span>|
|[<span data-ttu-id="a72c6-121">ação assign</span><span class="sxs-lookup"><span data-stu-id="a72c6-121">assign action</span></span>](../api/intune-shared-devicecompliancepolicy-assign.md)|<span data-ttu-id="a72c6-122">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="a72c6-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a72c6-123">Not yet documented</span></span>|
|<span data-ttu-id="a72c6-124">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="a72c6-124">scheduleActionsForRules action</span></span>|<span data-ttu-id="a72c6-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a72c6-125">None</span></span>|<span data-ttu-id="a72c6-126">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a72c6-126">Not yet documented</span></span>|
|<span data-ttu-id="a72c6-127">ação refreshDeviceComplianceReportSummarization] (.. /api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-127">refreshDeviceComplianceReportSummarization action](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span></span>|<span data-ttu-id="a72c6-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a72c6-128">None</span></span>|<span data-ttu-id="a72c6-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a72c6-129">Not yet documented</span></span>|
|<span data-ttu-id="a72c6-130">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a72c6-130">**Policy Set**</span></span>|
|[<span data-ttu-id="a72c6-131">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="a72c6-131">hasPayloadLinks action</span></span>](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|<span data-ttu-id="a72c6-132">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="a72c6-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a72c6-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a72c6-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a72c6-134">Properties</span></span>
|<span data-ttu-id="a72c6-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a72c6-135">Property</span></span>|<span data-ttu-id="a72c6-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a72c6-136">Type</span></span>|<span data-ttu-id="a72c6-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72c6-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a72c6-138">id</span><span class="sxs-lookup"><span data-stu-id="a72c6-138">id</span></span>|<span data-ttu-id="a72c6-139">String</span><span class="sxs-lookup"><span data-stu-id="a72c6-139">String</span></span>|<span data-ttu-id="a72c6-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a72c6-140">Key of the entity.</span></span>|
|<span data-ttu-id="a72c6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a72c6-141">roleScopeTagIds</span></span>|<span data-ttu-id="a72c6-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a72c6-142">String collection</span></span>|<span data-ttu-id="a72c6-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a72c6-143">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="a72c6-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a72c6-144">createdDateTime</span></span>|<span data-ttu-id="a72c6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a72c6-145">DateTimeOffset</span></span>|<span data-ttu-id="a72c6-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a72c6-146">DateTime the object was created.</span></span>|
|<span data-ttu-id="a72c6-147">description</span><span class="sxs-lookup"><span data-stu-id="a72c6-147">description</span></span>|<span data-ttu-id="a72c6-148">String</span><span class="sxs-lookup"><span data-stu-id="a72c6-148">String</span></span>|<span data-ttu-id="a72c6-149">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a72c6-149">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a72c6-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a72c6-150">lastModifiedDateTime</span></span>|<span data-ttu-id="a72c6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a72c6-151">DateTimeOffset</span></span>|<span data-ttu-id="a72c6-152">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a72c6-152">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a72c6-153">displayName</span><span class="sxs-lookup"><span data-stu-id="a72c6-153">displayName</span></span>|<span data-ttu-id="a72c6-154">String</span><span class="sxs-lookup"><span data-stu-id="a72c6-154">String</span></span>|<span data-ttu-id="a72c6-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a72c6-155">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a72c6-156">versão</span><span class="sxs-lookup"><span data-stu-id="a72c6-156">version</span></span>|<span data-ttu-id="a72c6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a72c6-157">Int32</span></span>|<span data-ttu-id="a72c6-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a72c6-158">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a72c6-159">Relações</span><span class="sxs-lookup"><span data-stu-id="a72c6-159">Relationships</span></span>
|<span data-ttu-id="a72c6-160">Relação</span><span class="sxs-lookup"><span data-stu-id="a72c6-160">Relationship</span></span>|<span data-ttu-id="a72c6-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="a72c6-161">Type</span></span>|<span data-ttu-id="a72c6-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72c6-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a72c6-163">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="a72c6-163">**Device configuration**</span></span>|
|<span data-ttu-id="a72c6-164">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="a72c6-164">scheduledActionsForRule</span></span>|<span data-ttu-id="a72c6-165">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="a72c6-166">A lista de ações agendadas para essa regra</span><span class="sxs-lookup"><span data-stu-id="a72c6-166">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="a72c6-167">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a72c6-167">deviceStatuses</span></span>|<span data-ttu-id="a72c6-168">Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="a72c6-169">Lista de DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="a72c6-169">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="a72c6-170">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a72c6-170">userStatuses</span></span>|<span data-ttu-id="a72c6-171">Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="a72c6-172">Lista de DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="a72c6-172">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="a72c6-173">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a72c6-173">deviceStatusOverview</span></span>|[<span data-ttu-id="a72c6-174">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a72c6-174">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="a72c6-175">Visão geral de status de dispositivos para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a72c6-175">Device compliance devices status overview</span></span>|
|<span data-ttu-id="a72c6-176">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a72c6-176">userStatusOverview</span></span>|[<span data-ttu-id="a72c6-177">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="a72c6-177">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="a72c6-178">Visão geral de status de usuários para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a72c6-178">Device compliance users status overview</span></span>|
|<span data-ttu-id="a72c6-179">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a72c6-179">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a72c6-180">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a72c6-181">Resumo do dispositivo para estado de configuração de conformidade</span><span class="sxs-lookup"><span data-stu-id="a72c6-181">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="a72c6-182">assignments</span><span class="sxs-lookup"><span data-stu-id="a72c6-182">assignments</span></span>|<span data-ttu-id="a72c6-183">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a72c6-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="a72c6-184">A coleção de atribuições para essa política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="a72c6-184">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a72c6-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a72c6-185">JSON Representation</span></span>
<span data-ttu-id="a72c6-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a72c6-186">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





