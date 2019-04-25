---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d17bbba221fd95405b2f92f05efa607787b28145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566777"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="c7ed6-104">Tipo de recurso deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7ed6-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="c7ed6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7ed6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7ed6-107">Esta é a classe base para a política de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="c7ed6-108">Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="c7ed6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7ed6-109">Methods</span></span>
|<span data-ttu-id="c7ed6-110">Método</span><span class="sxs-lookup"><span data-stu-id="c7ed6-110">Method</span></span>|<span data-ttu-id="c7ed6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7ed6-111">Return Type</span></span>|<span data-ttu-id="c7ed6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7ed6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7ed6-113">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="c7ed6-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="c7ed6-114">Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="c7ed6-115">Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7ed6-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="c7ed6-116">Obter deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7ed6-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="c7ed6-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7ed6-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="c7ed6-118">Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7ed6-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="c7ed6-119">ação assign</span><span class="sxs-lookup"><span data-stu-id="c7ed6-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="c7ed6-120">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c7ed6-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7ed6-121">Not yet documented</span></span>|
|[<span data-ttu-id="c7ed6-122">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="c7ed6-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="c7ed6-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c7ed6-123">None</span></span>|<span data-ttu-id="c7ed6-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7ed6-124">Not yet documented</span></span>|
|[<span data-ttu-id="c7ed6-125">ação refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="c7ed6-125">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="c7ed6-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c7ed6-126">None</span></span>|<span data-ttu-id="c7ed6-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7ed6-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c7ed6-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7ed6-128">Properties</span></span>
|<span data-ttu-id="c7ed6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7ed6-129">Property</span></span>|<span data-ttu-id="c7ed6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7ed6-130">Type</span></span>|<span data-ttu-id="c7ed6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7ed6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ed6-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7ed6-132">roleScopeTagIds</span></span>|<span data-ttu-id="c7ed6-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7ed6-133">String collection</span></span>|<span data-ttu-id="c7ed6-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-134">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="c7ed6-135">id</span><span class="sxs-lookup"><span data-stu-id="c7ed6-135">id</span></span>|<span data-ttu-id="c7ed6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7ed6-136">String</span></span>|<span data-ttu-id="c7ed6-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-137">Key of the entity.</span></span>|
|<span data-ttu-id="c7ed6-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7ed6-138">createdDateTime</span></span>|<span data-ttu-id="c7ed6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7ed6-139">DateTimeOffset</span></span>|<span data-ttu-id="c7ed6-140">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="c7ed6-141">description</span><span class="sxs-lookup"><span data-stu-id="c7ed6-141">description</span></span>|<span data-ttu-id="c7ed6-142">String</span><span class="sxs-lookup"><span data-stu-id="c7ed6-142">String</span></span>|<span data-ttu-id="c7ed6-143">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-143">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c7ed6-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7ed6-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c7ed6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7ed6-145">DateTimeOffset</span></span>|<span data-ttu-id="c7ed6-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c7ed6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c7ed6-147">displayName</span></span>|<span data-ttu-id="c7ed6-148">String</span><span class="sxs-lookup"><span data-stu-id="c7ed6-148">String</span></span>|<span data-ttu-id="c7ed6-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-149">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c7ed6-150">versão</span><span class="sxs-lookup"><span data-stu-id="c7ed6-150">version</span></span>|<span data-ttu-id="c7ed6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c7ed6-151">Int32</span></span>|<span data-ttu-id="c7ed6-152">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-152">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7ed6-153">Relações</span><span class="sxs-lookup"><span data-stu-id="c7ed6-153">Relationships</span></span>
|<span data-ttu-id="c7ed6-154">Relação</span><span class="sxs-lookup"><span data-stu-id="c7ed6-154">Relationship</span></span>|<span data-ttu-id="c7ed6-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7ed6-155">Type</span></span>|<span data-ttu-id="c7ed6-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7ed6-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ed6-157">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="c7ed6-157">scheduledActionsForRule</span></span>|<span data-ttu-id="c7ed6-158">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="c7ed6-159">A lista de ações agendadas para essa regra</span><span class="sxs-lookup"><span data-stu-id="c7ed6-159">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="c7ed6-160">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c7ed6-160">deviceStatuses</span></span>|<span data-ttu-id="c7ed6-161">Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="c7ed6-162">Lista de DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-162">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="c7ed6-163">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c7ed6-163">userStatuses</span></span>|<span data-ttu-id="c7ed6-164">Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="c7ed6-165">Lista de DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-165">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="c7ed6-166">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7ed6-166">deviceStatusOverview</span></span>|[<span data-ttu-id="c7ed6-167">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c7ed6-167">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="c7ed6-168">Visão geral de status de dispositivos para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c7ed6-168">Device compliance devices status overview</span></span>|
|<span data-ttu-id="c7ed6-169">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7ed6-169">userStatusOverview</span></span>|[<span data-ttu-id="c7ed6-170">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="c7ed6-170">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="c7ed6-171">Visão geral de status de usuários para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c7ed6-171">Device compliance users status overview</span></span>|
|<span data-ttu-id="c7ed6-172">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c7ed6-172">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c7ed6-173">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c7ed6-174">Resumo do dispositivo para estado de configuração de conformidade</span><span class="sxs-lookup"><span data-stu-id="c7ed6-174">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="c7ed6-175">assignments</span><span class="sxs-lookup"><span data-stu-id="c7ed6-175">assignments</span></span>|<span data-ttu-id="c7ed6-176">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed6-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c7ed6-177">A coleção de atribuições para essa política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-177">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7ed6-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7ed6-178">JSON Representation</span></span>
<span data-ttu-id="c7ed6-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7ed6-179">Here is a JSON representation of the resource.</span></span>
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





