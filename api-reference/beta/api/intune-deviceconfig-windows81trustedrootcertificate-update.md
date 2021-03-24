---
title: Atualizar windows81TrustedRootCertificate
description: Atualize as propriedades de um objeto windows81TrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3414bb0619f08d91c1ad3ab0dad5ef8dd485d821
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147200"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="b2820-103">Atualizar windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b2820-103">Update windows81TrustedRootCertificate</span></span>

<span data-ttu-id="b2820-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2820-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2820-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2820-107">Atualize as propriedades de um [objeto windows81TrustedRootCertificate.](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2820-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2820-108">Prerequisites</span></span>
<span data-ttu-id="b2820-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2820-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2820-111">Permission type</span></span>|<span data-ttu-id="b2820-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2820-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2820-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2820-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2820-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2820-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2820-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2820-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2820-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2820-116">Not supported.</span></span>|
|<span data-ttu-id="b2820-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2820-117">Application</span></span>|<span data-ttu-id="b2820-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2820-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2820-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2820-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b2820-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2820-120">Request headers</span></span>
|<span data-ttu-id="b2820-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2820-121">Header</span></span>|<span data-ttu-id="b2820-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2820-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2820-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2820-123">Authorization</span></span>|<span data-ttu-id="b2820-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2820-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2820-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2820-125">Accept</span></span>|<span data-ttu-id="b2820-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2820-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2820-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2820-127">Request body</span></span>
<span data-ttu-id="b2820-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windows81TrustedRootCertificate.](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="b2820-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b2820-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="b2820-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2820-130">Property</span></span>|<span data-ttu-id="b2820-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2820-131">Type</span></span>|<span data-ttu-id="b2820-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2820-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2820-133">id</span><span class="sxs-lookup"><span data-stu-id="b2820-133">id</span></span>|<span data-ttu-id="b2820-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2820-134">String</span></span>|<span data-ttu-id="b2820-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2820-135">Key of the entity.</span></span> <span data-ttu-id="b2820-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2820-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b2820-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2820-138">DateTimeOffset</span></span>|<span data-ttu-id="b2820-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b2820-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b2820-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2820-141">roleScopeTagIds</span></span>|<span data-ttu-id="b2820-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2820-142">String collection</span></span>|<span data-ttu-id="b2820-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="b2820-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b2820-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b2820-145">supportsScopeTags</span></span>|<span data-ttu-id="b2820-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="b2820-146">Boolean</span></span>|<span data-ttu-id="b2820-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b2820-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b2820-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b2820-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b2820-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b2820-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b2820-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2820-150">This property is read-only.</span></span> <span data-ttu-id="b2820-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b2820-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b2820-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b2820-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b2820-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b2820-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b2820-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2820-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b2820-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2820-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b2820-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b2820-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b2820-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b2820-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b2820-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b2820-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b2820-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b2820-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b2820-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2820-164">createdDateTime</span></span>|<span data-ttu-id="b2820-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2820-165">DateTimeOffset</span></span>|<span data-ttu-id="b2820-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b2820-166">DateTime the object was created.</span></span> <span data-ttu-id="b2820-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-168">descrição</span><span class="sxs-lookup"><span data-stu-id="b2820-168">description</span></span>|<span data-ttu-id="b2820-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2820-169">String</span></span>|<span data-ttu-id="b2820-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2820-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2820-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b2820-172">displayName</span></span>|<span data-ttu-id="b2820-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2820-173">String</span></span>|<span data-ttu-id="b2820-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2820-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2820-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-176">versão</span><span class="sxs-lookup"><span data-stu-id="b2820-176">version</span></span>|<span data-ttu-id="b2820-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b2820-177">Int32</span></span>|<span data-ttu-id="b2820-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2820-178">Version of the device configuration.</span></span> <span data-ttu-id="b2820-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2820-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2820-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b2820-180">trustedRootCertificate</span></span>|<span data-ttu-id="b2820-181">Binário</span><span class="sxs-lookup"><span data-stu-id="b2820-181">Binary</span></span>|<span data-ttu-id="b2820-182">Certificado Raiz Confiável</span><span class="sxs-lookup"><span data-stu-id="b2820-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="b2820-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="b2820-183">certFileName</span></span>|<span data-ttu-id="b2820-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2820-184">String</span></span>|<span data-ttu-id="b2820-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="b2820-185">File name to display in UI.</span></span>|
|<span data-ttu-id="b2820-186">destinationStore</span><span class="sxs-lookup"><span data-stu-id="b2820-186">destinationStore</span></span>|[<span data-ttu-id="b2820-187">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="b2820-187">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="b2820-188">Local do armazenamento de destino para o Certificado Raiz Confiável.</span><span class="sxs-lookup"><span data-stu-id="b2820-188">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="b2820-189">Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="b2820-189">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="b2820-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2820-190">Response</span></span>
<span data-ttu-id="b2820-191">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2820-191">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2820-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2820-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2820-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2820-193">Request</span></span>
<span data-ttu-id="b2820-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2820-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
Content-type: application/json
Content-length: 1198

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="b2820-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2820-195">Response</span></span>
<span data-ttu-id="b2820-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2820-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1370

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




