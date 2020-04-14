---
title: Criar windows10PFXImportCertificateProfile
description: Criar um novo objeto windows10PFXImportCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ed8a051dd84a94597387ac88e101a80fb287428
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43339644"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="ff1d5-103">Criar windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ff1d5-103">Create windows10PFXImportCertificateProfile</span></span>

<span data-ttu-id="ff1d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff1d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff1d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff1d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff1d5-107">Criar um novo objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ff1d5-107">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff1d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff1d5-108">Prerequisites</span></span>
<span data-ttu-id="ff1d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff1d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff1d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff1d5-111">Permission type</span></span>|<span data-ttu-id="ff1d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff1d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff1d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff1d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff1d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff1d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-116">Not supported.</span></span>|
|<span data-ttu-id="ff1d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff1d5-117">Application</span></span>|<span data-ttu-id="ff1d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff1d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff1d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff1d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ff1d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff1d5-120">Request headers</span></span>
|<span data-ttu-id="ff1d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff1d5-121">Header</span></span>|<span data-ttu-id="ff1d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff1d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff1d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff1d5-123">Authorization</span></span>|<span data-ttu-id="ff1d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff1d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff1d5-125">Accept</span></span>|<span data-ttu-id="ff1d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff1d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff1d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff1d5-127">Request body</span></span>
<span data-ttu-id="ff1d5-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-128">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="ff1d5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-129">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="ff1d5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff1d5-130">Property</span></span>|<span data-ttu-id="ff1d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff1d5-131">Type</span></span>|<span data-ttu-id="ff1d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff1d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff1d5-133">id</span><span class="sxs-lookup"><span data-stu-id="ff1d5-133">id</span></span>|<span data-ttu-id="ff1d5-134">String</span><span class="sxs-lookup"><span data-stu-id="ff1d5-134">String</span></span>|<span data-ttu-id="ff1d5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-135">Key of the entity.</span></span> <span data-ttu-id="ff1d5-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff1d5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ff1d5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff1d5-138">DateTimeOffset</span></span>|<span data-ttu-id="ff1d5-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ff1d5-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff1d5-141">roleScopeTagIds</span></span>|<span data-ttu-id="ff1d5-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ff1d5-142">String collection</span></span>|<span data-ttu-id="ff1d5-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ff1d5-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ff1d5-145">supportsScopeTags</span></span>|<span data-ttu-id="ff1d5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff1d5-146">Boolean</span></span>|<span data-ttu-id="ff1d5-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ff1d5-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ff1d5-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ff1d5-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-150">This property is read-only.</span></span> <span data-ttu-id="ff1d5-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff1d5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ff1d5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff1d5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ff1d5-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ff1d5-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff1d5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ff1d5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff1d5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ff1d5-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ff1d5-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff1d5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ff1d5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff1d5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ff1d5-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ff1d5-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff1d5-164">createdDateTime</span></span>|<span data-ttu-id="ff1d5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff1d5-165">DateTimeOffset</span></span>|<span data-ttu-id="ff1d5-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-166">DateTime the object was created.</span></span> <span data-ttu-id="ff1d5-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-168">description</span><span class="sxs-lookup"><span data-stu-id="ff1d5-168">description</span></span>|<span data-ttu-id="ff1d5-169">String</span><span class="sxs-lookup"><span data-stu-id="ff1d5-169">String</span></span>|<span data-ttu-id="ff1d5-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff1d5-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ff1d5-172">displayName</span></span>|<span data-ttu-id="ff1d5-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff1d5-173">String</span></span>|<span data-ttu-id="ff1d5-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff1d5-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-176">versão</span><span class="sxs-lookup"><span data-stu-id="ff1d5-176">version</span></span>|<span data-ttu-id="ff1d5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ff1d5-177">Int32</span></span>|<span data-ttu-id="ff1d5-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-178">Version of the device configuration.</span></span> <span data-ttu-id="ff1d5-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff1d5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff1d5-180">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ff1d5-180">keyStorageProvider</span></span>|[<span data-ttu-id="ff1d5-181">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ff1d5-181">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ff1d5-182">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-182">Not yet documented.</span></span> <span data-ttu-id="ff1d5-183">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-183">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="ff1d5-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff1d5-184">Response</span></span>
<span data-ttu-id="ff1d5-185">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-185">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff1d5-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff1d5-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff1d5-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff1d5-187">Request</span></span>
<span data-ttu-id="ff1d5-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ff1d5-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff1d5-189">Response</span></span>
<span data-ttu-id="ff1d5-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff1d5-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



