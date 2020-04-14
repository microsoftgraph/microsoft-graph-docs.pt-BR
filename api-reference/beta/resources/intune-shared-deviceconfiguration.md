---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db852683da51975edd1841860478685cb588fb53
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356550"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="11724-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11724-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="11724-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11724-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11724-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11724-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11724-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11724-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11724-107">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-107">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="11724-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="11724-108">Methods</span></span>
|<span data-ttu-id="11724-109">Método</span><span class="sxs-lookup"><span data-stu-id="11724-109">Method</span></span>|<span data-ttu-id="11724-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11724-110">Return Type</span></span>|<span data-ttu-id="11724-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11724-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11724-112">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="11724-112">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="11724-113">Conjunto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11724-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="11724-114">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="11724-114">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="11724-115">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11724-115">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="11724-116">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11724-116">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="11724-117">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="11724-117">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="11724-118">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="11724-118">**Device configuration**</span></span>|
|[<span data-ttu-id="11724-119">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="11724-119">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="11724-120">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11724-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11724-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11724-121">Not yet documented</span></span>|
|[<span data-ttu-id="11724-122">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="11724-122">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="11724-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="11724-123">None</span></span>|<span data-ttu-id="11724-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11724-124">Not yet documented</span></span>|
|[<span data-ttu-id="11724-125">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="11724-125">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="11724-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="11724-126">None</span></span>|<span data-ttu-id="11724-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11724-127">Not yet documented</span></span>|
|[<span data-ttu-id="11724-128">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="11724-128">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="11724-129">coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="11724-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="11724-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11724-130">Not yet documented</span></span>|
|<span data-ttu-id="11724-131">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="11724-131">**Policy Set**</span></span>|
|[<span data-ttu-id="11724-132">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="11724-132">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="11724-133">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="11724-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="11724-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="11724-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="11724-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11724-135">Properties</span></span>
|<span data-ttu-id="11724-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11724-136">Property</span></span>|<span data-ttu-id="11724-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="11724-137">Type</span></span>|<span data-ttu-id="11724-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="11724-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11724-139">id</span><span class="sxs-lookup"><span data-stu-id="11724-139">id</span></span>|<span data-ttu-id="11724-140">String</span><span class="sxs-lookup"><span data-stu-id="11724-140">String</span></span>|<span data-ttu-id="11724-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="11724-141">Key of the entity.</span></span>|
|<span data-ttu-id="11724-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11724-142">lastModifiedDateTime</span></span>|<span data-ttu-id="11724-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11724-143">DateTimeOffset</span></span>|<span data-ttu-id="11724-144">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="11724-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="11724-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11724-145">roleScopeTagIds</span></span>|<span data-ttu-id="11724-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="11724-146">String collection</span></span>|<span data-ttu-id="11724-147">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="11724-147">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="11724-148">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="11724-148">supportsScopeTags</span></span>|<span data-ttu-id="11724-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="11724-149">Boolean</span></span>|<span data-ttu-id="11724-150">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="11724-150">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="11724-151">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="11724-151">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="11724-152">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="11724-152">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="11724-153">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11724-153">This property is read-only.</span></span>|
|<span data-ttu-id="11724-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="11724-154">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="11724-155">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="11724-155">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="11724-156">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="11724-156">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="11724-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="11724-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="11724-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="11724-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="11724-159">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="11724-159">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="11724-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="11724-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="11724-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="11724-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="11724-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="11724-162">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="11724-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11724-163">createdDateTime</span></span>|<span data-ttu-id="11724-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11724-164">DateTimeOffset</span></span>|<span data-ttu-id="11724-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="11724-165">DateTime the object was created.</span></span>|
|<span data-ttu-id="11724-166">description</span><span class="sxs-lookup"><span data-stu-id="11724-166">description</span></span>|<span data-ttu-id="11724-167">String</span><span class="sxs-lookup"><span data-stu-id="11724-167">String</span></span>|<span data-ttu-id="11724-168">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-168">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="11724-169">displayName</span><span class="sxs-lookup"><span data-stu-id="11724-169">displayName</span></span>|<span data-ttu-id="11724-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11724-170">String</span></span>|<span data-ttu-id="11724-171">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-171">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="11724-172">versão</span><span class="sxs-lookup"><span data-stu-id="11724-172">version</span></span>|<span data-ttu-id="11724-173">Int32</span><span class="sxs-lookup"><span data-stu-id="11724-173">Int32</span></span>|<span data-ttu-id="11724-174">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-174">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11724-175">Relações</span><span class="sxs-lookup"><span data-stu-id="11724-175">Relationships</span></span>
|<span data-ttu-id="11724-176">Relação</span><span class="sxs-lookup"><span data-stu-id="11724-176">Relationship</span></span>|<span data-ttu-id="11724-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="11724-177">Type</span></span>|<span data-ttu-id="11724-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="11724-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11724-179">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="11724-179">**Device configuration**</span></span>|
|<span data-ttu-id="11724-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="11724-180">groupAssignments</span></span>|<span data-ttu-id="11724-181">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11724-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="11724-182">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-182">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="11724-183">assignments</span><span class="sxs-lookup"><span data-stu-id="11724-183">assignments</span></span>|<span data-ttu-id="11724-184">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11724-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11724-185">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-185">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="11724-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="11724-186">deviceStatuses</span></span>|<span data-ttu-id="11724-187">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="11724-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="11724-188">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11724-188">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="11724-189">userStatuses</span><span class="sxs-lookup"><span data-stu-id="11724-189">userStatuses</span></span>|<span data-ttu-id="11724-190">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="11724-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="11724-191">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="11724-191">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="11724-192">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="11724-192">deviceStatusOverview</span></span>|[<span data-ttu-id="11724-193">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="11724-193">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="11724-194">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="11724-194">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="11724-195">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="11724-195">userStatusOverview</span></span>|[<span data-ttu-id="11724-196">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="11724-196">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="11724-197">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="11724-197">Device Configuration users status overview</span></span>|
|<span data-ttu-id="11724-198">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="11724-198">deviceSettingStateSummaries</span></span>|<span data-ttu-id="11724-199">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="11724-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="11724-200">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11724-200">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11724-201">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11724-201">JSON Representation</span></span>
<span data-ttu-id="11724-202">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11724-202">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



