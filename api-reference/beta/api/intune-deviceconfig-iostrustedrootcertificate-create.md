---
title: Criar iosTrustedRootCertificate
description: Criar um novo objeto iosTrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc9de912bfb51c86f1d154a21ffa1c1e5345f9d7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948715"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="5ec61-103">Criar iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5ec61-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="5ec61-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ec61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ec61-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ec61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ec61-106">Criar um novo objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="5ec61-106">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ec61-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ec61-107">Prerequisites</span></span>
<span data-ttu-id="5ec61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ec61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ec61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ec61-110">Permission type</span></span>|<span data-ttu-id="5ec61-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ec61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ec61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ec61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ec61-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec61-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ec61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ec61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ec61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ec61-115">Not supported.</span></span>|
|<span data-ttu-id="5ec61-116">Application</span><span class="sxs-lookup"><span data-stu-id="5ec61-116">Application</span></span>|<span data-ttu-id="5ec61-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec61-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ec61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ec61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="5ec61-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec61-119">Request headers</span></span>
|<span data-ttu-id="5ec61-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ec61-120">Header</span></span>|<span data-ttu-id="5ec61-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ec61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ec61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ec61-122">Authorization</span></span>|<span data-ttu-id="5ec61-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ec61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ec61-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ec61-124">Accept</span></span>|<span data-ttu-id="5ec61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ec61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ec61-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec61-126">Request body</span></span>
<span data-ttu-id="5ec61-127">No corpo da solicitação, forneça uma representação JSON do objeto iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="5ec61-127">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="5ec61-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="5ec61-128">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="5ec61-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ec61-129">Property</span></span>|<span data-ttu-id="5ec61-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ec61-130">Type</span></span>|<span data-ttu-id="5ec61-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ec61-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec61-132">id</span><span class="sxs-lookup"><span data-stu-id="5ec61-132">id</span></span>|<span data-ttu-id="5ec61-133">String</span><span class="sxs-lookup"><span data-stu-id="5ec61-133">String</span></span>|<span data-ttu-id="5ec61-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ec61-134">Key of the entity.</span></span> <span data-ttu-id="5ec61-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec61-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ec61-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec61-137">DateTimeOffset</span></span>|<span data-ttu-id="5ec61-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ec61-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ec61-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ec61-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ec61-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ec61-141">String collection</span></span>|<span data-ttu-id="5ec61-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5ec61-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ec61-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5ec61-144">supportsScopeTags</span></span>|<span data-ttu-id="5ec61-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ec61-145">Boolean</span></span>|<span data-ttu-id="5ec61-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5ec61-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ec61-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5ec61-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ec61-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5ec61-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ec61-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ec61-149">This property is read-only.</span></span> <span data-ttu-id="5ec61-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ec61-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5ec61-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ec61-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5ec61-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5ec61-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5ec61-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ec61-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5ec61-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ec61-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5ec61-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5ec61-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5ec61-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ec61-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5ec61-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ec61-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5ec61-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5ec61-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5ec61-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec61-163">createdDateTime</span></span>|<span data-ttu-id="5ec61-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec61-164">DateTimeOffset</span></span>|<span data-ttu-id="5ec61-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ec61-165">DateTime the object was created.</span></span> <span data-ttu-id="5ec61-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-167">description</span><span class="sxs-lookup"><span data-stu-id="5ec61-167">description</span></span>|<span data-ttu-id="5ec61-168">String</span><span class="sxs-lookup"><span data-stu-id="5ec61-168">String</span></span>|<span data-ttu-id="5ec61-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ec61-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ec61-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5ec61-171">displayName</span></span>|<span data-ttu-id="5ec61-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ec61-172">String</span></span>|<span data-ttu-id="5ec61-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ec61-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ec61-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-175">versão</span><span class="sxs-lookup"><span data-stu-id="5ec61-175">version</span></span>|<span data-ttu-id="5ec61-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec61-176">Int32</span></span>|<span data-ttu-id="5ec61-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ec61-177">Version of the device configuration.</span></span> <span data-ttu-id="5ec61-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ec61-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec61-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5ec61-179">trustedRootCertificate</span></span>|<span data-ttu-id="5ec61-180">Binária</span><span class="sxs-lookup"><span data-stu-id="5ec61-180">Binary</span></span>|<span data-ttu-id="5ec61-181">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="5ec61-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="5ec61-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="5ec61-182">certFileName</span></span>|<span data-ttu-id="5ec61-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="5ec61-183">String</span></span>|<span data-ttu-id="5ec61-184">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ec61-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="5ec61-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec61-185">Response</span></span>
<span data-ttu-id="5ec61-186">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec61-186">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ec61-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ec61-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ec61-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec61-188">Request</span></span>
<span data-ttu-id="5ec61-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ec61-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 1136

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="5ec61-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec61-190">Response</span></span>
<span data-ttu-id="5ec61-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ec61-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1308

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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





