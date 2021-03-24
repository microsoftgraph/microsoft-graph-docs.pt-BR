---
title: Atualizar androidWorkProfileTrustedRootCertificate
description: Atualize as propriedades de um objeto androidWorkProfileTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f299fa239ebde1e6af234b0379bc3c78e65bd66
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148047"
---
# <a name="update-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="988b8-103">Atualizar androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="988b8-103">Update androidWorkProfileTrustedRootCertificate</span></span>

<span data-ttu-id="988b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="988b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="988b8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="988b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="988b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="988b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="988b8-107">Atualize as propriedades de [um objeto androidWorkProfileTrustedRootCertificate.](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-107">Update the properties of a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="988b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="988b8-108">Prerequisites</span></span>
<span data-ttu-id="988b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="988b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="988b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="988b8-111">Permission type</span></span>|<span data-ttu-id="988b8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="988b8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="988b8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="988b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="988b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="988b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="988b8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="988b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="988b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="988b8-116">Not supported.</span></span>|
|<span data-ttu-id="988b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="988b8-117">Application</span></span>|<span data-ttu-id="988b8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="988b8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="988b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="988b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="988b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="988b8-120">Request headers</span></span>
|<span data-ttu-id="988b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="988b8-121">Header</span></span>|<span data-ttu-id="988b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="988b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="988b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="988b8-123">Authorization</span></span>|<span data-ttu-id="988b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="988b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="988b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="988b8-125">Accept</span></span>|<span data-ttu-id="988b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="988b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="988b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="988b8-127">Request body</span></span>
<span data-ttu-id="988b8-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidWorkProfileTrustedRootCertificate.](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-128">In the request body, supply a JSON representation for the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="988b8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="988b8-129">The following table shows the properties that are required when you create the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span></span>

|<span data-ttu-id="988b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="988b8-130">Property</span></span>|<span data-ttu-id="988b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="988b8-131">Type</span></span>|<span data-ttu-id="988b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="988b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="988b8-133">id</span><span class="sxs-lookup"><span data-stu-id="988b8-133">id</span></span>|<span data-ttu-id="988b8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="988b8-134">String</span></span>|<span data-ttu-id="988b8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="988b8-135">Key of the entity.</span></span> <span data-ttu-id="988b8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="988b8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="988b8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988b8-138">DateTimeOffset</span></span>|<span data-ttu-id="988b8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="988b8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="988b8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="988b8-141">roleScopeTagIds</span></span>|<span data-ttu-id="988b8-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="988b8-142">String collection</span></span>|<span data-ttu-id="988b8-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="988b8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="988b8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="988b8-145">supportsScopeTags</span></span>|<span data-ttu-id="988b8-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="988b8-146">Boolean</span></span>|<span data-ttu-id="988b8-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="988b8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="988b8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="988b8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="988b8-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="988b8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="988b8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="988b8-150">This property is read-only.</span></span> <span data-ttu-id="988b8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="988b8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="988b8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="988b8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="988b8-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="988b8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="988b8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="988b8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="988b8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="988b8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="988b8-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="988b8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="988b8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="988b8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="988b8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="988b8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="988b8-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="988b8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="988b8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="988b8-164">createdDateTime</span></span>|<span data-ttu-id="988b8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988b8-165">DateTimeOffset</span></span>|<span data-ttu-id="988b8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="988b8-166">DateTime the object was created.</span></span> <span data-ttu-id="988b8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-168">descrição</span><span class="sxs-lookup"><span data-stu-id="988b8-168">description</span></span>|<span data-ttu-id="988b8-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="988b8-169">String</span></span>|<span data-ttu-id="988b8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="988b8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="988b8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="988b8-172">displayName</span></span>|<span data-ttu-id="988b8-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="988b8-173">String</span></span>|<span data-ttu-id="988b8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="988b8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="988b8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-176">versão</span><span class="sxs-lookup"><span data-stu-id="988b8-176">version</span></span>|<span data-ttu-id="988b8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="988b8-177">Int32</span></span>|<span data-ttu-id="988b8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="988b8-178">Version of the device configuration.</span></span> <span data-ttu-id="988b8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="988b8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="988b8-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="988b8-180">trustedRootCertificate</span></span>|<span data-ttu-id="988b8-181">Binário</span><span class="sxs-lookup"><span data-stu-id="988b8-181">Binary</span></span>|<span data-ttu-id="988b8-182">Certificado Raiz Confiável</span><span class="sxs-lookup"><span data-stu-id="988b8-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="988b8-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="988b8-183">certFileName</span></span>|<span data-ttu-id="988b8-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="988b8-184">String</span></span>|<span data-ttu-id="988b8-185">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="988b8-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="988b8-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="988b8-186">Response</span></span>
<span data-ttu-id="988b8-187">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="988b8-187">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="988b8-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="988b8-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="988b8-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="988b8-189">Request</span></span>
<span data-ttu-id="988b8-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="988b8-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="988b8-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="988b8-191">Response</span></span>
<span data-ttu-id="988b8-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="988b8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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




