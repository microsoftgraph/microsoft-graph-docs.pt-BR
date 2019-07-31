---
title: Atualizar androidForWorkTrustedRootCertificate
description: Atualiza as propriedades de um objeto androidForWorkTrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a4919b068b7eadda304463b80d730114f0d49da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963133"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="ac209-103">Atualizar androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ac209-103">Update androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="ac209-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac209-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac209-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac209-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac209-106">Atualiza as propriedades de um objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ac209-106">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac209-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac209-107">Prerequisites</span></span>
<span data-ttu-id="ac209-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac209-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac209-110">Permission type</span></span>|<span data-ttu-id="ac209-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac209-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac209-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac209-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac209-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac209-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac209-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac209-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac209-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac209-115">Not supported.</span></span>|
|<span data-ttu-id="ac209-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac209-116">Application</span></span>|<span data-ttu-id="ac209-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac209-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac209-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac209-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="ac209-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac209-119">Request headers</span></span>
|<span data-ttu-id="ac209-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac209-120">Header</span></span>|<span data-ttu-id="ac209-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ac209-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac209-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac209-122">Authorization</span></span>|<span data-ttu-id="ac209-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac209-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac209-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac209-124">Accept</span></span>|<span data-ttu-id="ac209-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac209-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac209-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac209-126">Request body</span></span>
<span data-ttu-id="ac209-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ac209-127">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="ac209-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ac209-128">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="ac209-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac209-129">Property</span></span>|<span data-ttu-id="ac209-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac209-130">Type</span></span>|<span data-ttu-id="ac209-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac209-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac209-132">id</span><span class="sxs-lookup"><span data-stu-id="ac209-132">id</span></span>|<span data-ttu-id="ac209-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac209-133">String</span></span>|<span data-ttu-id="ac209-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ac209-134">Key of the entity.</span></span> <span data-ttu-id="ac209-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac209-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ac209-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac209-137">DateTimeOffset</span></span>|<span data-ttu-id="ac209-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ac209-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ac209-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac209-140">roleScopeTagIds</span></span>|<span data-ttu-id="ac209-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac209-141">String collection</span></span>|<span data-ttu-id="ac209-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ac209-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ac209-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ac209-144">supportsScopeTags</span></span>|<span data-ttu-id="ac209-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac209-145">Boolean</span></span>|<span data-ttu-id="ac209-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ac209-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ac209-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ac209-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ac209-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ac209-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ac209-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac209-149">This property is read-only.</span></span> <span data-ttu-id="ac209-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac209-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ac209-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac209-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ac209-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ac209-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ac209-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac209-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ac209-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac209-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ac209-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ac209-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ac209-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac209-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ac209-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac209-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ac209-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ac209-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ac209-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac209-163">createdDateTime</span></span>|<span data-ttu-id="ac209-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac209-164">DateTimeOffset</span></span>|<span data-ttu-id="ac209-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ac209-165">DateTime the object was created.</span></span> <span data-ttu-id="ac209-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-167">descrição</span><span class="sxs-lookup"><span data-stu-id="ac209-167">description</span></span>|<span data-ttu-id="ac209-168">String</span><span class="sxs-lookup"><span data-stu-id="ac209-168">String</span></span>|<span data-ttu-id="ac209-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac209-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ac209-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ac209-171">displayName</span></span>|<span data-ttu-id="ac209-172">String</span><span class="sxs-lookup"><span data-stu-id="ac209-172">String</span></span>|<span data-ttu-id="ac209-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac209-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ac209-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-175">versão</span><span class="sxs-lookup"><span data-stu-id="ac209-175">version</span></span>|<span data-ttu-id="ac209-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ac209-176">Int32</span></span>|<span data-ttu-id="ac209-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac209-177">Version of the device configuration.</span></span> <span data-ttu-id="ac209-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac209-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac209-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ac209-179">trustedRootCertificate</span></span>|<span data-ttu-id="ac209-180">Binária</span><span class="sxs-lookup"><span data-stu-id="ac209-180">Binary</span></span>|<span data-ttu-id="ac209-181">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="ac209-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="ac209-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="ac209-182">certFileName</span></span>|<span data-ttu-id="ac209-183">String</span><span class="sxs-lookup"><span data-stu-id="ac209-183">String</span></span>|<span data-ttu-id="ac209-184">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac209-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="ac209-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac209-185">Response</span></span>
<span data-ttu-id="ac209-186">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac209-186">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac209-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac209-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac209-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac209-188">Request</span></span>
<span data-ttu-id="ac209-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac209-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="ac209-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac209-190">Response</span></span>
<span data-ttu-id="ac209-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac209-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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





