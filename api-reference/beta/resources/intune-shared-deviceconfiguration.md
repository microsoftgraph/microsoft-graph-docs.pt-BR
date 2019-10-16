---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68204c747aa983ed44cf2c30fb056baaa7de7225
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539145"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="22861-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="22861-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="22861-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22861-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22861-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="22861-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="22861-107">Methods</span></span>
|<span data-ttu-id="22861-108">Método</span><span class="sxs-lookup"><span data-stu-id="22861-108">Method</span></span>|<span data-ttu-id="22861-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22861-109">Return Type</span></span>|<span data-ttu-id="22861-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22861-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22861-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="22861-111">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="22861-112">Conjunto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22861-112">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="22861-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22861-113">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="22861-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="22861-114">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="22861-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="22861-115">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="22861-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22861-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="22861-117">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="22861-117">**Device configuration**</span></span>|
|[<span data-ttu-id="22861-118">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="22861-118">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="22861-119">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="22861-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="22861-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22861-120">Not yet documented</span></span>|
|[<span data-ttu-id="22861-121">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="22861-121">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="22861-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="22861-122">None</span></span>|<span data-ttu-id="22861-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22861-123">Not yet documented</span></span>|
|[<span data-ttu-id="22861-124">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="22861-124">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="22861-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="22861-125">None</span></span>|<span data-ttu-id="22861-126">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22861-126">Not yet documented</span></span>|
|[<span data-ttu-id="22861-127">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="22861-127">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="22861-128">coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="22861-128">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="22861-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22861-129">Not yet documented</span></span>|
|<span data-ttu-id="22861-130">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="22861-130">**Policy Set**</span></span>|
|[<span data-ttu-id="22861-131">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="22861-131">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="22861-132">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="22861-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="22861-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22861-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="22861-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22861-134">Properties</span></span>
|<span data-ttu-id="22861-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22861-135">Property</span></span>|<span data-ttu-id="22861-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="22861-136">Type</span></span>|<span data-ttu-id="22861-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="22861-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22861-138">id</span><span class="sxs-lookup"><span data-stu-id="22861-138">id</span></span>|<span data-ttu-id="22861-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22861-139">String</span></span>|<span data-ttu-id="22861-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22861-140">Key of the entity.</span></span>|
|<span data-ttu-id="22861-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22861-141">lastModifiedDateTime</span></span>|<span data-ttu-id="22861-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22861-142">DateTimeOffset</span></span>|<span data-ttu-id="22861-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22861-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="22861-144">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22861-144">roleScopeTagIds</span></span>|<span data-ttu-id="22861-145">String collection</span><span class="sxs-lookup"><span data-stu-id="22861-145">String collection</span></span>|<span data-ttu-id="22861-146">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="22861-146">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="22861-147">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="22861-147">supportsScopeTags</span></span>|<span data-ttu-id="22861-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="22861-148">Boolean</span></span>|<span data-ttu-id="22861-149">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="22861-149">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22861-150">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="22861-150">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22861-151">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="22861-151">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22861-152">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22861-152">This property is read-only.</span></span>|
|<span data-ttu-id="22861-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22861-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22861-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22861-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22861-155">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="22861-155">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="22861-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22861-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22861-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22861-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22861-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="22861-158">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="22861-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22861-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22861-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22861-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22861-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="22861-161">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="22861-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22861-162">createdDateTime</span></span>|<span data-ttu-id="22861-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22861-163">DateTimeOffset</span></span>|<span data-ttu-id="22861-164">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22861-164">DateTime the object was created.</span></span>|
|<span data-ttu-id="22861-165">description</span><span class="sxs-lookup"><span data-stu-id="22861-165">description</span></span>|<span data-ttu-id="22861-166">String</span><span class="sxs-lookup"><span data-stu-id="22861-166">String</span></span>|<span data-ttu-id="22861-167">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-167">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="22861-168">displayName</span><span class="sxs-lookup"><span data-stu-id="22861-168">displayName</span></span>|<span data-ttu-id="22861-169">String</span><span class="sxs-lookup"><span data-stu-id="22861-169">String</span></span>|<span data-ttu-id="22861-170">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-170">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="22861-171">versão</span><span class="sxs-lookup"><span data-stu-id="22861-171">version</span></span>|<span data-ttu-id="22861-172">Int32</span><span class="sxs-lookup"><span data-stu-id="22861-172">Int32</span></span>|<span data-ttu-id="22861-173">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-173">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22861-174">Relações</span><span class="sxs-lookup"><span data-stu-id="22861-174">Relationships</span></span>
|<span data-ttu-id="22861-175">Relação</span><span class="sxs-lookup"><span data-stu-id="22861-175">Relationship</span></span>|<span data-ttu-id="22861-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="22861-176">Type</span></span>|<span data-ttu-id="22861-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="22861-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22861-178">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="22861-178">**Device configuration**</span></span>|
|<span data-ttu-id="22861-179">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="22861-179">groupAssignments</span></span>|<span data-ttu-id="22861-180">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="22861-180">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="22861-181">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-181">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="22861-182">assignments</span><span class="sxs-lookup"><span data-stu-id="22861-182">assignments</span></span>|<span data-ttu-id="22861-183">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="22861-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="22861-184">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-184">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="22861-185">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="22861-185">deviceStatuses</span></span>|<span data-ttu-id="22861-186">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="22861-186">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="22861-187">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22861-187">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="22861-188">userStatuses</span><span class="sxs-lookup"><span data-stu-id="22861-188">userStatuses</span></span>|<span data-ttu-id="22861-189">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22861-189">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="22861-190">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="22861-190">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="22861-191">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="22861-191">deviceStatusOverview</span></span>|[<span data-ttu-id="22861-192">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="22861-192">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="22861-193">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="22861-193">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="22861-194">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="22861-194">userStatusOverview</span></span>|[<span data-ttu-id="22861-195">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="22861-195">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="22861-196">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="22861-196">Device Configuration users status overview</span></span>|
|<span data-ttu-id="22861-197">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="22861-197">deviceSettingStateSummaries</span></span>|<span data-ttu-id="22861-198">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="22861-198">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="22861-199">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="22861-199">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22861-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22861-200">JSON Representation</span></span>
<span data-ttu-id="22861-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22861-201">Here is a JSON representation of the resource.</span></span>
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



