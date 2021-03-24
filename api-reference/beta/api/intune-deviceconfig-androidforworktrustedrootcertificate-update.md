---
title: Atualizar androidForWorkTrustedRootCertificate
description: Atualize as propriedades de um objeto androidForWorkTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9403e51fdaa2ea7cb2ee7915c1e16cffe028d0ae
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138236"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="0f857-103">Atualizar androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0f857-103">Update androidForWorkTrustedRootCertificate</span></span>

<span data-ttu-id="0f857-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f857-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f857-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f857-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f857-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f857-107">Atualize as propriedades de [um objeto androidForWorkTrustedRootCertificate.](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-107">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f857-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f857-108">Prerequisites</span></span>
<span data-ttu-id="0f857-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f857-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f857-111">Permission type</span></span>|<span data-ttu-id="0f857-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f857-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f857-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f857-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f857-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f857-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f857-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f857-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f857-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f857-116">Not supported.</span></span>|
|<span data-ttu-id="0f857-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f857-117">Application</span></span>|<span data-ttu-id="0f857-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f857-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f857-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f857-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="0f857-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f857-120">Request headers</span></span>
|<span data-ttu-id="0f857-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f857-121">Header</span></span>|<span data-ttu-id="0f857-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f857-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f857-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f857-123">Authorization</span></span>|<span data-ttu-id="0f857-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f857-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f857-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f857-125">Accept</span></span>|<span data-ttu-id="0f857-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f857-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f857-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f857-127">Request body</span></span>
<span data-ttu-id="0f857-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidForWorkTrustedRootCertificate.](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-128">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="0f857-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0f857-129">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="0f857-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f857-130">Property</span></span>|<span data-ttu-id="0f857-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f857-131">Type</span></span>|<span data-ttu-id="0f857-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f857-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f857-133">id</span><span class="sxs-lookup"><span data-stu-id="0f857-133">id</span></span>|<span data-ttu-id="0f857-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f857-134">String</span></span>|<span data-ttu-id="0f857-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f857-135">Key of the entity.</span></span> <span data-ttu-id="0f857-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f857-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0f857-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f857-138">DateTimeOffset</span></span>|<span data-ttu-id="0f857-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0f857-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0f857-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f857-141">roleScopeTagIds</span></span>|<span data-ttu-id="0f857-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f857-142">String collection</span></span>|<span data-ttu-id="0f857-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="0f857-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f857-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0f857-145">supportsScopeTags</span></span>|<span data-ttu-id="0f857-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="0f857-146">Boolean</span></span>|<span data-ttu-id="0f857-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0f857-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0f857-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0f857-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0f857-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0f857-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0f857-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f857-150">This property is read-only.</span></span> <span data-ttu-id="0f857-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f857-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0f857-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f857-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0f857-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0f857-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0f857-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f857-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0f857-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f857-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0f857-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0f857-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0f857-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f857-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0f857-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f857-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0f857-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0f857-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0f857-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f857-164">createdDateTime</span></span>|<span data-ttu-id="0f857-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f857-165">DateTimeOffset</span></span>|<span data-ttu-id="0f857-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0f857-166">DateTime the object was created.</span></span> <span data-ttu-id="0f857-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-168">descrição</span><span class="sxs-lookup"><span data-stu-id="0f857-168">description</span></span>|<span data-ttu-id="0f857-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f857-169">String</span></span>|<span data-ttu-id="0f857-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f857-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f857-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0f857-172">displayName</span></span>|<span data-ttu-id="0f857-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f857-173">String</span></span>|<span data-ttu-id="0f857-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f857-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f857-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-176">versão</span><span class="sxs-lookup"><span data-stu-id="0f857-176">version</span></span>|<span data-ttu-id="0f857-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0f857-177">Int32</span></span>|<span data-ttu-id="0f857-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f857-178">Version of the device configuration.</span></span> <span data-ttu-id="0f857-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f857-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f857-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0f857-180">trustedRootCertificate</span></span>|<span data-ttu-id="0f857-181">Binário</span><span class="sxs-lookup"><span data-stu-id="0f857-181">Binary</span></span>|<span data-ttu-id="0f857-182">Certificado Raiz Confiável</span><span class="sxs-lookup"><span data-stu-id="0f857-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="0f857-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="0f857-183">certFileName</span></span>|<span data-ttu-id="0f857-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f857-184">String</span></span>|<span data-ttu-id="0f857-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f857-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="0f857-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f857-186">Response</span></span>
<span data-ttu-id="0f857-187">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f857-187">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f857-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f857-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f857-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f857-189">Request</span></span>
<span data-ttu-id="0f857-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f857-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f857-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f857-191">Response</span></span>
<span data-ttu-id="0f857-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f857-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




