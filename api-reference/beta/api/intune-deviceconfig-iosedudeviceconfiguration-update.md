---
title: Atualizar iosEduDeviceConfiguration
description: Atualiza as propriedades de um objeto iosEduDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4da4b6c7ec00d3ea28f06769178edd31dd0be354
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439210"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="723e8-103">Atualizar iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="723e8-103">Update iosEduDeviceConfiguration</span></span>

<span data-ttu-id="723e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="723e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="723e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="723e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="723e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="723e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="723e8-107">Atualiza as propriedades de um objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="723e8-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="723e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="723e8-108">Prerequisites</span></span>
<span data-ttu-id="723e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="723e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="723e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="723e8-111">Permission type</span></span>|<span data-ttu-id="723e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="723e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="723e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="723e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="723e8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723e8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="723e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="723e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="723e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="723e8-116">Not supported.</span></span>|
|<span data-ttu-id="723e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="723e8-117">Application</span></span>|<span data-ttu-id="723e8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723e8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="723e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="723e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="723e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="723e8-120">Request headers</span></span>
|<span data-ttu-id="723e8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="723e8-121">Header</span></span>|<span data-ttu-id="723e8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="723e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="723e8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="723e8-123">Authorization</span></span>|<span data-ttu-id="723e8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="723e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="723e8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="723e8-125">Accept</span></span>|<span data-ttu-id="723e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="723e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="723e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="723e8-127">Request body</span></span>
<span data-ttu-id="723e8-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="723e8-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="723e8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="723e8-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="723e8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="723e8-130">Property</span></span>|<span data-ttu-id="723e8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="723e8-131">Type</span></span>|<span data-ttu-id="723e8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="723e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="723e8-133">id</span><span class="sxs-lookup"><span data-stu-id="723e8-133">id</span></span>|<span data-ttu-id="723e8-134">String</span><span class="sxs-lookup"><span data-stu-id="723e8-134">String</span></span>|<span data-ttu-id="723e8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="723e8-135">Key of the entity.</span></span> <span data-ttu-id="723e8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="723e8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="723e8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="723e8-138">DateTimeOffset</span></span>|<span data-ttu-id="723e8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="723e8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="723e8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="723e8-141">roleScopeTagIds</span></span>|<span data-ttu-id="723e8-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="723e8-142">String collection</span></span>|<span data-ttu-id="723e8-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="723e8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="723e8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="723e8-145">supportsScopeTags</span></span>|<span data-ttu-id="723e8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="723e8-146">Boolean</span></span>|<span data-ttu-id="723e8-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="723e8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="723e8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="723e8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="723e8-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="723e8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="723e8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="723e8-150">This property is read-only.</span></span> <span data-ttu-id="723e8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="723e8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="723e8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="723e8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="723e8-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="723e8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="723e8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="723e8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="723e8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="723e8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="723e8-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="723e8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="723e8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="723e8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="723e8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="723e8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="723e8-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="723e8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="723e8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="723e8-164">createdDateTime</span></span>|<span data-ttu-id="723e8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="723e8-165">DateTimeOffset</span></span>|<span data-ttu-id="723e8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="723e8-166">DateTime the object was created.</span></span> <span data-ttu-id="723e8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-168">description</span><span class="sxs-lookup"><span data-stu-id="723e8-168">description</span></span>|<span data-ttu-id="723e8-169">String</span><span class="sxs-lookup"><span data-stu-id="723e8-169">String</span></span>|<span data-ttu-id="723e8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="723e8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="723e8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="723e8-172">displayName</span></span>|<span data-ttu-id="723e8-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="723e8-173">String</span></span>|<span data-ttu-id="723e8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="723e8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="723e8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-176">versão</span><span class="sxs-lookup"><span data-stu-id="723e8-176">version</span></span>|<span data-ttu-id="723e8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="723e8-177">Int32</span></span>|<span data-ttu-id="723e8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="723e8-178">Version of the device configuration.</span></span> <span data-ttu-id="723e8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="723e8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="723e8-180">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="723e8-180">teacherCertificateSettings</span></span>|[<span data-ttu-id="723e8-181">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="723e8-181">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="723e8-182">Certificados de raiz confiável e PFX para professores</span><span class="sxs-lookup"><span data-stu-id="723e8-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="723e8-183">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="723e8-183">studentCertificateSettings</span></span>|[<span data-ttu-id="723e8-184">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="723e8-184">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="723e8-185">Os certificados de raiz confiável e PFX do aluno</span><span class="sxs-lookup"><span data-stu-id="723e8-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="723e8-186">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="723e8-186">deviceCertificateSettings</span></span>|[<span data-ttu-id="723e8-187">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="723e8-187">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="723e8-188">Os certificados de raiz confiável e PFX do dispositivo</span><span class="sxs-lookup"><span data-stu-id="723e8-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="723e8-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="723e8-189">Response</span></span>
<span data-ttu-id="723e8-190">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="723e8-190">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="723e8-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="723e8-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="723e8-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="723e8-192">Request</span></span>
<span data-ttu-id="723e8-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="723e8-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="723e8-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="723e8-194">Response</span></span>
<span data-ttu-id="723e8-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="723e8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



