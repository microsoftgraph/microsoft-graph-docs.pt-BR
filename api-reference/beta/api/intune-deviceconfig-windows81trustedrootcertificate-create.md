---
title: Criar windows81TrustedRootCertificate
description: Criar um novo objeto windows81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8c975efdc65ffaff3dd048b871449b531930274
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962187"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="da56d-103">Criar windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="da56d-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="da56d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da56d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da56d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da56d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da56d-106">Criar um novo objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="da56d-106">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da56d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da56d-107">Prerequisites</span></span>
<span data-ttu-id="da56d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da56d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da56d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da56d-110">Permission type</span></span>|<span data-ttu-id="da56d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da56d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da56d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da56d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da56d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da56d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da56d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da56d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da56d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da56d-115">Not supported.</span></span>|
|<span data-ttu-id="da56d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da56d-116">Application</span></span>|<span data-ttu-id="da56d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da56d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da56d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da56d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="da56d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da56d-119">Request headers</span></span>
|<span data-ttu-id="da56d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da56d-120">Header</span></span>|<span data-ttu-id="da56d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="da56d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da56d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="da56d-122">Authorization</span></span>|<span data-ttu-id="da56d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da56d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da56d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da56d-124">Accept</span></span>|<span data-ttu-id="da56d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da56d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da56d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da56d-126">Request body</span></span>
<span data-ttu-id="da56d-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="da56d-127">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="da56d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="da56d-128">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="da56d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da56d-129">Property</span></span>|<span data-ttu-id="da56d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="da56d-130">Type</span></span>|<span data-ttu-id="da56d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="da56d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da56d-132">id</span><span class="sxs-lookup"><span data-stu-id="da56d-132">id</span></span>|<span data-ttu-id="da56d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da56d-133">String</span></span>|<span data-ttu-id="da56d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="da56d-134">Key of the entity.</span></span> <span data-ttu-id="da56d-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da56d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="da56d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da56d-137">DateTimeOffset</span></span>|<span data-ttu-id="da56d-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="da56d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="da56d-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da56d-140">roleScopeTagIds</span></span>|<span data-ttu-id="da56d-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="da56d-141">String collection</span></span>|<span data-ttu-id="da56d-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="da56d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da56d-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da56d-144">supportsScopeTags</span></span>|<span data-ttu-id="da56d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="da56d-145">Boolean</span></span>|<span data-ttu-id="da56d-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="da56d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da56d-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="da56d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da56d-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="da56d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da56d-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da56d-149">This property is read-only.</span></span> <span data-ttu-id="da56d-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da56d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="da56d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da56d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="da56d-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="da56d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="da56d-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da56d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="da56d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da56d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="da56d-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="da56d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="da56d-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da56d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="da56d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da56d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="da56d-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="da56d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="da56d-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da56d-163">createdDateTime</span></span>|<span data-ttu-id="da56d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da56d-164">DateTimeOffset</span></span>|<span data-ttu-id="da56d-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="da56d-165">DateTime the object was created.</span></span> <span data-ttu-id="da56d-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-167">descrição</span><span class="sxs-lookup"><span data-stu-id="da56d-167">description</span></span>|<span data-ttu-id="da56d-168">String</span><span class="sxs-lookup"><span data-stu-id="da56d-168">String</span></span>|<span data-ttu-id="da56d-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da56d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da56d-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="da56d-171">displayName</span></span>|<span data-ttu-id="da56d-172">String</span><span class="sxs-lookup"><span data-stu-id="da56d-172">String</span></span>|<span data-ttu-id="da56d-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da56d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da56d-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-175">versão</span><span class="sxs-lookup"><span data-stu-id="da56d-175">version</span></span>|<span data-ttu-id="da56d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="da56d-176">Int32</span></span>|<span data-ttu-id="da56d-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da56d-177">Version of the device configuration.</span></span> <span data-ttu-id="da56d-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da56d-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da56d-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="da56d-179">trustedRootCertificate</span></span>|<span data-ttu-id="da56d-180">Binária</span><span class="sxs-lookup"><span data-stu-id="da56d-180">Binary</span></span>|<span data-ttu-id="da56d-181">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="da56d-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="da56d-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="da56d-182">certFileName</span></span>|<span data-ttu-id="da56d-183">String</span><span class="sxs-lookup"><span data-stu-id="da56d-183">String</span></span>|<span data-ttu-id="da56d-184">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="da56d-184">File name to display in UI.</span></span>|
|<span data-ttu-id="da56d-185">destinationStore</span><span class="sxs-lookup"><span data-stu-id="da56d-185">destinationStore</span></span>|[<span data-ttu-id="da56d-186">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="da56d-186">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="da56d-187">Local do repositório de destino para o certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="da56d-187">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="da56d-188">Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="da56d-188">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="da56d-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="da56d-189">Response</span></span>
<span data-ttu-id="da56d-190">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da56d-190">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da56d-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da56d-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="da56d-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da56d-192">Request</span></span>
<span data-ttu-id="da56d-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da56d-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="da56d-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="da56d-194">Response</span></span>
<span data-ttu-id="da56d-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da56d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





