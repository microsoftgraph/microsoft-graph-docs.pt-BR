---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5a82af9a6d5de359891498b32489a899e3b8f82
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306888"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="b1688-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1688-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="b1688-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1688-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1688-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1688-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1688-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1688-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1688-107">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-107">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="b1688-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b1688-108">Methods</span></span>
|<span data-ttu-id="b1688-109">Método</span><span class="sxs-lookup"><span data-stu-id="b1688-109">Method</span></span>|<span data-ttu-id="b1688-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1688-110">Return Type</span></span>|<span data-ttu-id="b1688-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1688-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1688-112">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="b1688-112">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="b1688-113">Conjunto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="b1688-114">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1688-114">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b1688-115">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1688-115">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="b1688-116">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1688-116">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="b1688-117">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1688-117">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="b1688-118">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b1688-118">**Device configuration**</span></span>|
|[<span data-ttu-id="b1688-119">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b1688-119">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="b1688-120">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b1688-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1688-121">Not yet documented</span></span>|
|[<span data-ttu-id="b1688-122">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="b1688-122">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="b1688-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b1688-123">None</span></span>|<span data-ttu-id="b1688-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1688-124">Not yet documented</span></span>|
|[<span data-ttu-id="b1688-125">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="b1688-125">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="b1688-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b1688-126">None</span></span>|<span data-ttu-id="b1688-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1688-127">Not yet documented</span></span>|
|[<span data-ttu-id="b1688-128">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="b1688-128">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="b1688-129">coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="b1688-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1688-130">Not yet documented</span></span>|
|<span data-ttu-id="b1688-131">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b1688-131">**Policy Set**</span></span>|
|[<span data-ttu-id="b1688-132">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="b1688-132">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="b1688-133">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="b1688-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1688-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b1688-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1688-135">Properties</span></span>
|<span data-ttu-id="b1688-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1688-136">Property</span></span>|<span data-ttu-id="b1688-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1688-137">Type</span></span>|<span data-ttu-id="b1688-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1688-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1688-139">id</span><span class="sxs-lookup"><span data-stu-id="b1688-139">id</span></span>|<span data-ttu-id="b1688-140">String</span><span class="sxs-lookup"><span data-stu-id="b1688-140">String</span></span>|<span data-ttu-id="b1688-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1688-141">Key of the entity.</span></span>|
|<span data-ttu-id="b1688-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1688-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b1688-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1688-143">DateTimeOffset</span></span>|<span data-ttu-id="b1688-144">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b1688-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b1688-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1688-145">roleScopeTagIds</span></span>|<span data-ttu-id="b1688-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1688-146">String collection</span></span>|<span data-ttu-id="b1688-147">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b1688-147">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="b1688-148">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b1688-148">supportsScopeTags</span></span>|<span data-ttu-id="b1688-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1688-149">Boolean</span></span>|<span data-ttu-id="b1688-150">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b1688-150">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b1688-151">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b1688-151">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b1688-152">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1688-152">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b1688-153">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1688-153">This property is read-only.</span></span>|
|<span data-ttu-id="b1688-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1688-154">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b1688-155">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1688-155">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b1688-156">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b1688-156">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="b1688-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1688-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b1688-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1688-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b1688-159">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b1688-159">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="b1688-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1688-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b1688-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1688-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b1688-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b1688-162">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="b1688-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1688-163">createdDateTime</span></span>|<span data-ttu-id="b1688-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1688-164">DateTimeOffset</span></span>|<span data-ttu-id="b1688-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b1688-165">DateTime the object was created.</span></span>|
|<span data-ttu-id="b1688-166">description</span><span class="sxs-lookup"><span data-stu-id="b1688-166">description</span></span>|<span data-ttu-id="b1688-167">String</span><span class="sxs-lookup"><span data-stu-id="b1688-167">String</span></span>|<span data-ttu-id="b1688-168">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-168">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="b1688-169">displayName</span><span class="sxs-lookup"><span data-stu-id="b1688-169">displayName</span></span>|<span data-ttu-id="b1688-170">String</span><span class="sxs-lookup"><span data-stu-id="b1688-170">String</span></span>|<span data-ttu-id="b1688-171">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-171">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="b1688-172">versão</span><span class="sxs-lookup"><span data-stu-id="b1688-172">version</span></span>|<span data-ttu-id="b1688-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b1688-173">Int32</span></span>|<span data-ttu-id="b1688-174">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-174">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1688-175">Relações</span><span class="sxs-lookup"><span data-stu-id="b1688-175">Relationships</span></span>
|<span data-ttu-id="b1688-176">Relação</span><span class="sxs-lookup"><span data-stu-id="b1688-176">Relationship</span></span>|<span data-ttu-id="b1688-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1688-177">Type</span></span>|<span data-ttu-id="b1688-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1688-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1688-179">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b1688-179">**Device configuration**</span></span>|
|<span data-ttu-id="b1688-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="b1688-180">groupAssignments</span></span>|<span data-ttu-id="b1688-181">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="b1688-182">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-182">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="b1688-183">assignments</span><span class="sxs-lookup"><span data-stu-id="b1688-183">assignments</span></span>|<span data-ttu-id="b1688-184">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b1688-185">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-185">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="b1688-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b1688-186">deviceStatuses</span></span>|<span data-ttu-id="b1688-187">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b1688-188">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1688-188">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="b1688-189">userStatuses</span><span class="sxs-lookup"><span data-stu-id="b1688-189">userStatuses</span></span>|<span data-ttu-id="b1688-190">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="b1688-191">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="b1688-191">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="b1688-192">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="b1688-192">deviceStatusOverview</span></span>|[<span data-ttu-id="b1688-193">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b1688-193">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="b1688-194">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b1688-194">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="b1688-195">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="b1688-195">userStatusOverview</span></span>|[<span data-ttu-id="b1688-196">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="b1688-196">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="b1688-197">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b1688-197">Device Configuration users status overview</span></span>|
|<span data-ttu-id="b1688-198">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b1688-198">deviceSettingStateSummaries</span></span>|<span data-ttu-id="b1688-199">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="b1688-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="b1688-200">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b1688-200">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1688-201">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1688-201">JSON Representation</span></span>
<span data-ttu-id="b1688-202">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1688-202">Here is a JSON representation of the resource.</span></span>
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




