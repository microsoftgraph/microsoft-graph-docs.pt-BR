---
title: Criar iosEduDeviceConfiguration
description: Crie um novo objeto iosEduDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6e9e889b740db34a74529999e83e612b866b073
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129913"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="8c263-103">Criar iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c263-103">Create iosEduDeviceConfiguration</span></span>

<span data-ttu-id="8c263-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c263-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c263-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c263-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c263-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c263-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c263-107">Crie um novo [objeto iosEduDeviceConfiguration.](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c263-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c263-108">Prerequisites</span></span>
<span data-ttu-id="8c263-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c263-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c263-111">Permission type</span></span>|<span data-ttu-id="8c263-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c263-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c263-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c263-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c263-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c263-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c263-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c263-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c263-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c263-116">Not supported.</span></span>|
|<span data-ttu-id="8c263-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c263-117">Application</span></span>|<span data-ttu-id="8c263-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c263-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c263-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c263-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8c263-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c263-120">Request headers</span></span>
|<span data-ttu-id="8c263-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c263-121">Header</span></span>|<span data-ttu-id="8c263-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c263-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c263-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c263-123">Authorization</span></span>|<span data-ttu-id="8c263-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c263-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c263-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c263-125">Accept</span></span>|<span data-ttu-id="8c263-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c263-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c263-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c263-127">Request body</span></span>
<span data-ttu-id="8c263-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8c263-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="8c263-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8c263-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="8c263-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c263-130">Property</span></span>|<span data-ttu-id="8c263-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c263-131">Type</span></span>|<span data-ttu-id="8c263-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c263-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c263-133">id</span><span class="sxs-lookup"><span data-stu-id="8c263-133">id</span></span>|<span data-ttu-id="8c263-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c263-134">String</span></span>|<span data-ttu-id="8c263-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c263-135">Key of the entity.</span></span> <span data-ttu-id="8c263-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c263-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8c263-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c263-138">DateTimeOffset</span></span>|<span data-ttu-id="8c263-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8c263-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8c263-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c263-141">roleScopeTagIds</span></span>|<span data-ttu-id="8c263-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c263-142">String collection</span></span>|<span data-ttu-id="8c263-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="8c263-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8c263-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8c263-145">supportsScopeTags</span></span>|<span data-ttu-id="8c263-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="8c263-146">Boolean</span></span>|<span data-ttu-id="8c263-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8c263-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8c263-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8c263-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8c263-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8c263-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8c263-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8c263-150">This property is read-only.</span></span> <span data-ttu-id="8c263-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8c263-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8c263-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8c263-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8c263-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="8c263-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8c263-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8c263-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8c263-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8c263-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8c263-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="8c263-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8c263-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8c263-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8c263-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8c263-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8c263-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="8c263-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8c263-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c263-164">createdDateTime</span></span>|<span data-ttu-id="8c263-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c263-165">DateTimeOffset</span></span>|<span data-ttu-id="8c263-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8c263-166">DateTime the object was created.</span></span> <span data-ttu-id="8c263-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-168">descrição</span><span class="sxs-lookup"><span data-stu-id="8c263-168">description</span></span>|<span data-ttu-id="8c263-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c263-169">String</span></span>|<span data-ttu-id="8c263-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c263-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8c263-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8c263-172">displayName</span></span>|<span data-ttu-id="8c263-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c263-173">String</span></span>|<span data-ttu-id="8c263-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c263-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8c263-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-176">versão</span><span class="sxs-lookup"><span data-stu-id="8c263-176">version</span></span>|<span data-ttu-id="8c263-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8c263-177">Int32</span></span>|<span data-ttu-id="8c263-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c263-178">Version of the device configuration.</span></span> <span data-ttu-id="8c263-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c263-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c263-180">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="8c263-180">teacherCertificateSettings</span></span>|[<span data-ttu-id="8c263-181">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="8c263-181">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="8c263-182">Os certificados Raiz Confiável e PFX para Professor</span><span class="sxs-lookup"><span data-stu-id="8c263-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="8c263-183">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="8c263-183">studentCertificateSettings</span></span>|[<span data-ttu-id="8c263-184">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="8c263-184">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="8c263-185">Os certificados Raiz Confiável e PFX para Aluno</span><span class="sxs-lookup"><span data-stu-id="8c263-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="8c263-186">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="8c263-186">deviceCertificateSettings</span></span>|[<span data-ttu-id="8c263-187">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="8c263-187">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="8c263-188">Os certificados Raiz Confiável e PFX para Dispositivo</span><span class="sxs-lookup"><span data-stu-id="8c263-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="8c263-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c263-189">Response</span></span>
<span data-ttu-id="8c263-190">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c263-190">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c263-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c263-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c263-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c263-192">Request</span></span>
<span data-ttu-id="8c263-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c263-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2683

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```

### <a name="response"></a><span data-ttu-id="8c263-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c263-194">Response</span></span>
<span data-ttu-id="8c263-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c263-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2855

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```




