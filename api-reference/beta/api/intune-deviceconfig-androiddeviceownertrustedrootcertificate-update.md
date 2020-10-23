---
title: Atualizar androidDeviceOwnerTrustedRootCertificate
description: Atualiza as propriedades de um objeto androidDeviceOwnerTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04b84fe63a787caaa2fb98def2d57732e4e9da9c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727199"
---
# <a name="update-androiddeviceownertrustedrootcertificate"></a><span data-ttu-id="7207b-103">Atualizar androidDeviceOwnerTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7207b-103">Update androidDeviceOwnerTrustedRootCertificate</span></span>

<span data-ttu-id="7207b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7207b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7207b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7207b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7207b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7207b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7207b-107">Atualiza as propriedades de um objeto [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="7207b-107">Update the properties of a [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7207b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7207b-108">Prerequisites</span></span>
<span data-ttu-id="7207b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7207b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7207b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7207b-111">Permission type</span></span>|<span data-ttu-id="7207b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7207b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7207b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7207b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7207b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7207b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7207b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7207b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7207b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7207b-116">Not supported.</span></span>|
|<span data-ttu-id="7207b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7207b-117">Application</span></span>|<span data-ttu-id="7207b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7207b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7207b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7207b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="7207b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7207b-120">Request headers</span></span>
|<span data-ttu-id="7207b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7207b-121">Header</span></span>|<span data-ttu-id="7207b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7207b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7207b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7207b-123">Authorization</span></span>|<span data-ttu-id="7207b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7207b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7207b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7207b-125">Accept</span></span>|<span data-ttu-id="7207b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7207b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7207b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7207b-127">Request body</span></span>
<span data-ttu-id="7207b-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="7207b-128">In the request body, supply a JSON representation for the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="7207b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7207b-129">The following table shows the properties that are required when you create the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span></span>

|<span data-ttu-id="7207b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7207b-130">Property</span></span>|<span data-ttu-id="7207b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7207b-131">Type</span></span>|<span data-ttu-id="7207b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7207b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7207b-133">id</span><span class="sxs-lookup"><span data-stu-id="7207b-133">id</span></span>|<span data-ttu-id="7207b-134">String</span><span class="sxs-lookup"><span data-stu-id="7207b-134">String</span></span>|<span data-ttu-id="7207b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7207b-135">Key of the entity.</span></span> <span data-ttu-id="7207b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7207b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7207b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7207b-138">DateTimeOffset</span></span>|<span data-ttu-id="7207b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7207b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7207b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7207b-141">roleScopeTagIds</span></span>|<span data-ttu-id="7207b-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7207b-142">String collection</span></span>|<span data-ttu-id="7207b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7207b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7207b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7207b-145">supportsScopeTags</span></span>|<span data-ttu-id="7207b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="7207b-146">Boolean</span></span>|<span data-ttu-id="7207b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7207b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7207b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7207b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7207b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7207b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7207b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7207b-150">This property is read-only.</span></span> <span data-ttu-id="7207b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7207b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7207b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7207b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7207b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="7207b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7207b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7207b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7207b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7207b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7207b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="7207b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7207b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7207b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7207b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7207b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7207b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="7207b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7207b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7207b-164">createdDateTime</span></span>|<span data-ttu-id="7207b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7207b-165">DateTimeOffset</span></span>|<span data-ttu-id="7207b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7207b-166">DateTime the object was created.</span></span> <span data-ttu-id="7207b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-168">description</span><span class="sxs-lookup"><span data-stu-id="7207b-168">description</span></span>|<span data-ttu-id="7207b-169">String</span><span class="sxs-lookup"><span data-stu-id="7207b-169">String</span></span>|<span data-ttu-id="7207b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7207b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7207b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7207b-172">displayName</span></span>|<span data-ttu-id="7207b-173">String</span><span class="sxs-lookup"><span data-stu-id="7207b-173">String</span></span>|<span data-ttu-id="7207b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7207b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7207b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-176">versão</span><span class="sxs-lookup"><span data-stu-id="7207b-176">version</span></span>|<span data-ttu-id="7207b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7207b-177">Int32</span></span>|<span data-ttu-id="7207b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7207b-178">Version of the device configuration.</span></span> <span data-ttu-id="7207b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7207b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7207b-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7207b-180">trustedRootCertificate</span></span>|<span data-ttu-id="7207b-181">Binária</span><span class="sxs-lookup"><span data-stu-id="7207b-181">Binary</span></span>|<span data-ttu-id="7207b-182">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="7207b-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="7207b-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="7207b-183">certFileName</span></span>|<span data-ttu-id="7207b-184">String</span><span class="sxs-lookup"><span data-stu-id="7207b-184">String</span></span>|<span data-ttu-id="7207b-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7207b-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="7207b-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="7207b-186">Response</span></span>
<span data-ttu-id="7207b-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7207b-187">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7207b-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7207b-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="7207b-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7207b-189">Request</span></span>
<span data-ttu-id="7207b-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7207b-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="7207b-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="7207b-191">Response</span></span>
<span data-ttu-id="7207b-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7207b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
  "id": "6efc1a55-1a55-6efc-551a-fc6e551afc6e",
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





