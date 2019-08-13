---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88f1dc66fbbb95b4b8f9a340949f41f573eb22fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333041"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="adb96-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="adb96-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="adb96-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="adb96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adb96-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="adb96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adb96-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="adb96-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="adb96-107">Methods</span></span>
|<span data-ttu-id="adb96-108">Método</span><span class="sxs-lookup"><span data-stu-id="adb96-108">Method</span></span>|<span data-ttu-id="adb96-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="adb96-109">Return Type</span></span>|<span data-ttu-id="adb96-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb96-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="adb96-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="adb96-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="adb96-112">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="adb96-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb96-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="adb96-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="adb96-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="adb96-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="adb96-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="adb96-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb96-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="adb96-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="adb96-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="adb96-118">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="adb96-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adb96-119">Not yet documented</span></span>|
|[<span data-ttu-id="adb96-120">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="adb96-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="adb96-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="adb96-121">None</span></span>|<span data-ttu-id="adb96-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adb96-122">Not yet documented</span></span>|
|[<span data-ttu-id="adb96-123">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="adb96-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="adb96-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="adb96-124">None</span></span>|<span data-ttu-id="adb96-125">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adb96-125">Not yet documented</span></span>|
|[<span data-ttu-id="adb96-126">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="adb96-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="adb96-127">coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="adb96-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adb96-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="adb96-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="adb96-129">Properties</span></span>
|<span data-ttu-id="adb96-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adb96-130">Property</span></span>|<span data-ttu-id="adb96-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="adb96-131">Type</span></span>|<span data-ttu-id="adb96-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb96-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adb96-133">id</span><span class="sxs-lookup"><span data-stu-id="adb96-133">id</span></span>|<span data-ttu-id="adb96-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb96-134">String</span></span>|<span data-ttu-id="adb96-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="adb96-135">Key of the entity.</span></span>|
|<span data-ttu-id="adb96-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adb96-136">lastModifiedDateTime</span></span>|<span data-ttu-id="adb96-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb96-137">DateTimeOffset</span></span>|<span data-ttu-id="adb96-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="adb96-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="adb96-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="adb96-139">roleScopeTagIds</span></span>|<span data-ttu-id="adb96-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb96-140">String collection</span></span>|<span data-ttu-id="adb96-141">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="adb96-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="adb96-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="adb96-142">supportsScopeTags</span></span>|<span data-ttu-id="adb96-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="adb96-143">Boolean</span></span>|<span data-ttu-id="adb96-144">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="adb96-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="adb96-145">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="adb96-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="adb96-146">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="adb96-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="adb96-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="adb96-147">This property is read-only.</span></span>|
|<span data-ttu-id="adb96-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="adb96-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="adb96-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="adb96-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="adb96-150">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="adb96-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="adb96-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="adb96-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="adb96-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="adb96-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="adb96-153">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="adb96-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="adb96-154">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="adb96-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="adb96-155">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="adb96-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="adb96-156">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="adb96-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="adb96-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adb96-157">createdDateTime</span></span>|<span data-ttu-id="adb96-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb96-158">DateTimeOffset</span></span>|<span data-ttu-id="adb96-159">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="adb96-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="adb96-160">descrição</span><span class="sxs-lookup"><span data-stu-id="adb96-160">description</span></span>|<span data-ttu-id="adb96-161">String</span><span class="sxs-lookup"><span data-stu-id="adb96-161">String</span></span>|<span data-ttu-id="adb96-162">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="adb96-163">displayName</span><span class="sxs-lookup"><span data-stu-id="adb96-163">displayName</span></span>|<span data-ttu-id="adb96-164">String</span><span class="sxs-lookup"><span data-stu-id="adb96-164">String</span></span>|<span data-ttu-id="adb96-165">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="adb96-166">versão</span><span class="sxs-lookup"><span data-stu-id="adb96-166">version</span></span>|<span data-ttu-id="adb96-167">Int32</span><span class="sxs-lookup"><span data-stu-id="adb96-167">Int32</span></span>|<span data-ttu-id="adb96-168">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adb96-169">Relações</span><span class="sxs-lookup"><span data-stu-id="adb96-169">Relationships</span></span>
|<span data-ttu-id="adb96-170">Relação</span><span class="sxs-lookup"><span data-stu-id="adb96-170">Relationship</span></span>|<span data-ttu-id="adb96-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="adb96-171">Type</span></span>|<span data-ttu-id="adb96-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb96-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adb96-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="adb96-173">groupAssignments</span></span>|<span data-ttu-id="adb96-174">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="adb96-175">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="adb96-176">assignments</span><span class="sxs-lookup"><span data-stu-id="adb96-176">assignments</span></span>|<span data-ttu-id="adb96-177">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="adb96-178">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="adb96-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="adb96-179">deviceStatuses</span></span>|<span data-ttu-id="adb96-180">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="adb96-181">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adb96-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="adb96-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="adb96-182">userStatuses</span></span>|<span data-ttu-id="adb96-183">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="adb96-184">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="adb96-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="adb96-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="adb96-185">deviceStatusOverview</span></span>|[<span data-ttu-id="adb96-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="adb96-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="adb96-187">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="adb96-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="adb96-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="adb96-188">userStatusOverview</span></span>|[<span data-ttu-id="adb96-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="adb96-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="adb96-190">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="adb96-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="adb96-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="adb96-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="adb96-192">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="adb96-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="adb96-193">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="adb96-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adb96-194">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="adb96-194">JSON Representation</span></span>
<span data-ttu-id="adb96-195">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="adb96-195">Here is a JSON representation of the resource.</span></span>
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



