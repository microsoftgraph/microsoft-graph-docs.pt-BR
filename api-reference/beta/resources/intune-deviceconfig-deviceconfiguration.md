---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b9bc0bc5c2c589a1eaf1bceb989c981806d553f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001681"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="9178b-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9178b-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="9178b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9178b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9178b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9178b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9178b-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="9178b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9178b-107">Methods</span></span>
|<span data-ttu-id="9178b-108">Método</span><span class="sxs-lookup"><span data-stu-id="9178b-108">Method</span></span>|<span data-ttu-id="9178b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9178b-109">Return Type</span></span>|<span data-ttu-id="9178b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9178b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9178b-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="9178b-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="9178b-112">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="9178b-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9178b-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9178b-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9178b-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="9178b-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9178b-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="9178b-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9178b-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9178b-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="9178b-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="9178b-118">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9178b-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9178b-119">Not yet documented</span></span>|
|[<span data-ttu-id="9178b-120">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="9178b-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="9178b-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9178b-121">None</span></span>|<span data-ttu-id="9178b-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9178b-122">Not yet documented</span></span>|
|[<span data-ttu-id="9178b-123">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="9178b-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="9178b-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9178b-124">None</span></span>|<span data-ttu-id="9178b-125">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9178b-125">Not yet documented</span></span>|
|[<span data-ttu-id="9178b-126">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="9178b-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="9178b-127">coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="9178b-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9178b-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9178b-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9178b-129">Properties</span></span>
|<span data-ttu-id="9178b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9178b-130">Property</span></span>|<span data-ttu-id="9178b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9178b-131">Type</span></span>|<span data-ttu-id="9178b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9178b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9178b-133">id</span><span class="sxs-lookup"><span data-stu-id="9178b-133">id</span></span>|<span data-ttu-id="9178b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9178b-134">String</span></span>|<span data-ttu-id="9178b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9178b-135">Key of the entity.</span></span>|
|<span data-ttu-id="9178b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9178b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9178b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9178b-137">DateTimeOffset</span></span>|<span data-ttu-id="9178b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9178b-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9178b-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9178b-139">roleScopeTagIds</span></span>|<span data-ttu-id="9178b-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9178b-140">String collection</span></span>|<span data-ttu-id="9178b-141">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9178b-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="9178b-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9178b-142">supportsScopeTags</span></span>|<span data-ttu-id="9178b-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="9178b-143">Boolean</span></span>|<span data-ttu-id="9178b-144">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9178b-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9178b-145">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9178b-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9178b-146">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9178b-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9178b-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9178b-147">This property is read-only.</span></span>|
|<span data-ttu-id="9178b-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9178b-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9178b-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9178b-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9178b-150">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9178b-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="9178b-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9178b-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9178b-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9178b-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9178b-153">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9178b-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="9178b-154">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9178b-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9178b-155">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9178b-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9178b-156">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9178b-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="9178b-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9178b-157">createdDateTime</span></span>|<span data-ttu-id="9178b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9178b-158">DateTimeOffset</span></span>|<span data-ttu-id="9178b-159">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9178b-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="9178b-160">descrição</span><span class="sxs-lookup"><span data-stu-id="9178b-160">description</span></span>|<span data-ttu-id="9178b-161">String</span><span class="sxs-lookup"><span data-stu-id="9178b-161">String</span></span>|<span data-ttu-id="9178b-162">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="9178b-163">displayName</span><span class="sxs-lookup"><span data-stu-id="9178b-163">displayName</span></span>|<span data-ttu-id="9178b-164">String</span><span class="sxs-lookup"><span data-stu-id="9178b-164">String</span></span>|<span data-ttu-id="9178b-165">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="9178b-166">versão</span><span class="sxs-lookup"><span data-stu-id="9178b-166">version</span></span>|<span data-ttu-id="9178b-167">Int32</span><span class="sxs-lookup"><span data-stu-id="9178b-167">Int32</span></span>|<span data-ttu-id="9178b-168">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9178b-169">Relações</span><span class="sxs-lookup"><span data-stu-id="9178b-169">Relationships</span></span>
|<span data-ttu-id="9178b-170">Relação</span><span class="sxs-lookup"><span data-stu-id="9178b-170">Relationship</span></span>|<span data-ttu-id="9178b-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="9178b-171">Type</span></span>|<span data-ttu-id="9178b-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="9178b-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9178b-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="9178b-173">groupAssignments</span></span>|<span data-ttu-id="9178b-174">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="9178b-175">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="9178b-176">assignments</span><span class="sxs-lookup"><span data-stu-id="9178b-176">assignments</span></span>|<span data-ttu-id="9178b-177">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9178b-178">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="9178b-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="9178b-179">deviceStatuses</span></span>|<span data-ttu-id="9178b-180">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="9178b-181">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9178b-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="9178b-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="9178b-182">userStatuses</span></span>|<span data-ttu-id="9178b-183">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="9178b-184">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="9178b-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="9178b-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="9178b-185">deviceStatusOverview</span></span>|[<span data-ttu-id="9178b-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9178b-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="9178b-187">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9178b-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="9178b-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="9178b-188">userStatusOverview</span></span>|[<span data-ttu-id="9178b-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="9178b-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="9178b-190">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9178b-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="9178b-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="9178b-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="9178b-192">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9178b-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="9178b-193">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9178b-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9178b-194">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9178b-194">JSON Representation</span></span>
<span data-ttu-id="9178b-195">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9178b-195">Here is a JSON representation of the resource.</span></span>
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





