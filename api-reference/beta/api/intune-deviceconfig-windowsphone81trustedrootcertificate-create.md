---
title: Criar windowsPhone81TrustedRootCertificate
description: Criar um novo objeto windowsPhone81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8a7cb78c99c060e8ab449c89efc16623c0fb82e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532747"
---
# <a name="create-windowsphone81trustedrootcertificate"></a><span data-ttu-id="5c5e7-103">Criar windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5c5e7-103">Create windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="5c5e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c5e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c5e7-106">Criar um novo objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="5c5e7-106">Create a new [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c5e7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c5e7-107">Prerequisites</span></span>
<span data-ttu-id="5c5e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c5e7-110">Permission type</span></span>|<span data-ttu-id="5c5e7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c5e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c5e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c5e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c5e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-115">Not supported.</span></span>|
|<span data-ttu-id="5c5e7-116">Application</span><span class="sxs-lookup"><span data-stu-id="5c5e7-116">Application</span></span>|<span data-ttu-id="5c5e7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5e7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c5e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c5e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5e7-119">Request headers</span></span>
|<span data-ttu-id="5c5e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c5e7-120">Header</span></span>|<span data-ttu-id="5c5e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5c5e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c5e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c5e7-122">Authorization</span></span>|<span data-ttu-id="5c5e7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c5e7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c5e7-124">Accept</span></span>|<span data-ttu-id="5c5e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c5e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5e7-126">Request body</span></span>
<span data-ttu-id="5c5e7-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-127">In the request body, supply a JSON representation for the windowsPhone81TrustedRootCertificate object.</span></span>

<span data-ttu-id="5c5e7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-128">The following table shows the properties that are required when you create the windowsPhone81TrustedRootCertificate.</span></span>

|<span data-ttu-id="5c5e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c5e7-129">Property</span></span>|<span data-ttu-id="5c5e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c5e7-130">Type</span></span>|<span data-ttu-id="5c5e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c5e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c5e7-132">id</span><span class="sxs-lookup"><span data-stu-id="5c5e7-132">id</span></span>|<span data-ttu-id="5c5e7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c5e7-133">String</span></span>|<span data-ttu-id="5c5e7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-134">Key of the entity.</span></span> <span data-ttu-id="5c5e7-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c5e7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c5e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c5e7-137">DateTimeOffset</span></span>|<span data-ttu-id="5c5e7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c5e7-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c5e7-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c5e7-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5c5e7-141">String collection</span></span>|<span data-ttu-id="5c5e7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c5e7-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5c5e7-144">supportsScopeTags</span></span>|<span data-ttu-id="5c5e7-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c5e7-145">Boolean</span></span>|<span data-ttu-id="5c5e7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c5e7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c5e7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c5e7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-149">This property is read-only.</span></span> <span data-ttu-id="5c5e7-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c5e7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5c5e7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c5e7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5c5e7-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5c5e7-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c5e7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5c5e7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c5e7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5c5e7-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5c5e7-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c5e7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5c5e7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c5e7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5c5e7-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5c5e7-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c5e7-163">createdDateTime</span></span>|<span data-ttu-id="5c5e7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c5e7-164">DateTimeOffset</span></span>|<span data-ttu-id="5c5e7-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-165">DateTime the object was created.</span></span> <span data-ttu-id="5c5e7-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-167">description</span><span class="sxs-lookup"><span data-stu-id="5c5e7-167">description</span></span>|<span data-ttu-id="5c5e7-168">String</span><span class="sxs-lookup"><span data-stu-id="5c5e7-168">String</span></span>|<span data-ttu-id="5c5e7-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c5e7-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5c5e7-171">displayName</span></span>|<span data-ttu-id="5c5e7-172">String</span><span class="sxs-lookup"><span data-stu-id="5c5e7-172">String</span></span>|<span data-ttu-id="5c5e7-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c5e7-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-175">versão</span><span class="sxs-lookup"><span data-stu-id="5c5e7-175">version</span></span>|<span data-ttu-id="5c5e7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5c5e7-176">Int32</span></span>|<span data-ttu-id="5c5e7-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-177">Version of the device configuration.</span></span> <span data-ttu-id="5c5e7-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c5e7-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c5e7-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5c5e7-179">trustedRootCertificate</span></span>|<span data-ttu-id="5c5e7-180">Binária</span><span class="sxs-lookup"><span data-stu-id="5c5e7-180">Binary</span></span>|<span data-ttu-id="5c5e7-181">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="5c5e7-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="5c5e7-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="5c5e7-182">certFileName</span></span>|<span data-ttu-id="5c5e7-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c5e7-183">String</span></span>|<span data-ttu-id="5c5e7-184">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="5c5e7-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5e7-185">Response</span></span>
<span data-ttu-id="5c5e7-186">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-186">If successful, this method returns a `201 Created` response code and a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c5e7-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c5e7-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c5e7-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5e7-188">Request</span></span>
<span data-ttu-id="5c5e7-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="5c5e7-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5e7-190">Response</span></span>
<span data-ttu-id="5c5e7-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c5e7-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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






