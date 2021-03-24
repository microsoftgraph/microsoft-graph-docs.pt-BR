---
title: Criar iosTrustedRootCertificate
description: Crie um novo objeto iosTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d5de056c846c6a3e0c035dd2f39ecc9bbb185bc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147718"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="69ed2-103">Criar iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69ed2-103">Create iosTrustedRootCertificate</span></span>

<span data-ttu-id="69ed2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ed2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69ed2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69ed2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69ed2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69ed2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69ed2-107">Crie um novo [objeto iosTrustedRootCertificate.](../resources/intune-deviceconfig-iostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-107">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69ed2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69ed2-108">Prerequisites</span></span>
<span data-ttu-id="69ed2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ed2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69ed2-111">Permission type</span></span>|<span data-ttu-id="69ed2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69ed2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ed2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69ed2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69ed2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ed2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69ed2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69ed2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ed2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69ed2-116">Not supported.</span></span>|
|<span data-ttu-id="69ed2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69ed2-117">Application</span></span>|<span data-ttu-id="69ed2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ed2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ed2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69ed2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="69ed2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69ed2-120">Request headers</span></span>
|<span data-ttu-id="69ed2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69ed2-121">Header</span></span>|<span data-ttu-id="69ed2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="69ed2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ed2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="69ed2-123">Authorization</span></span>|<span data-ttu-id="69ed2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69ed2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ed2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69ed2-125">Accept</span></span>|<span data-ttu-id="69ed2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69ed2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ed2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69ed2-127">Request body</span></span>
<span data-ttu-id="69ed2-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="69ed2-128">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="69ed2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="69ed2-129">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="69ed2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69ed2-130">Property</span></span>|<span data-ttu-id="69ed2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="69ed2-131">Type</span></span>|<span data-ttu-id="69ed2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="69ed2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69ed2-133">id</span><span class="sxs-lookup"><span data-stu-id="69ed2-133">id</span></span>|<span data-ttu-id="69ed2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69ed2-134">String</span></span>|<span data-ttu-id="69ed2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69ed2-135">Key of the entity.</span></span> <span data-ttu-id="69ed2-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69ed2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="69ed2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ed2-138">DateTimeOffset</span></span>|<span data-ttu-id="69ed2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="69ed2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="69ed2-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="69ed2-141">roleScopeTagIds</span></span>|<span data-ttu-id="69ed2-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="69ed2-142">String collection</span></span>|<span data-ttu-id="69ed2-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="69ed2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="69ed2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="69ed2-145">supportsScopeTags</span></span>|<span data-ttu-id="69ed2-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="69ed2-146">Boolean</span></span>|<span data-ttu-id="69ed2-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="69ed2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="69ed2-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="69ed2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="69ed2-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="69ed2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="69ed2-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69ed2-150">This property is read-only.</span></span> <span data-ttu-id="69ed2-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="69ed2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="69ed2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="69ed2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="69ed2-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="69ed2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="69ed2-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="69ed2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="69ed2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="69ed2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="69ed2-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="69ed2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="69ed2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="69ed2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="69ed2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="69ed2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="69ed2-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="69ed2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="69ed2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69ed2-164">createdDateTime</span></span>|<span data-ttu-id="69ed2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ed2-165">DateTimeOffset</span></span>|<span data-ttu-id="69ed2-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="69ed2-166">DateTime the object was created.</span></span> <span data-ttu-id="69ed2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-168">descrição</span><span class="sxs-lookup"><span data-stu-id="69ed2-168">description</span></span>|<span data-ttu-id="69ed2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69ed2-169">String</span></span>|<span data-ttu-id="69ed2-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69ed2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69ed2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="69ed2-172">displayName</span></span>|<span data-ttu-id="69ed2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69ed2-173">String</span></span>|<span data-ttu-id="69ed2-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69ed2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69ed2-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-176">versão</span><span class="sxs-lookup"><span data-stu-id="69ed2-176">version</span></span>|<span data-ttu-id="69ed2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed2-177">Int32</span></span>|<span data-ttu-id="69ed2-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69ed2-178">Version of the device configuration.</span></span> <span data-ttu-id="69ed2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69ed2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69ed2-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69ed2-180">trustedRootCertificate</span></span>|<span data-ttu-id="69ed2-181">Binário</span><span class="sxs-lookup"><span data-stu-id="69ed2-181">Binary</span></span>|<span data-ttu-id="69ed2-182">Certificado Raiz Confiável.</span><span class="sxs-lookup"><span data-stu-id="69ed2-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="69ed2-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="69ed2-183">certFileName</span></span>|<span data-ttu-id="69ed2-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69ed2-184">String</span></span>|<span data-ttu-id="69ed2-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="69ed2-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="69ed2-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ed2-186">Response</span></span>
<span data-ttu-id="69ed2-187">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69ed2-187">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ed2-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69ed2-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="69ed2-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69ed2-189">Request</span></span>
<span data-ttu-id="69ed2-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69ed2-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69ed2-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ed2-191">Response</span></span>
<span data-ttu-id="69ed2-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69ed2-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




