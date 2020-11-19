---
title: Atualizar iosTrustedRootCertificate
description: Atualiza as propriedades de um objeto iosTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 298752e1dd390d536c83c60efabeb1d8b0a4c4e8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300329"
---
# <a name="update-iostrustedrootcertificate"></a><span data-ttu-id="69f8d-103">Atualizar iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69f8d-103">Update iosTrustedRootCertificate</span></span>

<span data-ttu-id="69f8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69f8d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69f8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f8d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69f8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f8d-107">Atualiza as propriedades de um objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="69f8d-107">Update the properties of a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f8d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69f8d-108">Prerequisites</span></span>
<span data-ttu-id="69f8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69f8d-111">Permission type</span></span>|<span data-ttu-id="69f8d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69f8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69f8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69f8d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f8d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69f8d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69f8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69f8d-116">Not supported.</span></span>|
|<span data-ttu-id="69f8d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69f8d-117">Application</span></span>|<span data-ttu-id="69f8d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f8d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f8d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69f8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="69f8d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69f8d-120">Request headers</span></span>
|<span data-ttu-id="69f8d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69f8d-121">Header</span></span>|<span data-ttu-id="69f8d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="69f8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f8d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="69f8d-123">Authorization</span></span>|<span data-ttu-id="69f8d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69f8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f8d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69f8d-125">Accept</span></span>|<span data-ttu-id="69f8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69f8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69f8d-127">Request body</span></span>
<span data-ttu-id="69f8d-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="69f8d-128">In the request body, supply a JSON representation for the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="69f8d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="69f8d-129">The following table shows the properties that are required when you create the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="69f8d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69f8d-130">Property</span></span>|<span data-ttu-id="69f8d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="69f8d-131">Type</span></span>|<span data-ttu-id="69f8d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f8d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f8d-133">id</span><span class="sxs-lookup"><span data-stu-id="69f8d-133">id</span></span>|<span data-ttu-id="69f8d-134">String</span><span class="sxs-lookup"><span data-stu-id="69f8d-134">String</span></span>|<span data-ttu-id="69f8d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69f8d-135">Key of the entity.</span></span> <span data-ttu-id="69f8d-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69f8d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="69f8d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69f8d-138">DateTimeOffset</span></span>|<span data-ttu-id="69f8d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="69f8d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="69f8d-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="69f8d-141">roleScopeTagIds</span></span>|<span data-ttu-id="69f8d-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="69f8d-142">String collection</span></span>|<span data-ttu-id="69f8d-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="69f8d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="69f8d-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="69f8d-145">supportsScopeTags</span></span>|<span data-ttu-id="69f8d-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="69f8d-146">Boolean</span></span>|<span data-ttu-id="69f8d-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="69f8d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="69f8d-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="69f8d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="69f8d-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="69f8d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="69f8d-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69f8d-150">This property is read-only.</span></span> <span data-ttu-id="69f8d-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="69f8d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="69f8d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="69f8d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="69f8d-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="69f8d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="69f8d-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="69f8d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="69f8d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="69f8d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="69f8d-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="69f8d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="69f8d-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="69f8d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="69f8d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="69f8d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="69f8d-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="69f8d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="69f8d-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69f8d-164">createdDateTime</span></span>|<span data-ttu-id="69f8d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69f8d-165">DateTimeOffset</span></span>|<span data-ttu-id="69f8d-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="69f8d-166">DateTime the object was created.</span></span> <span data-ttu-id="69f8d-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-168">description</span><span class="sxs-lookup"><span data-stu-id="69f8d-168">description</span></span>|<span data-ttu-id="69f8d-169">String</span><span class="sxs-lookup"><span data-stu-id="69f8d-169">String</span></span>|<span data-ttu-id="69f8d-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69f8d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69f8d-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="69f8d-172">displayName</span></span>|<span data-ttu-id="69f8d-173">String</span><span class="sxs-lookup"><span data-stu-id="69f8d-173">String</span></span>|<span data-ttu-id="69f8d-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69f8d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69f8d-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-176">versão</span><span class="sxs-lookup"><span data-stu-id="69f8d-176">version</span></span>|<span data-ttu-id="69f8d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="69f8d-177">Int32</span></span>|<span data-ttu-id="69f8d-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69f8d-178">Version of the device configuration.</span></span> <span data-ttu-id="69f8d-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69f8d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69f8d-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69f8d-180">trustedRootCertificate</span></span>|<span data-ttu-id="69f8d-181">Binária</span><span class="sxs-lookup"><span data-stu-id="69f8d-181">Binary</span></span>|<span data-ttu-id="69f8d-182">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="69f8d-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="69f8d-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="69f8d-183">certFileName</span></span>|<span data-ttu-id="69f8d-184">String</span><span class="sxs-lookup"><span data-stu-id="69f8d-184">String</span></span>|<span data-ttu-id="69f8d-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="69f8d-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="69f8d-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f8d-186">Response</span></span>
<span data-ttu-id="69f8d-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69f8d-187">If successful, this method returns a `200 OK` response code and an updated [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f8d-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69f8d-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f8d-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69f8d-189">Request</span></span>
<span data-ttu-id="69f8d-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69f8d-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
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

### <a name="response"></a><span data-ttu-id="69f8d-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f8d-191">Response</span></span>
<span data-ttu-id="69f8d-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69f8d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




