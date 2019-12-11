---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b68a4ee25a2a21826bc7b292f159b11f563a5ee
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949206"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="c706f-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c706f-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="c706f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c706f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c706f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c706f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c706f-106">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c706f-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c706f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c706f-107">Prerequisites</span></span>
<span data-ttu-id="c706f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c706f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c706f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c706f-110">Permission type</span></span>|<span data-ttu-id="c706f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c706f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c706f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c706f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c706f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c706f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c706f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c706f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c706f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c706f-115">Not supported.</span></span>|
|<span data-ttu-id="c706f-116">Application</span><span class="sxs-lookup"><span data-stu-id="c706f-116">Application</span></span>|<span data-ttu-id="c706f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c706f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c706f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c706f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c706f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c706f-119">Request headers</span></span>
|<span data-ttu-id="c706f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c706f-120">Header</span></span>|<span data-ttu-id="c706f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c706f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c706f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c706f-122">Authorization</span></span>|<span data-ttu-id="c706f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c706f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c706f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c706f-124">Accept</span></span>|<span data-ttu-id="c706f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c706f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c706f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c706f-126">Request body</span></span>
<span data-ttu-id="c706f-127">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c706f-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="c706f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c706f-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="c706f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c706f-129">Property</span></span>|<span data-ttu-id="c706f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c706f-130">Type</span></span>|<span data-ttu-id="c706f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c706f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c706f-132">id</span><span class="sxs-lookup"><span data-stu-id="c706f-132">id</span></span>|<span data-ttu-id="c706f-133">String</span><span class="sxs-lookup"><span data-stu-id="c706f-133">String</span></span>|<span data-ttu-id="c706f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c706f-134">Key of the entity.</span></span> <span data-ttu-id="c706f-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c706f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c706f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c706f-137">DateTimeOffset</span></span>|<span data-ttu-id="c706f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c706f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c706f-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c706f-140">roleScopeTagIds</span></span>|<span data-ttu-id="c706f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c706f-141">String collection</span></span>|<span data-ttu-id="c706f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c706f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c706f-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c706f-144">supportsScopeTags</span></span>|<span data-ttu-id="c706f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c706f-145">Boolean</span></span>|<span data-ttu-id="c706f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c706f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c706f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c706f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c706f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c706f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c706f-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c706f-149">This property is read-only.</span></span> <span data-ttu-id="c706f-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c706f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c706f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c706f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c706f-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c706f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c706f-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c706f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c706f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c706f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c706f-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c706f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c706f-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c706f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c706f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c706f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c706f-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c706f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c706f-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c706f-163">createdDateTime</span></span>|<span data-ttu-id="c706f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c706f-164">DateTimeOffset</span></span>|<span data-ttu-id="c706f-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c706f-165">DateTime the object was created.</span></span> <span data-ttu-id="c706f-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-167">description</span><span class="sxs-lookup"><span data-stu-id="c706f-167">description</span></span>|<span data-ttu-id="c706f-168">String</span><span class="sxs-lookup"><span data-stu-id="c706f-168">String</span></span>|<span data-ttu-id="c706f-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c706f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c706f-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c706f-171">displayName</span></span>|<span data-ttu-id="c706f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c706f-172">String</span></span>|<span data-ttu-id="c706f-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c706f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c706f-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-175">versão</span><span class="sxs-lookup"><span data-stu-id="c706f-175">version</span></span>|<span data-ttu-id="c706f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c706f-176">Int32</span></span>|<span data-ttu-id="c706f-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c706f-177">Version of the device configuration.</span></span> <span data-ttu-id="c706f-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c706f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c706f-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="c706f-179">licenseType</span></span>|[<span data-ttu-id="c706f-180">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="c706f-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="c706f-181">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c706f-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="c706f-182">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="c706f-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="c706f-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="c706f-183">targetEdition</span></span>|[<span data-ttu-id="c706f-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="c706f-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="c706f-185">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c706f-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="c706f-186">Os valores possíveis são `windows10Enterprise`: `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="c706f-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="c706f-187">license</span><span class="sxs-lookup"><span data-stu-id="c706f-187">license</span></span>|<span data-ttu-id="c706f-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c706f-188">String</span></span>|<span data-ttu-id="c706f-189">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c706f-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="c706f-190">productKey</span><span class="sxs-lookup"><span data-stu-id="c706f-190">productKey</span></span>|<span data-ttu-id="c706f-191">String</span><span class="sxs-lookup"><span data-stu-id="c706f-191">String</span></span>|<span data-ttu-id="c706f-192">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c706f-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="c706f-193">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="c706f-193">windowsSMode</span></span>|[<span data-ttu-id="c706f-194">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c706f-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="c706f-195">Configuração de modo S.</span><span class="sxs-lookup"><span data-stu-id="c706f-195">S mode configuration.</span></span> <span data-ttu-id="c706f-196">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="c706f-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="c706f-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="c706f-197">Response</span></span>
<span data-ttu-id="c706f-198">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c706f-198">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c706f-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c706f-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="c706f-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c706f-200">Request</span></span>
<span data-ttu-id="c706f-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c706f-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1204

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="c706f-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="c706f-202">Response</span></span>
<span data-ttu-id="c706f-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c706f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1376

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```





