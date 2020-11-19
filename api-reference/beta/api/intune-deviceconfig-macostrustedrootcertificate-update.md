---
title: Atualizar macOSTrustedRootCertificate
description: Atualiza as propriedades de um objeto macOSTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 378d24da1bc556ea23716887c2d8f274314b689e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271027"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="d25cf-103">Atualizar macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d25cf-103">Update macOSTrustedRootCertificate</span></span>

<span data-ttu-id="d25cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d25cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d25cf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d25cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d25cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d25cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d25cf-107">Atualiza as propriedades de um objeto [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d25cf-107">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d25cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d25cf-108">Prerequisites</span></span>
<span data-ttu-id="d25cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d25cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d25cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d25cf-111">Permission type</span></span>|<span data-ttu-id="d25cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d25cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d25cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d25cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d25cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d25cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d25cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d25cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d25cf-116">Not supported.</span></span>|
|<span data-ttu-id="d25cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d25cf-117">Application</span></span>|<span data-ttu-id="d25cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d25cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d25cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{macOSTrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="d25cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d25cf-120">Request headers</span></span>
|<span data-ttu-id="d25cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d25cf-121">Header</span></span>|<span data-ttu-id="d25cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d25cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d25cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d25cf-123">Authorization</span></span>|<span data-ttu-id="d25cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d25cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d25cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d25cf-125">Accept</span></span>|<span data-ttu-id="d25cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d25cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d25cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d25cf-127">Request body</span></span>
<span data-ttu-id="d25cf-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d25cf-128">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="d25cf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d25cf-129">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="d25cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d25cf-130">Property</span></span>|<span data-ttu-id="d25cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d25cf-131">Type</span></span>|<span data-ttu-id="d25cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d25cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d25cf-133">id</span><span class="sxs-lookup"><span data-stu-id="d25cf-133">id</span></span>|<span data-ttu-id="d25cf-134">String</span><span class="sxs-lookup"><span data-stu-id="d25cf-134">String</span></span>|<span data-ttu-id="d25cf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d25cf-135">Key of the entity.</span></span> <span data-ttu-id="d25cf-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d25cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d25cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d25cf-138">DateTimeOffset</span></span>|<span data-ttu-id="d25cf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d25cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d25cf-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d25cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="d25cf-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d25cf-142">String collection</span></span>|<span data-ttu-id="d25cf-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d25cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d25cf-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d25cf-145">supportsScopeTags</span></span>|<span data-ttu-id="d25cf-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d25cf-146">Boolean</span></span>|<span data-ttu-id="d25cf-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d25cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d25cf-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d25cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d25cf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d25cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d25cf-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d25cf-150">This property is read-only.</span></span> <span data-ttu-id="d25cf-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d25cf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d25cf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d25cf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d25cf-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d25cf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d25cf-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d25cf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d25cf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d25cf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d25cf-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d25cf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d25cf-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d25cf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d25cf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d25cf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d25cf-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d25cf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d25cf-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d25cf-164">createdDateTime</span></span>|<span data-ttu-id="d25cf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d25cf-165">DateTimeOffset</span></span>|<span data-ttu-id="d25cf-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d25cf-166">DateTime the object was created.</span></span> <span data-ttu-id="d25cf-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-168">description</span><span class="sxs-lookup"><span data-stu-id="d25cf-168">description</span></span>|<span data-ttu-id="d25cf-169">String</span><span class="sxs-lookup"><span data-stu-id="d25cf-169">String</span></span>|<span data-ttu-id="d25cf-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d25cf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d25cf-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d25cf-172">displayName</span></span>|<span data-ttu-id="d25cf-173">String</span><span class="sxs-lookup"><span data-stu-id="d25cf-173">String</span></span>|<span data-ttu-id="d25cf-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d25cf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d25cf-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-176">versão</span><span class="sxs-lookup"><span data-stu-id="d25cf-176">version</span></span>|<span data-ttu-id="d25cf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d25cf-177">Int32</span></span>|<span data-ttu-id="d25cf-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d25cf-178">Version of the device configuration.</span></span> <span data-ttu-id="d25cf-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d25cf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d25cf-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d25cf-180">trustedRootCertificate</span></span>|<span data-ttu-id="d25cf-181">Binária</span><span class="sxs-lookup"><span data-stu-id="d25cf-181">Binary</span></span>|<span data-ttu-id="d25cf-182">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="d25cf-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="d25cf-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="d25cf-183">certFileName</span></span>|<span data-ttu-id="d25cf-184">String</span><span class="sxs-lookup"><span data-stu-id="d25cf-184">String</span></span>|<span data-ttu-id="d25cf-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="d25cf-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d25cf-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25cf-186">Response</span></span>
<span data-ttu-id="d25cf-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d25cf-187">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d25cf-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d25cf-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="d25cf-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d25cf-189">Request</span></span>
<span data-ttu-id="d25cf-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d25cf-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
Content-type: application/json
Content-length: 1138

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="d25cf-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25cf-191">Response</span></span>
<span data-ttu-id="d25cf-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d25cf-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1310

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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




