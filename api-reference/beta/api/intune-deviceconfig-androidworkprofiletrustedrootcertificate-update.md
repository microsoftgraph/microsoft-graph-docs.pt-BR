---
title: Atualizar androidWorkProfileTrustedRootCertificate
description: Atualiza as propriedades de um objeto androidWorkProfileTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c31ab20052be28b31bd4dd45e60cd747da4dd954
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206606"
---
# <a name="update-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="53b27-103">Atualizar androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="53b27-103">Update androidWorkProfileTrustedRootCertificate</span></span>

<span data-ttu-id="53b27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53b27-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53b27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53b27-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53b27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53b27-107">Atualiza as propriedades de um objeto [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="53b27-107">Update the properties of a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53b27-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53b27-108">Prerequisites</span></span>
<span data-ttu-id="53b27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b27-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53b27-111">Permission type</span></span>|<span data-ttu-id="53b27-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53b27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b27-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53b27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53b27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53b27-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53b27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b27-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53b27-116">Not supported.</span></span>|
|<span data-ttu-id="53b27-117">Application</span><span class="sxs-lookup"><span data-stu-id="53b27-117">Application</span></span>|<span data-ttu-id="53b27-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b27-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b27-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53b27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="53b27-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53b27-120">Request headers</span></span>
|<span data-ttu-id="53b27-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53b27-121">Header</span></span>|<span data-ttu-id="53b27-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53b27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53b27-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53b27-123">Authorization</span></span>|<span data-ttu-id="53b27-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53b27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53b27-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53b27-125">Accept</span></span>|<span data-ttu-id="53b27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53b27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b27-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53b27-127">Request body</span></span>
<span data-ttu-id="53b27-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="53b27-128">In the request body, supply a JSON representation for the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="53b27-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="53b27-129">The following table shows the properties that are required when you create the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span></span>

|<span data-ttu-id="53b27-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53b27-130">Property</span></span>|<span data-ttu-id="53b27-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53b27-131">Type</span></span>|<span data-ttu-id="53b27-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b27-133">id</span><span class="sxs-lookup"><span data-stu-id="53b27-133">id</span></span>|<span data-ttu-id="53b27-134">String</span><span class="sxs-lookup"><span data-stu-id="53b27-134">String</span></span>|<span data-ttu-id="53b27-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53b27-135">Key of the entity.</span></span> <span data-ttu-id="53b27-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53b27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="53b27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b27-138">DateTimeOffset</span></span>|<span data-ttu-id="53b27-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="53b27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="53b27-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53b27-141">roleScopeTagIds</span></span>|<span data-ttu-id="53b27-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b27-142">String collection</span></span>|<span data-ttu-id="53b27-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="53b27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="53b27-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="53b27-145">supportsScopeTags</span></span>|<span data-ttu-id="53b27-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="53b27-146">Boolean</span></span>|<span data-ttu-id="53b27-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="53b27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="53b27-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="53b27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="53b27-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="53b27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="53b27-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53b27-150">This property is read-only.</span></span> <span data-ttu-id="53b27-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="53b27-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="53b27-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="53b27-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="53b27-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="53b27-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="53b27-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="53b27-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="53b27-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="53b27-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="53b27-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="53b27-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="53b27-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="53b27-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="53b27-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="53b27-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="53b27-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="53b27-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="53b27-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53b27-164">createdDateTime</span></span>|<span data-ttu-id="53b27-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b27-165">DateTimeOffset</span></span>|<span data-ttu-id="53b27-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="53b27-166">DateTime the object was created.</span></span> <span data-ttu-id="53b27-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-168">description</span><span class="sxs-lookup"><span data-stu-id="53b27-168">description</span></span>|<span data-ttu-id="53b27-169">String</span><span class="sxs-lookup"><span data-stu-id="53b27-169">String</span></span>|<span data-ttu-id="53b27-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53b27-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53b27-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-172">displayName</span><span class="sxs-lookup"><span data-stu-id="53b27-172">displayName</span></span>|<span data-ttu-id="53b27-173">String</span><span class="sxs-lookup"><span data-stu-id="53b27-173">String</span></span>|<span data-ttu-id="53b27-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53b27-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53b27-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-176">versão</span><span class="sxs-lookup"><span data-stu-id="53b27-176">version</span></span>|<span data-ttu-id="53b27-177">Int32</span><span class="sxs-lookup"><span data-stu-id="53b27-177">Int32</span></span>|<span data-ttu-id="53b27-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53b27-178">Version of the device configuration.</span></span> <span data-ttu-id="53b27-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53b27-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53b27-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="53b27-180">trustedRootCertificate</span></span>|<span data-ttu-id="53b27-181">Binária</span><span class="sxs-lookup"><span data-stu-id="53b27-181">Binary</span></span>|<span data-ttu-id="53b27-182">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="53b27-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="53b27-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="53b27-183">certFileName</span></span>|<span data-ttu-id="53b27-184">String</span><span class="sxs-lookup"><span data-stu-id="53b27-184">String</span></span>|<span data-ttu-id="53b27-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="53b27-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="53b27-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b27-186">Response</span></span>
<span data-ttu-id="53b27-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53b27-187">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b27-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53b27-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="53b27-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53b27-189">Request</span></span>
<span data-ttu-id="53b27-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53b27-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="53b27-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b27-191">Response</span></span>
<span data-ttu-id="53b27-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53b27-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




