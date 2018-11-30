---
title: Criar iosPkcsCertificateProfile
description: Crie um novo objeto de iosPkcsCertificateProfile.
ms.openlocfilehash: 6d8d20a09c5613acd21d8e18fbbc5dc663366f90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037652"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="a0daf-103">Criar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a0daf-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="a0daf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0daf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0daf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0daf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0daf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0daf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0daf-107">Crie um novo objeto de [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a0daf-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0daf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0daf-108">Prerequisites</span></span>
<span data-ttu-id="a0daf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0daf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0daf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0daf-111">Permission type</span></span>|<span data-ttu-id="a0daf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0daf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0daf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0daf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0daf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0daf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0daf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0daf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0daf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0daf-116">Not supported.</span></span>|
|<span data-ttu-id="a0daf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0daf-117">Application</span></span>|<span data-ttu-id="a0daf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0daf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0daf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0daf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0daf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0daf-120">Request headers</span></span>
|<span data-ttu-id="a0daf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0daf-121">Header</span></span>|<span data-ttu-id="a0daf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0daf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0daf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0daf-123">Authorization</span></span>|<span data-ttu-id="a0daf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0daf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0daf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0daf-125">Accept</span></span>|<span data-ttu-id="a0daf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0daf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0daf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0daf-127">Request body</span></span>
<span data-ttu-id="a0daf-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a0daf-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="a0daf-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a0daf-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="a0daf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0daf-130">Property</span></span>|<span data-ttu-id="a0daf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0daf-131">Type</span></span>|<span data-ttu-id="a0daf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0daf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0daf-133">id</span><span class="sxs-lookup"><span data-stu-id="a0daf-133">id</span></span>|<span data-ttu-id="a0daf-134">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-134">String</span></span>|<span data-ttu-id="a0daf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0daf-135">Key of the entity.</span></span> <span data-ttu-id="a0daf-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0daf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a0daf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0daf-138">DateTimeOffset</span></span>|<span data-ttu-id="a0daf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0daf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a0daf-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0daf-141">roleScopeTagIds</span></span>|<span data-ttu-id="a0daf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a0daf-142">String collection</span></span>|<span data-ttu-id="a0daf-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0daf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0daf-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0daf-145">supportsScopeTags</span></span>|<span data-ttu-id="a0daf-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a0daf-146">Boolean</span></span>|<span data-ttu-id="a0daf-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a0daf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0daf-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a0daf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0daf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a0daf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0daf-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0daf-150">This property is read-only.</span></span> <span data-ttu-id="a0daf-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0daf-152">createdDateTime</span></span>|<span data-ttu-id="a0daf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0daf-153">DateTimeOffset</span></span>|<span data-ttu-id="a0daf-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a0daf-154">DateTime the object was created.</span></span> <span data-ttu-id="a0daf-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-156">description</span><span class="sxs-lookup"><span data-stu-id="a0daf-156">description</span></span>|<span data-ttu-id="a0daf-157">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-157">String</span></span>|<span data-ttu-id="a0daf-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0daf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0daf-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a0daf-160">displayName</span></span>|<span data-ttu-id="a0daf-161">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-161">String</span></span>|<span data-ttu-id="a0daf-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0daf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0daf-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-164">version</span><span class="sxs-lookup"><span data-stu-id="a0daf-164">version</span></span>|<span data-ttu-id="a0daf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a0daf-165">Int32</span></span>|<span data-ttu-id="a0daf-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0daf-166">Version of the device configuration.</span></span> <span data-ttu-id="a0daf-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0daf-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a0daf-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a0daf-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a0daf-169">Int32</span></span>|<span data-ttu-id="a0daf-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="a0daf-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a0daf-171">Válido valores de 1 a 99 Inherited de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0daf-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a0daf-172">subjectNameFormat</span></span>|[<span data-ttu-id="a0daf-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a0daf-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="a0daf-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0daf-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="a0daf-175">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0daf-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="a0daf-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="a0daf-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="a0daf-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a0daf-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a0daf-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a0daf-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a0daf-179">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0daf-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="a0daf-180">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0daf-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="a0daf-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a0daf-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a0daf-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a0daf-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a0daf-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a0daf-183">Int32</span></span>|<span data-ttu-id="a0daf-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0daf-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a0daf-185">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0daf-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0daf-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a0daf-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a0daf-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a0daf-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a0daf-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0daf-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a0daf-189">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0daf-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="a0daf-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a0daf-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a0daf-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="a0daf-191">certificationAuthority</span></span>|<span data-ttu-id="a0daf-192">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-192">String</span></span>|<span data-ttu-id="a0daf-193">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="a0daf-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="a0daf-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="a0daf-194">certificationAuthorityName</span></span>|<span data-ttu-id="a0daf-195">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-195">String</span></span>|<span data-ttu-id="a0daf-196">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="a0daf-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="a0daf-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="a0daf-197">certificateTemplateName</span></span>|<span data-ttu-id="a0daf-198">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-198">String</span></span>|<span data-ttu-id="a0daf-199">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="a0daf-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="a0daf-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a0daf-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a0daf-201">String</span><span class="sxs-lookup"><span data-stu-id="a0daf-201">String</span></span>|<span data-ttu-id="a0daf-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="a0daf-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a0daf-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0daf-203">Response</span></span>
<span data-ttu-id="a0daf-204">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0daf-204">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0daf-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0daf-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0daf-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0daf-206">Request</span></span>
<span data-ttu-id="a0daf-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0daf-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 825

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="a0daf-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0daf-208">Response</span></span>
<span data-ttu-id="a0daf-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0daf-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





