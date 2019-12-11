---
title: Criar iosEduDeviceConfiguration
description: Criar um novo objeto iosEduDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d035345050c1b872c1e7ab1e8699294c013a20d8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948960"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="37010-103">Criar iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="37010-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="37010-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37010-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37010-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37010-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37010-106">Criar um novo objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="37010-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37010-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37010-107">Prerequisites</span></span>
<span data-ttu-id="37010-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37010-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37010-110">Permission type</span></span>|<span data-ttu-id="37010-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37010-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37010-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37010-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37010-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37010-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37010-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37010-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37010-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37010-115">Not supported.</span></span>|
|<span data-ttu-id="37010-116">Application</span><span class="sxs-lookup"><span data-stu-id="37010-116">Application</span></span>|<span data-ttu-id="37010-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37010-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37010-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37010-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="37010-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37010-119">Request headers</span></span>
|<span data-ttu-id="37010-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37010-120">Header</span></span>|<span data-ttu-id="37010-121">Valor</span><span class="sxs-lookup"><span data-stu-id="37010-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37010-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37010-122">Authorization</span></span>|<span data-ttu-id="37010-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37010-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37010-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37010-124">Accept</span></span>|<span data-ttu-id="37010-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37010-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37010-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37010-126">Request body</span></span>
<span data-ttu-id="37010-127">No corpo da solicitação, forneça uma representação JSON do objeto iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="37010-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="37010-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="37010-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="37010-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37010-129">Property</span></span>|<span data-ttu-id="37010-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37010-130">Type</span></span>|<span data-ttu-id="37010-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37010-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37010-132">id</span><span class="sxs-lookup"><span data-stu-id="37010-132">id</span></span>|<span data-ttu-id="37010-133">String</span><span class="sxs-lookup"><span data-stu-id="37010-133">String</span></span>|<span data-ttu-id="37010-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37010-134">Key of the entity.</span></span> <span data-ttu-id="37010-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37010-136">lastModifiedDateTime</span></span>|<span data-ttu-id="37010-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37010-137">DateTimeOffset</span></span>|<span data-ttu-id="37010-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="37010-138">DateTime the object was last modified.</span></span> <span data-ttu-id="37010-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37010-140">roleScopeTagIds</span></span>|<span data-ttu-id="37010-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37010-141">String collection</span></span>|<span data-ttu-id="37010-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="37010-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37010-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37010-144">supportsScopeTags</span></span>|<span data-ttu-id="37010-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="37010-145">Boolean</span></span>|<span data-ttu-id="37010-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="37010-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37010-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="37010-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37010-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="37010-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37010-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37010-149">This property is read-only.</span></span> <span data-ttu-id="37010-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37010-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="37010-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37010-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="37010-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="37010-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="37010-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37010-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="37010-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37010-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="37010-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="37010-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="37010-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37010-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="37010-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37010-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="37010-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="37010-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="37010-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37010-163">createdDateTime</span></span>|<span data-ttu-id="37010-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37010-164">DateTimeOffset</span></span>|<span data-ttu-id="37010-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="37010-165">DateTime the object was created.</span></span> <span data-ttu-id="37010-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-167">description</span><span class="sxs-lookup"><span data-stu-id="37010-167">description</span></span>|<span data-ttu-id="37010-168">String</span><span class="sxs-lookup"><span data-stu-id="37010-168">String</span></span>|<span data-ttu-id="37010-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37010-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37010-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-171">displayName</span><span class="sxs-lookup"><span data-stu-id="37010-171">displayName</span></span>|<span data-ttu-id="37010-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37010-172">String</span></span>|<span data-ttu-id="37010-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37010-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37010-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-175">versão</span><span class="sxs-lookup"><span data-stu-id="37010-175">version</span></span>|<span data-ttu-id="37010-176">Int32</span><span class="sxs-lookup"><span data-stu-id="37010-176">Int32</span></span>|<span data-ttu-id="37010-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37010-177">Version of the device configuration.</span></span> <span data-ttu-id="37010-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37010-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37010-179">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="37010-179">teacherCertificateSettings</span></span>|[<span data-ttu-id="37010-180">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="37010-180">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="37010-181">Certificados de raiz confiável e PFX para professores</span><span class="sxs-lookup"><span data-stu-id="37010-181">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="37010-182">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="37010-182">studentCertificateSettings</span></span>|[<span data-ttu-id="37010-183">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="37010-183">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="37010-184">Os certificados de raiz confiável e PFX do aluno</span><span class="sxs-lookup"><span data-stu-id="37010-184">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="37010-185">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="37010-185">deviceCertificateSettings</span></span>|[<span data-ttu-id="37010-186">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="37010-186">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="37010-187">Os certificados de raiz confiável e PFX do dispositivo</span><span class="sxs-lookup"><span data-stu-id="37010-187">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="37010-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="37010-188">Response</span></span>
<span data-ttu-id="37010-189">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37010-189">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37010-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37010-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="37010-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37010-191">Request</span></span>
<span data-ttu-id="37010-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37010-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37010-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="37010-193">Response</span></span>
<span data-ttu-id="37010-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37010-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





