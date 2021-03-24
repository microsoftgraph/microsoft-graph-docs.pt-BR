---
title: Atualizar iosImportedPFXCertificateProfile
description: Atualize as propriedades de um objeto iosImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ecf3b6132b69147559b53d4969165e28e008adfe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131502"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="ce363-103">Atualizar iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ce363-103">Update iosImportedPFXCertificateProfile</span></span>

<span data-ttu-id="ce363-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce363-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce363-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce363-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce363-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce363-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce363-107">Atualize as propriedades de [um objeto iosImportedPFXCertificateProfile.](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-107">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce363-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce363-108">Prerequisites</span></span>
<span data-ttu-id="ce363-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce363-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce363-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce363-111">Permission type</span></span>|<span data-ttu-id="ce363-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce363-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce363-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce363-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce363-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce363-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce363-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce363-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce363-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce363-116">Not supported.</span></span>|
|<span data-ttu-id="ce363-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce363-117">Application</span></span>|<span data-ttu-id="ce363-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce363-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce363-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce363-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce363-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce363-120">Request headers</span></span>
|<span data-ttu-id="ce363-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce363-121">Header</span></span>|<span data-ttu-id="ce363-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ce363-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce363-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce363-123">Authorization</span></span>|<span data-ttu-id="ce363-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce363-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce363-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce363-125">Accept</span></span>|<span data-ttu-id="ce363-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce363-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce363-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce363-127">Request body</span></span>
<span data-ttu-id="ce363-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosImportedPFXCertificateProfile.](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-128">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="ce363-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ce363-129">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="ce363-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce363-130">Property</span></span>|<span data-ttu-id="ce363-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce363-131">Type</span></span>|<span data-ttu-id="ce363-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce363-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce363-133">id</span><span class="sxs-lookup"><span data-stu-id="ce363-133">id</span></span>|<span data-ttu-id="ce363-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce363-134">String</span></span>|<span data-ttu-id="ce363-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce363-135">Key of the entity.</span></span> <span data-ttu-id="ce363-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce363-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ce363-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce363-138">DateTimeOffset</span></span>|<span data-ttu-id="ce363-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ce363-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ce363-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce363-141">roleScopeTagIds</span></span>|<span data-ttu-id="ce363-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce363-142">String collection</span></span>|<span data-ttu-id="ce363-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ce363-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce363-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce363-145">supportsScopeTags</span></span>|<span data-ttu-id="ce363-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce363-146">Boolean</span></span>|<span data-ttu-id="ce363-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ce363-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce363-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ce363-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce363-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ce363-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce363-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce363-150">This property is read-only.</span></span> <span data-ttu-id="ce363-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce363-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ce363-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce363-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ce363-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ce363-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ce363-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce363-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ce363-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce363-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ce363-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ce363-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ce363-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce363-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ce363-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce363-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ce363-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ce363-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ce363-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce363-164">createdDateTime</span></span>|<span data-ttu-id="ce363-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce363-165">DateTimeOffset</span></span>|<span data-ttu-id="ce363-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ce363-166">DateTime the object was created.</span></span> <span data-ttu-id="ce363-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-168">descrição</span><span class="sxs-lookup"><span data-stu-id="ce363-168">description</span></span>|<span data-ttu-id="ce363-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce363-169">String</span></span>|<span data-ttu-id="ce363-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce363-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce363-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ce363-172">displayName</span></span>|<span data-ttu-id="ce363-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce363-173">String</span></span>|<span data-ttu-id="ce363-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce363-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce363-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-176">versão</span><span class="sxs-lookup"><span data-stu-id="ce363-176">version</span></span>|<span data-ttu-id="ce363-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ce363-177">Int32</span></span>|<span data-ttu-id="ce363-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce363-178">Version of the device configuration.</span></span> <span data-ttu-id="ce363-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce363-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce363-180">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ce363-180">intendedPurpose</span></span>|[<span data-ttu-id="ce363-181">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ce363-181">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="ce363-182">Finalidade pretendido do Perfil de Certificado - que pode ser Unassigned, SmimeEncryption, SmimeSigning etc. Os valores possíveis são: `unassigned` , , , , `smimeEncryption` `smimeSigning` `vpn` `wifi` .</span><span class="sxs-lookup"><span data-stu-id="ce363-182">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="ce363-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce363-183">Response</span></span>
<span data-ttu-id="ce363-184">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce363-184">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce363-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce363-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce363-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce363-186">Request</span></span>
<span data-ttu-id="ce363-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce363-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ce363-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce363-188">Response</span></span>
<span data-ttu-id="ce363-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce363-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




