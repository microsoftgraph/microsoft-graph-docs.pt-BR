---
title: Criar iosTrustedRootCertificate
description: Criar um novo objeto iosTrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d8e844ff18e383e50256f48d3bfc2a6bb4d3af0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533746"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="76756-103">Criar iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="76756-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="76756-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76756-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76756-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76756-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76756-106">Criar um novo objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="76756-106">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76756-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76756-107">Prerequisites</span></span>
<span data-ttu-id="76756-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76756-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76756-110">Permission type</span></span>|<span data-ttu-id="76756-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76756-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76756-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76756-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76756-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76756-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76756-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76756-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76756-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76756-115">Not supported.</span></span>|
|<span data-ttu-id="76756-116">Application</span><span class="sxs-lookup"><span data-stu-id="76756-116">Application</span></span>|<span data-ttu-id="76756-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76756-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76756-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76756-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="76756-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76756-119">Request headers</span></span>
|<span data-ttu-id="76756-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76756-120">Header</span></span>|<span data-ttu-id="76756-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76756-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76756-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76756-122">Authorization</span></span>|<span data-ttu-id="76756-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76756-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76756-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76756-124">Accept</span></span>|<span data-ttu-id="76756-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76756-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76756-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76756-126">Request body</span></span>
<span data-ttu-id="76756-127">No corpo da solicitação, forneça uma representação JSON do objeto iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="76756-127">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="76756-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="76756-128">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="76756-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76756-129">Property</span></span>|<span data-ttu-id="76756-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="76756-130">Type</span></span>|<span data-ttu-id="76756-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="76756-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76756-132">id</span><span class="sxs-lookup"><span data-stu-id="76756-132">id</span></span>|<span data-ttu-id="76756-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76756-133">String</span></span>|<span data-ttu-id="76756-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76756-134">Key of the entity.</span></span> <span data-ttu-id="76756-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76756-136">lastModifiedDateTime</span></span>|<span data-ttu-id="76756-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76756-137">DateTimeOffset</span></span>|<span data-ttu-id="76756-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76756-138">DateTime the object was last modified.</span></span> <span data-ttu-id="76756-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76756-140">roleScopeTagIds</span></span>|<span data-ttu-id="76756-141">String collection</span><span class="sxs-lookup"><span data-stu-id="76756-141">String collection</span></span>|<span data-ttu-id="76756-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="76756-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76756-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="76756-144">supportsScopeTags</span></span>|<span data-ttu-id="76756-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="76756-145">Boolean</span></span>|<span data-ttu-id="76756-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="76756-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76756-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="76756-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76756-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="76756-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76756-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76756-149">This property is read-only.</span></span> <span data-ttu-id="76756-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76756-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="76756-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76756-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="76756-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="76756-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="76756-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76756-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="76756-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76756-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="76756-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="76756-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="76756-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76756-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="76756-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76756-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="76756-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="76756-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="76756-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76756-163">createdDateTime</span></span>|<span data-ttu-id="76756-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76756-164">DateTimeOffset</span></span>|<span data-ttu-id="76756-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76756-165">DateTime the object was created.</span></span> <span data-ttu-id="76756-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-167">description</span><span class="sxs-lookup"><span data-stu-id="76756-167">description</span></span>|<span data-ttu-id="76756-168">String</span><span class="sxs-lookup"><span data-stu-id="76756-168">String</span></span>|<span data-ttu-id="76756-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76756-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76756-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-171">displayName</span><span class="sxs-lookup"><span data-stu-id="76756-171">displayName</span></span>|<span data-ttu-id="76756-172">String</span><span class="sxs-lookup"><span data-stu-id="76756-172">String</span></span>|<span data-ttu-id="76756-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76756-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76756-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-175">versão</span><span class="sxs-lookup"><span data-stu-id="76756-175">version</span></span>|<span data-ttu-id="76756-176">Int32</span><span class="sxs-lookup"><span data-stu-id="76756-176">Int32</span></span>|<span data-ttu-id="76756-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76756-177">Version of the device configuration.</span></span> <span data-ttu-id="76756-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76756-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76756-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="76756-179">trustedRootCertificate</span></span>|<span data-ttu-id="76756-180">Binária</span><span class="sxs-lookup"><span data-stu-id="76756-180">Binary</span></span>|<span data-ttu-id="76756-181">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="76756-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="76756-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="76756-182">certFileName</span></span>|<span data-ttu-id="76756-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76756-183">String</span></span>|<span data-ttu-id="76756-184">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="76756-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="76756-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="76756-185">Response</span></span>
<span data-ttu-id="76756-186">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76756-186">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76756-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76756-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="76756-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76756-188">Request</span></span>
<span data-ttu-id="76756-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76756-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76756-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="76756-190">Response</span></span>
<span data-ttu-id="76756-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76756-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






