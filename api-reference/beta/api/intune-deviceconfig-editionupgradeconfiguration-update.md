---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd770b26558be797956b05296a54ba3b0fb8da03
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967325"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="47815-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="47815-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="47815-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47815-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47815-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47815-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47815-106">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47815-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47815-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47815-107">Prerequisites</span></span>
<span data-ttu-id="47815-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47815-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47815-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47815-110">Permission type</span></span>|<span data-ttu-id="47815-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47815-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47815-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47815-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47815-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47815-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47815-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47815-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47815-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47815-115">Not supported.</span></span>|
|<span data-ttu-id="47815-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47815-116">Application</span></span>|<span data-ttu-id="47815-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47815-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47815-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47815-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="47815-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47815-119">Request headers</span></span>
|<span data-ttu-id="47815-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47815-120">Header</span></span>|<span data-ttu-id="47815-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47815-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47815-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47815-122">Authorization</span></span>|<span data-ttu-id="47815-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47815-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47815-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47815-124">Accept</span></span>|<span data-ttu-id="47815-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47815-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47815-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47815-126">Request body</span></span>
<span data-ttu-id="47815-127">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47815-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="47815-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47815-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="47815-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47815-129">Property</span></span>|<span data-ttu-id="47815-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="47815-130">Type</span></span>|<span data-ttu-id="47815-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="47815-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47815-132">id</span><span class="sxs-lookup"><span data-stu-id="47815-132">id</span></span>|<span data-ttu-id="47815-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47815-133">String</span></span>|<span data-ttu-id="47815-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47815-134">Key of the entity.</span></span> <span data-ttu-id="47815-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47815-136">lastModifiedDateTime</span></span>|<span data-ttu-id="47815-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47815-137">DateTimeOffset</span></span>|<span data-ttu-id="47815-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="47815-138">DateTime the object was last modified.</span></span> <span data-ttu-id="47815-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47815-140">roleScopeTagIds</span></span>|<span data-ttu-id="47815-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="47815-141">String collection</span></span>|<span data-ttu-id="47815-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="47815-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47815-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47815-144">supportsScopeTags</span></span>|<span data-ttu-id="47815-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="47815-145">Boolean</span></span>|<span data-ttu-id="47815-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="47815-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47815-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="47815-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47815-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="47815-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47815-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47815-149">This property is read-only.</span></span> <span data-ttu-id="47815-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47815-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47815-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47815-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47815-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="47815-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47815-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47815-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47815-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47815-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47815-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="47815-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47815-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47815-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47815-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47815-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47815-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="47815-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47815-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47815-163">createdDateTime</span></span>|<span data-ttu-id="47815-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47815-164">DateTimeOffset</span></span>|<span data-ttu-id="47815-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="47815-165">DateTime the object was created.</span></span> <span data-ttu-id="47815-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-167">descrição</span><span class="sxs-lookup"><span data-stu-id="47815-167">description</span></span>|<span data-ttu-id="47815-168">String</span><span class="sxs-lookup"><span data-stu-id="47815-168">String</span></span>|<span data-ttu-id="47815-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47815-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47815-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-171">displayName</span><span class="sxs-lookup"><span data-stu-id="47815-171">displayName</span></span>|<span data-ttu-id="47815-172">String</span><span class="sxs-lookup"><span data-stu-id="47815-172">String</span></span>|<span data-ttu-id="47815-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47815-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47815-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-175">versão</span><span class="sxs-lookup"><span data-stu-id="47815-175">version</span></span>|<span data-ttu-id="47815-176">Int32</span><span class="sxs-lookup"><span data-stu-id="47815-176">Int32</span></span>|<span data-ttu-id="47815-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47815-177">Version of the device configuration.</span></span> <span data-ttu-id="47815-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47815-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47815-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="47815-179">licenseType</span></span>|[<span data-ttu-id="47815-180">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="47815-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="47815-181">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="47815-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="47815-182">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="47815-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="47815-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="47815-183">targetEdition</span></span>|[<span data-ttu-id="47815-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="47815-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="47815-185">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="47815-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="47815-186">Os valores possíveis são `windows10Enterprise`: `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN`,,, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore` ,,,,,,,, , `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="47815-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="47815-187">license</span><span class="sxs-lookup"><span data-stu-id="47815-187">license</span></span>|<span data-ttu-id="47815-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47815-188">String</span></span>|<span data-ttu-id="47815-189">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="47815-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="47815-190">productKey</span><span class="sxs-lookup"><span data-stu-id="47815-190">productKey</span></span>|<span data-ttu-id="47815-191">String</span><span class="sxs-lookup"><span data-stu-id="47815-191">String</span></span>|<span data-ttu-id="47815-192">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="47815-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="47815-193">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="47815-193">windowsSMode</span></span>|[<span data-ttu-id="47815-194">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="47815-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="47815-195">Configuração de modo S.</span><span class="sxs-lookup"><span data-stu-id="47815-195">S mode configuration.</span></span> <span data-ttu-id="47815-196">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="47815-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="47815-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="47815-197">Response</span></span>
<span data-ttu-id="47815-198">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47815-198">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47815-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47815-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="47815-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47815-200">Request</span></span>
<span data-ttu-id="47815-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47815-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47815-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="47815-202">Response</span></span>
<span data-ttu-id="47815-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47815-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





