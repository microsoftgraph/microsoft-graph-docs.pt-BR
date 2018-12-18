---
title: Atualizar iosEduDeviceConfiguration
description: Atualize as propriedades de um objeto iosEduDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: afeb9c6a93a3af2d64f59e2613e86462a2914158
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307578"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="7d7b1-103">Atualizar iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d7b1-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="7d7b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d7b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d7b1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d7b1-107">Atualize as propriedades de um objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7d7b1-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d7b1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d7b1-108">Prerequisites</span></span>
<span data-ttu-id="7d7b1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7b1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d7b1-111">Permission type</span></span>|<span data-ttu-id="7d7b1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d7b1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d7b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d7b1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d7b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-116">Not supported.</span></span>|
|<span data-ttu-id="7d7b1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d7b1-117">Application</span></span>|<span data-ttu-id="7d7b1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d7b1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d7b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7d7b1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7b1-120">Request headers</span></span>
|<span data-ttu-id="7d7b1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d7b1-121">Header</span></span>|<span data-ttu-id="7d7b1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7d7b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d7b1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d7b1-123">Authorization</span></span>|<span data-ttu-id="7d7b1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d7b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d7b1-125">Accept</span></span>|<span data-ttu-id="7d7b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d7b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7b1-127">Request body</span></span>
<span data-ttu-id="7d7b1-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7d7b1-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="7d7b1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d7b1-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="7d7b1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d7b1-130">Property</span></span>|<span data-ttu-id="7d7b1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d7b1-131">Type</span></span>|<span data-ttu-id="7d7b1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7b1-133">id</span><span class="sxs-lookup"><span data-stu-id="7d7b1-133">id</span></span>|<span data-ttu-id="7d7b1-134">String</span><span class="sxs-lookup"><span data-stu-id="7d7b1-134">String</span></span>|<span data-ttu-id="7d7b1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-135">Key of the entity.</span></span> <span data-ttu-id="7d7b1-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7b1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7d7b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7b1-138">DateTimeOffset</span></span>|<span data-ttu-id="7d7b1-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7d7b1-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d7b1-141">roleScopeTagIds</span></span>|<span data-ttu-id="7d7b1-142">String collection</span><span class="sxs-lookup"><span data-stu-id="7d7b1-142">String collection</span></span>|<span data-ttu-id="7d7b1-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d7b1-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d7b1-145">supportsScopeTags</span></span>|<span data-ttu-id="7d7b1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d7b1-146">Boolean</span></span>|<span data-ttu-id="7d7b1-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d7b1-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d7b1-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d7b1-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-150">This property is read-only.</span></span> <span data-ttu-id="7d7b1-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7b1-152">createdDateTime</span></span>|<span data-ttu-id="7d7b1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7b1-153">DateTimeOffset</span></span>|<span data-ttu-id="7d7b1-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-154">DateTime the object was created.</span></span> <span data-ttu-id="7d7b1-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-156">description</span><span class="sxs-lookup"><span data-stu-id="7d7b1-156">description</span></span>|<span data-ttu-id="7d7b1-157">String</span><span class="sxs-lookup"><span data-stu-id="7d7b1-157">String</span></span>|<span data-ttu-id="7d7b1-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d7b1-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7d7b1-160">displayName</span></span>|<span data-ttu-id="7d7b1-161">String</span><span class="sxs-lookup"><span data-stu-id="7d7b1-161">String</span></span>|<span data-ttu-id="7d7b1-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d7b1-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-164">version</span><span class="sxs-lookup"><span data-stu-id="7d7b1-164">version</span></span>|<span data-ttu-id="7d7b1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7b1-165">Int32</span></span>|<span data-ttu-id="7d7b1-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-166">Version of the device configuration.</span></span> <span data-ttu-id="7d7b1-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7b1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7b1-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7d7b1-168">teacherCertificateSettings</span></span>|[<span data-ttu-id="7d7b1-169">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7d7b1-169">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="7d7b1-170">Os certificados raiz confiáveis e PFX professor</span><span class="sxs-lookup"><span data-stu-id="7d7b1-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="7d7b1-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7d7b1-171">studentCertificateSettings</span></span>|[<span data-ttu-id="7d7b1-172">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7d7b1-172">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="7d7b1-173">Os certificados raiz confiáveis e PFX de Student</span><span class="sxs-lookup"><span data-stu-id="7d7b1-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="7d7b1-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7d7b1-174">deviceCertificateSettings</span></span>|[<span data-ttu-id="7d7b1-175">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7d7b1-175">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="7d7b1-176">Os certificados raiz confiáveis e PFX de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7d7b1-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="7d7b1-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7b1-177">Response</span></span>
<span data-ttu-id="7d7b1-178">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-178">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7b1-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d7b1-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d7b1-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7b1-180">Request</span></span>
<span data-ttu-id="7d7b1-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1910

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="7d7b1-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7b1-182">Response</span></span>
<span data-ttu-id="7d7b1-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d7b1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





