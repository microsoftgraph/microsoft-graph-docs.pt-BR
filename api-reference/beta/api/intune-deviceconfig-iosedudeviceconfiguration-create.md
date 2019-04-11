---
title: Criar iosEduDeviceConfiguration
description: Criar um novo objeto iosEduDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ab5c0022994eed79b7905e4c681ec1cc2dd60b7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801978"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="843d7-103">Criar iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="843d7-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="843d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="843d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="843d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="843d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="843d7-106">Criar um novo objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="843d7-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="843d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="843d7-107">Prerequisites</span></span>
<span data-ttu-id="843d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="843d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="843d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="843d7-110">Permission type</span></span>|<span data-ttu-id="843d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="843d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="843d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="843d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="843d7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="843d7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="843d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="843d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="843d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="843d7-115">Not supported.</span></span>|
|<span data-ttu-id="843d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="843d7-116">Application</span></span>|<span data-ttu-id="843d7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="843d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="843d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="843d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="843d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="843d7-119">Request headers</span></span>
|<span data-ttu-id="843d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="843d7-120">Header</span></span>|<span data-ttu-id="843d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="843d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="843d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="843d7-122">Authorization</span></span>|<span data-ttu-id="843d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="843d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="843d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="843d7-124">Accept</span></span>|<span data-ttu-id="843d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="843d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="843d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="843d7-126">Request body</span></span>
<span data-ttu-id="843d7-127">No corpo da solicitação, forneça uma representação JSON do objeto iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="843d7-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="843d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="843d7-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="843d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="843d7-129">Property</span></span>|<span data-ttu-id="843d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="843d7-130">Type</span></span>|<span data-ttu-id="843d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="843d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="843d7-132">id</span><span class="sxs-lookup"><span data-stu-id="843d7-132">id</span></span>|<span data-ttu-id="843d7-133">String</span><span class="sxs-lookup"><span data-stu-id="843d7-133">String</span></span>|<span data-ttu-id="843d7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="843d7-134">Key of the entity.</span></span> <span data-ttu-id="843d7-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="843d7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="843d7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="843d7-137">DateTimeOffset</span></span>|<span data-ttu-id="843d7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="843d7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="843d7-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="843d7-140">roleScopeTagIds</span></span>|<span data-ttu-id="843d7-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="843d7-141">String collection</span></span>|<span data-ttu-id="843d7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="843d7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="843d7-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="843d7-144">supportsScopeTags</span></span>|<span data-ttu-id="843d7-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="843d7-145">Boolean</span></span>|<span data-ttu-id="843d7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="843d7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="843d7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="843d7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="843d7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="843d7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="843d7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="843d7-149">This property is read-only.</span></span> <span data-ttu-id="843d7-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="843d7-151">createdDateTime</span></span>|<span data-ttu-id="843d7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="843d7-152">DateTimeOffset</span></span>|<span data-ttu-id="843d7-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="843d7-153">DateTime the object was created.</span></span> <span data-ttu-id="843d7-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-155">description</span><span class="sxs-lookup"><span data-stu-id="843d7-155">description</span></span>|<span data-ttu-id="843d7-156">String</span><span class="sxs-lookup"><span data-stu-id="843d7-156">String</span></span>|<span data-ttu-id="843d7-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="843d7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="843d7-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="843d7-159">displayName</span></span>|<span data-ttu-id="843d7-160">String</span><span class="sxs-lookup"><span data-stu-id="843d7-160">String</span></span>|<span data-ttu-id="843d7-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="843d7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="843d7-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-163">versão</span><span class="sxs-lookup"><span data-stu-id="843d7-163">version</span></span>|<span data-ttu-id="843d7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="843d7-164">Int32</span></span>|<span data-ttu-id="843d7-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="843d7-165">Version of the device configuration.</span></span> <span data-ttu-id="843d7-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="843d7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="843d7-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="843d7-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="843d7-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="843d7-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="843d7-169">Certificados de raiz confiável e PFX para professores</span><span class="sxs-lookup"><span data-stu-id="843d7-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="843d7-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="843d7-170">studentCertificateSettings</span></span>|[<span data-ttu-id="843d7-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="843d7-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="843d7-172">Os certificados de raiz confiável e PFX do aluno</span><span class="sxs-lookup"><span data-stu-id="843d7-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="843d7-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="843d7-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="843d7-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="843d7-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="843d7-175">Os certificados de raiz confiável e PFX do dispositivo</span><span class="sxs-lookup"><span data-stu-id="843d7-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="843d7-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="843d7-176">Response</span></span>
<span data-ttu-id="843d7-177">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="843d7-177">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="843d7-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="843d7-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="843d7-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="843d7-179">Request</span></span>
<span data-ttu-id="843d7-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="843d7-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1910

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="843d7-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="843d7-181">Response</span></span>
<span data-ttu-id="843d7-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="843d7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2082

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





