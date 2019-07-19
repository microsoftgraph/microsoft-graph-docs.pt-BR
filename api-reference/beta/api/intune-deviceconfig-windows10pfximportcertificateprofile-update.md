---
title: Atualizar windows10PFXImportCertificateProfile
description: Atualiza as propriedades de um objeto windows10PFXImportCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ed0308eb76b92bbe60e576f9615e3401c90ea67
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962488"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="f9e74-103">Atualizar windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f9e74-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="f9e74-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9e74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9e74-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9e74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9e74-106">Atualiza as propriedades de um objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f9e74-106">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9e74-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9e74-107">Prerequisites</span></span>
<span data-ttu-id="f9e74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9e74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9e74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9e74-110">Permission type</span></span>|<span data-ttu-id="f9e74-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9e74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9e74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9e74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9e74-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9e74-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9e74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9e74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9e74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9e74-115">Not supported.</span></span>|
|<span data-ttu-id="f9e74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9e74-116">Application</span></span>|<span data-ttu-id="f9e74-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9e74-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9e74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9e74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f9e74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e74-119">Request headers</span></span>
|<span data-ttu-id="f9e74-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9e74-120">Header</span></span>|<span data-ttu-id="f9e74-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9e74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9e74-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9e74-122">Authorization</span></span>|<span data-ttu-id="f9e74-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9e74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9e74-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9e74-124">Accept</span></span>|<span data-ttu-id="f9e74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9e74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9e74-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e74-126">Request body</span></span>
<span data-ttu-id="f9e74-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f9e74-127">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="f9e74-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f9e74-128">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="f9e74-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9e74-129">Property</span></span>|<span data-ttu-id="f9e74-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9e74-130">Type</span></span>|<span data-ttu-id="f9e74-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e74-132">id</span><span class="sxs-lookup"><span data-stu-id="f9e74-132">id</span></span>|<span data-ttu-id="f9e74-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9e74-133">String</span></span>|<span data-ttu-id="f9e74-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9e74-134">Key of the entity.</span></span> <span data-ttu-id="f9e74-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e74-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f9e74-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e74-137">DateTimeOffset</span></span>|<span data-ttu-id="f9e74-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9e74-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f9e74-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9e74-140">roleScopeTagIds</span></span>|<span data-ttu-id="f9e74-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9e74-141">String collection</span></span>|<span data-ttu-id="f9e74-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f9e74-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9e74-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9e74-144">supportsScopeTags</span></span>|<span data-ttu-id="f9e74-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9e74-145">Boolean</span></span>|<span data-ttu-id="f9e74-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f9e74-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9e74-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f9e74-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9e74-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f9e74-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9e74-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9e74-149">This property is read-only.</span></span> <span data-ttu-id="f9e74-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f9e74-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f9e74-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f9e74-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f9e74-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f9e74-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f9e74-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f9e74-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f9e74-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f9e74-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f9e74-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f9e74-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f9e74-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f9e74-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f9e74-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f9e74-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f9e74-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f9e74-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f9e74-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e74-163">createdDateTime</span></span>|<span data-ttu-id="f9e74-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e74-164">DateTimeOffset</span></span>|<span data-ttu-id="f9e74-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9e74-165">DateTime the object was created.</span></span> <span data-ttu-id="f9e74-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-167">descrição</span><span class="sxs-lookup"><span data-stu-id="f9e74-167">description</span></span>|<span data-ttu-id="f9e74-168">String</span><span class="sxs-lookup"><span data-stu-id="f9e74-168">String</span></span>|<span data-ttu-id="f9e74-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9e74-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9e74-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f9e74-171">displayName</span></span>|<span data-ttu-id="f9e74-172">String</span><span class="sxs-lookup"><span data-stu-id="f9e74-172">String</span></span>|<span data-ttu-id="f9e74-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9e74-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9e74-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-175">versão</span><span class="sxs-lookup"><span data-stu-id="f9e74-175">version</span></span>|<span data-ttu-id="f9e74-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f9e74-176">Int32</span></span>|<span data-ttu-id="f9e74-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9e74-177">Version of the device configuration.</span></span> <span data-ttu-id="f9e74-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9e74-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9e74-179">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f9e74-179">keyStorageProvider</span></span>|[<span data-ttu-id="f9e74-180">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f9e74-180">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f9e74-181">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="f9e74-181">Not yet documented.</span></span> <span data-ttu-id="f9e74-182">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="f9e74-182">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="f9e74-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9e74-183">Response</span></span>
<span data-ttu-id="f9e74-184">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9e74-184">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9e74-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9e74-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9e74-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e74-186">Request</span></span>
<span data-ttu-id="f9e74-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9e74-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1090

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="f9e74-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9e74-188">Response</span></span>
<span data-ttu-id="f9e74-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9e74-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1262

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





