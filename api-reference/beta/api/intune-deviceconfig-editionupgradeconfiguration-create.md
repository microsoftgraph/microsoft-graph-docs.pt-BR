---
title: Criar editionUpgradeConfiguration
description: Cria um novo objeto editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c854b0fe3384372ec8523ed02fe6462e5518694
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442961"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="539a7-103">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="539a7-103">Create editionUpgradeConfiguration</span></span>

<span data-ttu-id="539a7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="539a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="539a7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="539a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="539a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="539a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="539a7-107">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="539a7-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="539a7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="539a7-108">Prerequisites</span></span>
<span data-ttu-id="539a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="539a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="539a7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="539a7-111">Permission type</span></span>|<span data-ttu-id="539a7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="539a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="539a7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="539a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="539a7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539a7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="539a7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="539a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="539a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="539a7-116">Not supported.</span></span>|
|<span data-ttu-id="539a7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="539a7-117">Application</span></span>|<span data-ttu-id="539a7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539a7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="539a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="539a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="539a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="539a7-120">Request headers</span></span>
|<span data-ttu-id="539a7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="539a7-121">Header</span></span>|<span data-ttu-id="539a7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="539a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="539a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="539a7-123">Authorization</span></span>|<span data-ttu-id="539a7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="539a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="539a7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="539a7-125">Accept</span></span>|<span data-ttu-id="539a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="539a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="539a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="539a7-127">Request body</span></span>
<span data-ttu-id="539a7-128">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="539a7-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="539a7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="539a7-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="539a7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="539a7-130">Property</span></span>|<span data-ttu-id="539a7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="539a7-131">Type</span></span>|<span data-ttu-id="539a7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="539a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="539a7-133">id</span><span class="sxs-lookup"><span data-stu-id="539a7-133">id</span></span>|<span data-ttu-id="539a7-134">String</span><span class="sxs-lookup"><span data-stu-id="539a7-134">String</span></span>|<span data-ttu-id="539a7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="539a7-135">Key of the entity.</span></span> <span data-ttu-id="539a7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="539a7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="539a7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="539a7-138">DateTimeOffset</span></span>|<span data-ttu-id="539a7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="539a7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="539a7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="539a7-141">roleScopeTagIds</span></span>|<span data-ttu-id="539a7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="539a7-142">String collection</span></span>|<span data-ttu-id="539a7-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="539a7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="539a7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="539a7-145">supportsScopeTags</span></span>|<span data-ttu-id="539a7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="539a7-146">Boolean</span></span>|<span data-ttu-id="539a7-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="539a7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="539a7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="539a7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="539a7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="539a7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="539a7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="539a7-150">This property is read-only.</span></span> <span data-ttu-id="539a7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="539a7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="539a7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="539a7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="539a7-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="539a7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="539a7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="539a7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="539a7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="539a7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="539a7-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="539a7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="539a7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="539a7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="539a7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="539a7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="539a7-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="539a7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="539a7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="539a7-164">createdDateTime</span></span>|<span data-ttu-id="539a7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="539a7-165">DateTimeOffset</span></span>|<span data-ttu-id="539a7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="539a7-166">DateTime the object was created.</span></span> <span data-ttu-id="539a7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-168">description</span><span class="sxs-lookup"><span data-stu-id="539a7-168">description</span></span>|<span data-ttu-id="539a7-169">String</span><span class="sxs-lookup"><span data-stu-id="539a7-169">String</span></span>|<span data-ttu-id="539a7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="539a7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="539a7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="539a7-172">displayName</span></span>|<span data-ttu-id="539a7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="539a7-173">String</span></span>|<span data-ttu-id="539a7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="539a7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="539a7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-176">versão</span><span class="sxs-lookup"><span data-stu-id="539a7-176">version</span></span>|<span data-ttu-id="539a7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="539a7-177">Int32</span></span>|<span data-ttu-id="539a7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="539a7-178">Version of the device configuration.</span></span> <span data-ttu-id="539a7-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="539a7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="539a7-180">licenseType</span><span class="sxs-lookup"><span data-stu-id="539a7-180">licenseType</span></span>|[<span data-ttu-id="539a7-181">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="539a7-181">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="539a7-182">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="539a7-182">Edition Upgrade License Type.</span></span> <span data-ttu-id="539a7-183">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="539a7-183">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="539a7-184">targetEdition</span><span class="sxs-lookup"><span data-stu-id="539a7-184">targetEdition</span></span>|[<span data-ttu-id="539a7-185">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="539a7-185">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="539a7-186">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="539a7-186">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="539a7-187">Os valores possíveis são `windows10Enterprise`: `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="539a7-187">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="539a7-188">license</span><span class="sxs-lookup"><span data-stu-id="539a7-188">license</span></span>|<span data-ttu-id="539a7-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="539a7-189">String</span></span>|<span data-ttu-id="539a7-190">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="539a7-190">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="539a7-191">productKey</span><span class="sxs-lookup"><span data-stu-id="539a7-191">productKey</span></span>|<span data-ttu-id="539a7-192">String</span><span class="sxs-lookup"><span data-stu-id="539a7-192">String</span></span>|<span data-ttu-id="539a7-193">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="539a7-193">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="539a7-194">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="539a7-194">windowsSMode</span></span>|[<span data-ttu-id="539a7-195">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="539a7-195">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="539a7-196">Configuração de modo S.</span><span class="sxs-lookup"><span data-stu-id="539a7-196">S mode configuration.</span></span> <span data-ttu-id="539a7-197">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="539a7-197">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="539a7-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="539a7-198">Response</span></span>
<span data-ttu-id="539a7-199">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="539a7-199">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="539a7-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="539a7-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="539a7-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="539a7-201">Request</span></span>
<span data-ttu-id="539a7-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="539a7-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="539a7-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="539a7-203">Response</span></span>
<span data-ttu-id="539a7-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="539a7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





