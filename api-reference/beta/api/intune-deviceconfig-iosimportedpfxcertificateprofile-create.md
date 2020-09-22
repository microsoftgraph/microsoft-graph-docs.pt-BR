---
title: Criar iosImportedPFXCertificateProfile
description: Criar um novo objeto iosImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5683c59b5bc22f4312476218e26c1d34367d5a37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995209"
---
# <a name="create-iosimportedpfxcertificateprofile"></a><span data-ttu-id="2c0be-103">Criar iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2c0be-103">Create iosImportedPFXCertificateProfile</span></span>

<span data-ttu-id="2c0be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c0be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c0be-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c0be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c0be-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c0be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0be-107">Criar um novo objeto [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2c0be-107">Create a new [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c0be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c0be-108">Prerequisites</span></span>
<span data-ttu-id="2c0be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c0be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c0be-111">Permission type</span></span>|<span data-ttu-id="2c0be-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c0be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c0be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c0be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c0be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c0be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c0be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c0be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c0be-116">Not supported.</span></span>|
|<span data-ttu-id="2c0be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c0be-117">Application</span></span>|<span data-ttu-id="2c0be-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0be-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c0be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c0be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2c0be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c0be-120">Request headers</span></span>
|<span data-ttu-id="2c0be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c0be-121">Header</span></span>|<span data-ttu-id="2c0be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2c0be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c0be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c0be-123">Authorization</span></span>|<span data-ttu-id="2c0be-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c0be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c0be-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c0be-125">Accept</span></span>|<span data-ttu-id="2c0be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c0be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c0be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c0be-127">Request body</span></span>
<span data-ttu-id="2c0be-128">No corpo da solicitação, forneça uma representação JSON do objeto iosImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="2c0be-128">In the request body, supply a JSON representation for the iosImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="2c0be-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="2c0be-129">The following table shows the properties that are required when you create the iosImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="2c0be-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c0be-130">Property</span></span>|<span data-ttu-id="2c0be-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c0be-131">Type</span></span>|<span data-ttu-id="2c0be-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c0be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0be-133">id</span><span class="sxs-lookup"><span data-stu-id="2c0be-133">id</span></span>|<span data-ttu-id="2c0be-134">String</span><span class="sxs-lookup"><span data-stu-id="2c0be-134">String</span></span>|<span data-ttu-id="2c0be-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2c0be-135">Key of the entity.</span></span> <span data-ttu-id="2c0be-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c0be-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2c0be-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c0be-138">DateTimeOffset</span></span>|<span data-ttu-id="2c0be-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2c0be-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2c0be-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c0be-141">roleScopeTagIds</span></span>|<span data-ttu-id="2c0be-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c0be-142">String collection</span></span>|<span data-ttu-id="2c0be-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2c0be-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c0be-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2c0be-145">supportsScopeTags</span></span>|<span data-ttu-id="2c0be-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0be-146">Boolean</span></span>|<span data-ttu-id="2c0be-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2c0be-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2c0be-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2c0be-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2c0be-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2c0be-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2c0be-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c0be-150">This property is read-only.</span></span> <span data-ttu-id="2c0be-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c0be-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2c0be-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c0be-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2c0be-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="2c0be-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2c0be-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c0be-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2c0be-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c0be-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2c0be-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="2c0be-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2c0be-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c0be-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2c0be-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c0be-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2c0be-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="2c0be-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2c0be-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c0be-164">createdDateTime</span></span>|<span data-ttu-id="2c0be-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c0be-165">DateTimeOffset</span></span>|<span data-ttu-id="2c0be-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2c0be-166">DateTime the object was created.</span></span> <span data-ttu-id="2c0be-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-168">description</span><span class="sxs-lookup"><span data-stu-id="2c0be-168">description</span></span>|<span data-ttu-id="2c0be-169">String</span><span class="sxs-lookup"><span data-stu-id="2c0be-169">String</span></span>|<span data-ttu-id="2c0be-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c0be-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c0be-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2c0be-172">displayName</span></span>|<span data-ttu-id="2c0be-173">String</span><span class="sxs-lookup"><span data-stu-id="2c0be-173">String</span></span>|<span data-ttu-id="2c0be-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c0be-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c0be-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-176">versão</span><span class="sxs-lookup"><span data-stu-id="2c0be-176">version</span></span>|<span data-ttu-id="2c0be-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0be-177">Int32</span></span>|<span data-ttu-id="2c0be-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c0be-178">Version of the device configuration.</span></span> <span data-ttu-id="2c0be-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c0be-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0be-180">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="2c0be-180">intendedPurpose</span></span>|[<span data-ttu-id="2c0be-181">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="2c0be-181">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="2c0be-182">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são: `unassigned` , `smimeEncryption` , `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="2c0be-182">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="2c0be-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c0be-183">Response</span></span>
<span data-ttu-id="2c0be-184">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c0be-184">If successful, this method returns a `201 Created` response code and a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c0be-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c0be-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c0be-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c0be-186">Request</span></span>
<span data-ttu-id="2c0be-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c0be-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1076

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="2c0be-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c0be-188">Response</span></span>
<span data-ttu-id="2c0be-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c0be-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1248

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
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
  "intendedPurpose": "smimeEncryption"
}
```






