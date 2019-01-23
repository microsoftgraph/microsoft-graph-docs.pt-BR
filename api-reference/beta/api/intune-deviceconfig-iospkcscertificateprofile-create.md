---
title: Criar iosPkcsCertificateProfile
description: Crie um novo objeto de iosPkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cb5f93296d7117cd003d807afbdf19211d607a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396256"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="cd9cf-103">Criar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="cd9cf-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="cd9cf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cd9cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd9cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd9cf-107">Crie um novo objeto de [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cd9cf-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd9cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd9cf-108">Prerequisites</span></span>
<span data-ttu-id="cd9cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd9cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cd9cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd9cf-111">Permission type</span></span>|<span data-ttu-id="cd9cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd9cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-116">Not supported.</span></span>|
|<span data-ttu-id="cd9cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd9cf-117">Application</span></span>|<span data-ttu-id="cd9cf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd9cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cd9cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd9cf-120">Request headers</span></span>
|<span data-ttu-id="cd9cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd9cf-121">Header</span></span>|<span data-ttu-id="cd9cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cd9cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd9cf-123">Authorization</span></span>|<span data-ttu-id="cd9cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd9cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd9cf-125">Accept</span></span>|<span data-ttu-id="cd9cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd9cf-127">Request body</span></span>
<span data-ttu-id="cd9cf-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="cd9cf-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="cd9cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd9cf-130">Property</span></span>|<span data-ttu-id="cd9cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd9cf-131">Type</span></span>|<span data-ttu-id="cd9cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd9cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9cf-133">id</span><span class="sxs-lookup"><span data-stu-id="cd9cf-133">id</span></span>|<span data-ttu-id="cd9cf-134">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-134">String</span></span>|<span data-ttu-id="cd9cf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-135">Key of the entity.</span></span> <span data-ttu-id="cd9cf-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd9cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cd9cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd9cf-138">DateTimeOffset</span></span>|<span data-ttu-id="cd9cf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cd9cf-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd9cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="cd9cf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="cd9cf-142">String collection</span></span>|<span data-ttu-id="cd9cf-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd9cf-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cd9cf-145">supportsScopeTags</span></span>|<span data-ttu-id="cd9cf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd9cf-146">Boolean</span></span>|<span data-ttu-id="cd9cf-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cd9cf-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cd9cf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cd9cf-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-150">This property is read-only.</span></span> <span data-ttu-id="cd9cf-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd9cf-152">createdDateTime</span></span>|<span data-ttu-id="cd9cf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd9cf-153">DateTimeOffset</span></span>|<span data-ttu-id="cd9cf-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-154">DateTime the object was created.</span></span> <span data-ttu-id="cd9cf-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-156">description</span><span class="sxs-lookup"><span data-stu-id="cd9cf-156">description</span></span>|<span data-ttu-id="cd9cf-157">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-157">String</span></span>|<span data-ttu-id="cd9cf-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd9cf-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="cd9cf-160">displayName</span></span>|<span data-ttu-id="cd9cf-161">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-161">String</span></span>|<span data-ttu-id="cd9cf-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd9cf-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-164">version</span><span class="sxs-lookup"><span data-stu-id="cd9cf-164">version</span></span>|<span data-ttu-id="cd9cf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cd9cf-165">Int32</span></span>|<span data-ttu-id="cd9cf-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-166">Version of the device configuration.</span></span> <span data-ttu-id="cd9cf-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd9cf-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="cd9cf-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="cd9cf-169">Int32</span><span class="sxs-lookup"><span data-stu-id="cd9cf-169">Int32</span></span>|<span data-ttu-id="cd9cf-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="cd9cf-171">Válido valores de 1 a 99 Inherited de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cd9cf-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cd9cf-172">subjectNameFormat</span></span>|[<span data-ttu-id="cd9cf-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cd9cf-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="cd9cf-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="cd9cf-175">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="cd9cf-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="cd9cf-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="cd9cf-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cd9cf-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="cd9cf-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cd9cf-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="cd9cf-179">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="cd9cf-180">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="cd9cf-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="cd9cf-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="cd9cf-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="cd9cf-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="cd9cf-183">Int32</span><span class="sxs-lookup"><span data-stu-id="cd9cf-183">Int32</span></span>|<span data-ttu-id="cd9cf-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="cd9cf-185">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cd9cf-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cd9cf-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="cd9cf-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cd9cf-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="cd9cf-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="cd9cf-189">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="cd9cf-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="cd9cf-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="cd9cf-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="cd9cf-191">certificationAuthority</span></span>|<span data-ttu-id="cd9cf-192">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-192">String</span></span>|<span data-ttu-id="cd9cf-193">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="cd9cf-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="cd9cf-194">certificationAuthorityName</span></span>|<span data-ttu-id="cd9cf-195">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-195">String</span></span>|<span data-ttu-id="cd9cf-196">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="cd9cf-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="cd9cf-197">certificateTemplateName</span></span>|<span data-ttu-id="cd9cf-198">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-198">String</span></span>|<span data-ttu-id="cd9cf-199">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="cd9cf-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cd9cf-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="cd9cf-201">String</span><span class="sxs-lookup"><span data-stu-id="cd9cf-201">String</span></span>|<span data-ttu-id="cd9cf-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="cd9cf-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd9cf-203">Response</span></span>
<span data-ttu-id="cd9cf-204">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-204">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9cf-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd9cf-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd9cf-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd9cf-206">Request</span></span>
<span data-ttu-id="cd9cf-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="cd9cf-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd9cf-208">Response</span></span>
<span data-ttu-id="cd9cf-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




