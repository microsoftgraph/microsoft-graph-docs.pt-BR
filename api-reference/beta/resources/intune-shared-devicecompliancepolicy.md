---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46aa0a0136bbc2ad00fdf70d4ab9a8d3bc6ef7f1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867291"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="afb59-104">Tipo de recurso deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="afb59-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="afb59-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb59-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afb59-106">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afb59-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afb59-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afb59-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afb59-108">Esta é a classe base para a política de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="afb59-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="afb59-109">Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui.</span><span class="sxs-lookup"><span data-stu-id="afb59-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="afb59-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="afb59-110">Methods</span></span>
|<span data-ttu-id="afb59-111">Método</span><span class="sxs-lookup"><span data-stu-id="afb59-111">Method</span></span>|<span data-ttu-id="afb59-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="afb59-112">Return Type</span></span>|<span data-ttu-id="afb59-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb59-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="afb59-114">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="afb59-114">List deviceCompliancePolicies</span></span>](../api/intune-shared-devicecompliancepolicy-list.md)|<span data-ttu-id="afb59-115">Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="afb59-116">Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afb59-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="afb59-117">Obter deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="afb59-117">Get deviceCompliancePolicy</span></span>](../api/intune-shared-devicecompliancepolicy-get.md)|[<span data-ttu-id="afb59-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="afb59-118">deviceCompliancePolicy</span></span>](../resources/intune-shared-devicecompliancepolicy.md)|<span data-ttu-id="afb59-119">Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afb59-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>|
|<span data-ttu-id="afb59-120">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="afb59-120">**Device configuration**</span></span>|
|[<span data-ttu-id="afb59-121">ação assign</span><span class="sxs-lookup"><span data-stu-id="afb59-121">assign action</span></span>](../api/intune-shared-devicecompliancepolicy-assign.md)|<span data-ttu-id="afb59-122">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="afb59-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="afb59-123">Not yet documented</span></span>|
|<span data-ttu-id="afb59-124">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="afb59-124">scheduleActionsForRules action</span></span>|<span data-ttu-id="afb59-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="afb59-125">None</span></span>|<span data-ttu-id="afb59-126">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="afb59-126">Not yet documented</span></span>|
|<span data-ttu-id="afb59-127">ação refreshDeviceComplianceReportSummarization](.. /api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-127">refreshDeviceComplianceReportSummarization action](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span></span>|<span data-ttu-id="afb59-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="afb59-128">None</span></span>|<span data-ttu-id="afb59-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="afb59-129">Not yet documented</span></span>|
|<span data-ttu-id="afb59-130">**Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="afb59-130">**Policy Set**</span></span>|
|[<span data-ttu-id="afb59-131">Ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="afb59-131">hasPayloadLinks action</span></span>](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|<span data-ttu-id="afb59-132">[coleção hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="afb59-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="afb59-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="afb59-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afb59-134">Properties</span></span>
|<span data-ttu-id="afb59-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afb59-135">Property</span></span>|<span data-ttu-id="afb59-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="afb59-136">Type</span></span>|<span data-ttu-id="afb59-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb59-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb59-138">id</span><span class="sxs-lookup"><span data-stu-id="afb59-138">id</span></span>|<span data-ttu-id="afb59-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb59-139">String</span></span>|<span data-ttu-id="afb59-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afb59-140">Key of the entity.</span></span>|
|<span data-ttu-id="afb59-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afb59-141">roleScopeTagIds</span></span>|<span data-ttu-id="afb59-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="afb59-142">String collection</span></span>|<span data-ttu-id="afb59-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="afb59-143">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="afb59-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afb59-144">createdDateTime</span></span>|<span data-ttu-id="afb59-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb59-145">DateTimeOffset</span></span>|<span data-ttu-id="afb59-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="afb59-146">DateTime the object was created.</span></span>|
|<span data-ttu-id="afb59-147">description</span><span class="sxs-lookup"><span data-stu-id="afb59-147">description</span></span>|<span data-ttu-id="afb59-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb59-148">String</span></span>|<span data-ttu-id="afb59-149">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afb59-149">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="afb59-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afb59-150">lastModifiedDateTime</span></span>|<span data-ttu-id="afb59-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb59-151">DateTimeOffset</span></span>|<span data-ttu-id="afb59-152">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="afb59-152">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="afb59-153">displayName</span><span class="sxs-lookup"><span data-stu-id="afb59-153">displayName</span></span>|<span data-ttu-id="afb59-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb59-154">String</span></span>|<span data-ttu-id="afb59-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afb59-155">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="afb59-156">versão</span><span class="sxs-lookup"><span data-stu-id="afb59-156">version</span></span>|<span data-ttu-id="afb59-157">Int32</span><span class="sxs-lookup"><span data-stu-id="afb59-157">Int32</span></span>|<span data-ttu-id="afb59-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afb59-158">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afb59-159">Relações</span><span class="sxs-lookup"><span data-stu-id="afb59-159">Relationships</span></span>
|<span data-ttu-id="afb59-160">Relação</span><span class="sxs-lookup"><span data-stu-id="afb59-160">Relationship</span></span>|<span data-ttu-id="afb59-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="afb59-161">Type</span></span>|<span data-ttu-id="afb59-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb59-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb59-163">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="afb59-163">**Device configuration**</span></span>|
|<span data-ttu-id="afb59-164">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="afb59-164">scheduledActionsForRule</span></span>|<span data-ttu-id="afb59-165">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="afb59-166">A lista de ações agendadas para essa regra</span><span class="sxs-lookup"><span data-stu-id="afb59-166">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="afb59-167">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="afb59-167">deviceStatuses</span></span>|<span data-ttu-id="afb59-168">Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="afb59-169">Lista de DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="afb59-169">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="afb59-170">userStatuses</span><span class="sxs-lookup"><span data-stu-id="afb59-170">userStatuses</span></span>|<span data-ttu-id="afb59-171">Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="afb59-172">Lista de DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="afb59-172">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="afb59-173">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="afb59-173">deviceStatusOverview</span></span>|[<span data-ttu-id="afb59-174">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="afb59-174">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="afb59-175">Visão geral de status de dispositivos para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="afb59-175">Device compliance devices status overview</span></span>|
|<span data-ttu-id="afb59-176">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="afb59-176">userStatusOverview</span></span>|[<span data-ttu-id="afb59-177">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="afb59-177">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="afb59-178">Visão geral de status de usuários para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="afb59-178">Device compliance users status overview</span></span>|
|<span data-ttu-id="afb59-179">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="afb59-179">deviceSettingStateSummaries</span></span>|<span data-ttu-id="afb59-180">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="afb59-181">Resumo do dispositivo para estado de configuração de conformidade</span><span class="sxs-lookup"><span data-stu-id="afb59-181">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="afb59-182">assignments</span><span class="sxs-lookup"><span data-stu-id="afb59-182">assignments</span></span>|<span data-ttu-id="afb59-183">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="afb59-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="afb59-184">A coleção de atribuições para essa política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="afb59-184">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="afb59-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afb59-185">JSON Representation</span></span>
<span data-ttu-id="afb59-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afb59-186">Here is a JSON representation of the resource.</span></span>
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




