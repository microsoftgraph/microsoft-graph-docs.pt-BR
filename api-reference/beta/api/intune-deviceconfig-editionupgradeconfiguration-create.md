---
title: Criar editionUpgradeConfiguration
description: Cria um novo objeto editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a45feaefd9a8540f8ed29b280d7ce234f9ccf0b0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168058"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="a1cac-103">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1cac-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="a1cac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1cac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1cac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1cac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1cac-106">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1cac-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1cac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1cac-107">Prerequisites</span></span>
<span data-ttu-id="a1cac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1cac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1cac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1cac-110">Permission type</span></span>|<span data-ttu-id="a1cac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1cac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1cac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1cac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1cac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1cac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1cac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1cac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1cac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1cac-115">Not supported.</span></span>|
|<span data-ttu-id="a1cac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1cac-116">Application</span></span>|<span data-ttu-id="a1cac-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1cac-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1cac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1cac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1cac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1cac-119">Request headers</span></span>
|<span data-ttu-id="a1cac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1cac-120">Header</span></span>|<span data-ttu-id="a1cac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1cac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1cac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1cac-122">Authorization</span></span>|<span data-ttu-id="a1cac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1cac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1cac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1cac-124">Accept</span></span>|<span data-ttu-id="a1cac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1cac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1cac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1cac-126">Request body</span></span>
<span data-ttu-id="a1cac-127">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1cac-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="a1cac-128">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1cac-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="a1cac-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1cac-129">Property</span></span>|<span data-ttu-id="a1cac-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1cac-130">Type</span></span>|<span data-ttu-id="a1cac-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1cac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1cac-132">id</span><span class="sxs-lookup"><span data-stu-id="a1cac-132">id</span></span>|<span data-ttu-id="a1cac-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1cac-133">String</span></span>|<span data-ttu-id="a1cac-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1cac-134">Key of the entity.</span></span> <span data-ttu-id="a1cac-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1cac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a1cac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1cac-137">DateTimeOffset</span></span>|<span data-ttu-id="a1cac-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a1cac-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a1cac-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1cac-140">roleScopeTagIds</span></span>|<span data-ttu-id="a1cac-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1cac-141">String collection</span></span>|<span data-ttu-id="a1cac-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a1cac-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1cac-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a1cac-144">supportsScopeTags</span></span>|<span data-ttu-id="a1cac-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1cac-145">Boolean</span></span>|<span data-ttu-id="a1cac-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a1cac-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a1cac-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a1cac-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a1cac-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a1cac-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a1cac-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1cac-149">This property is read-only.</span></span> <span data-ttu-id="a1cac-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1cac-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a1cac-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1cac-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a1cac-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a1cac-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a1cac-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1cac-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a1cac-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1cac-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a1cac-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a1cac-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a1cac-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1cac-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a1cac-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1cac-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a1cac-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a1cac-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a1cac-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1cac-163">createdDateTime</span></span>|<span data-ttu-id="a1cac-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1cac-164">DateTimeOffset</span></span>|<span data-ttu-id="a1cac-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a1cac-165">DateTime the object was created.</span></span> <span data-ttu-id="a1cac-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-167">descrição</span><span class="sxs-lookup"><span data-stu-id="a1cac-167">description</span></span>|<span data-ttu-id="a1cac-168">String</span><span class="sxs-lookup"><span data-stu-id="a1cac-168">String</span></span>|<span data-ttu-id="a1cac-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1cac-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1cac-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a1cac-171">displayName</span></span>|<span data-ttu-id="a1cac-172">String</span><span class="sxs-lookup"><span data-stu-id="a1cac-172">String</span></span>|<span data-ttu-id="a1cac-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1cac-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1cac-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-175">versão</span><span class="sxs-lookup"><span data-stu-id="a1cac-175">version</span></span>|<span data-ttu-id="a1cac-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a1cac-176">Int32</span></span>|<span data-ttu-id="a1cac-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1cac-177">Version of the device configuration.</span></span> <span data-ttu-id="a1cac-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1cac-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1cac-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="a1cac-179">licenseType</span></span>|[<span data-ttu-id="a1cac-180">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="a1cac-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="a1cac-181">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="a1cac-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="a1cac-182">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a1cac-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="a1cac-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="a1cac-183">targetEdition</span></span>|[<span data-ttu-id="a1cac-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="a1cac-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="a1cac-185">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="a1cac-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="a1cac-186">Os valores possíveis são `windows10Enterprise`: `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN`,,, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore` ,,,,,,,, , `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="a1cac-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="a1cac-187">license</span><span class="sxs-lookup"><span data-stu-id="a1cac-187">license</span></span>|<span data-ttu-id="a1cac-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1cac-188">String</span></span>|<span data-ttu-id="a1cac-189">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="a1cac-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="a1cac-190">productKey</span><span class="sxs-lookup"><span data-stu-id="a1cac-190">productKey</span></span>|<span data-ttu-id="a1cac-191">String</span><span class="sxs-lookup"><span data-stu-id="a1cac-191">String</span></span>|<span data-ttu-id="a1cac-192">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="a1cac-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="a1cac-193">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="a1cac-193">windowsSMode</span></span>|[<span data-ttu-id="a1cac-194">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1cac-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="a1cac-195">Configuração de modo S.</span><span class="sxs-lookup"><span data-stu-id="a1cac-195">S mode configuration.</span></span> <span data-ttu-id="a1cac-196">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="a1cac-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1cac-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1cac-197">Response</span></span>
<span data-ttu-id="a1cac-198">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1cac-198">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1cac-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1cac-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1cac-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1cac-200">Request</span></span>
<span data-ttu-id="a1cac-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1cac-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a1cac-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1cac-202">Response</span></span>
<span data-ttu-id="a1cac-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1cac-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




