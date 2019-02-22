---
title: Criar iosEduDeviceConfiguration
description: Criar um novo objeto iosEduDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02a54274513700202ff4c59d43fe8758882bb751
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173742"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="c7702-103">Criar iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7702-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="c7702-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7702-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7702-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7702-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7702-106">Criar um novo objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c7702-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7702-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7702-107">Prerequisites</span></span>
<span data-ttu-id="c7702-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7702-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7702-110">Permission type</span></span>|<span data-ttu-id="c7702-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7702-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7702-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7702-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7702-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7702-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7702-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7702-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7702-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7702-115">Not supported.</span></span>|
|<span data-ttu-id="c7702-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7702-116">Application</span></span>|<span data-ttu-id="c7702-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7702-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7702-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7702-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7702-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7702-119">Request headers</span></span>
|<span data-ttu-id="c7702-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7702-120">Header</span></span>|<span data-ttu-id="c7702-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c7702-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7702-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7702-122">Authorization</span></span>|<span data-ttu-id="c7702-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7702-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7702-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7702-124">Accept</span></span>|<span data-ttu-id="c7702-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7702-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7702-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7702-126">Request body</span></span>
<span data-ttu-id="c7702-127">No corpo da solicitação, forneça uma representação JSON do objeto iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7702-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="c7702-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7702-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="c7702-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7702-129">Property</span></span>|<span data-ttu-id="c7702-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7702-130">Type</span></span>|<span data-ttu-id="c7702-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7702-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7702-132">id</span><span class="sxs-lookup"><span data-stu-id="c7702-132">id</span></span>|<span data-ttu-id="c7702-133">String</span><span class="sxs-lookup"><span data-stu-id="c7702-133">String</span></span>|<span data-ttu-id="c7702-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c7702-134">Key of the entity.</span></span> <span data-ttu-id="c7702-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7702-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c7702-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7702-137">DateTimeOffset</span></span>|<span data-ttu-id="c7702-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c7702-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c7702-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7702-140">roleScopeTagIds</span></span>|<span data-ttu-id="c7702-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7702-141">String collection</span></span>|<span data-ttu-id="c7702-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c7702-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7702-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c7702-144">supportsScopeTags</span></span>|<span data-ttu-id="c7702-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c7702-145">Boolean</span></span>|<span data-ttu-id="c7702-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c7702-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c7702-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c7702-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c7702-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c7702-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c7702-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7702-149">This property is read-only.</span></span> <span data-ttu-id="c7702-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7702-151">createdDateTime</span></span>|<span data-ttu-id="c7702-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7702-152">DateTimeOffset</span></span>|<span data-ttu-id="c7702-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c7702-153">DateTime the object was created.</span></span> <span data-ttu-id="c7702-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-155">description</span><span class="sxs-lookup"><span data-stu-id="c7702-155">description</span></span>|<span data-ttu-id="c7702-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7702-156">String</span></span>|<span data-ttu-id="c7702-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7702-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7702-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c7702-159">displayName</span></span>|<span data-ttu-id="c7702-160">String</span><span class="sxs-lookup"><span data-stu-id="c7702-160">String</span></span>|<span data-ttu-id="c7702-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7702-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7702-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-163">version</span><span class="sxs-lookup"><span data-stu-id="c7702-163">version</span></span>|<span data-ttu-id="c7702-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c7702-164">Int32</span></span>|<span data-ttu-id="c7702-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7702-165">Version of the device configuration.</span></span> <span data-ttu-id="c7702-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7702-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7702-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="c7702-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="c7702-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="c7702-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="c7702-169">Certificados de raiz confiável e PFX para professores</span><span class="sxs-lookup"><span data-stu-id="c7702-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="c7702-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="c7702-170">studentCertificateSettings</span></span>|[<span data-ttu-id="c7702-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="c7702-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="c7702-172">Os certificados de raiz confiável e PFX do aluno</span><span class="sxs-lookup"><span data-stu-id="c7702-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="c7702-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="c7702-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="c7702-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="c7702-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="c7702-175">Os certificados de raiz confiável e PFX do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7702-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="c7702-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7702-176">Response</span></span>
<span data-ttu-id="c7702-177">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7702-177">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7702-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7702-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7702-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7702-179">Request</span></span>
<span data-ttu-id="c7702-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7702-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7702-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7702-181">Response</span></span>
<span data-ttu-id="c7702-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7702-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




