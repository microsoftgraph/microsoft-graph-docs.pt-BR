---
title: Atualizar iosPkcsCertificateProfile
description: Atualiza as propriedades de um objeto iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c33d5beb2220ae9c60027ebb5cd0ecbc1b19a6ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174661"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="37c17-103">Atualizar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="37c17-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="37c17-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37c17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37c17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37c17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37c17-106">Atualiza as propriedades de um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="37c17-106">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37c17-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37c17-107">Prerequisites</span></span>
<span data-ttu-id="37c17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="37c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37c17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37c17-110">Permission type</span></span>|<span data-ttu-id="37c17-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37c17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37c17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37c17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37c17-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c17-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37c17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37c17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37c17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c17-115">Not supported.</span></span>|
|<span data-ttu-id="37c17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37c17-116">Application</span></span>|<span data-ttu-id="37c17-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37c17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37c17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="37c17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37c17-119">Request headers</span></span>
|<span data-ttu-id="37c17-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37c17-120">Header</span></span>|<span data-ttu-id="37c17-121">Valor</span><span class="sxs-lookup"><span data-stu-id="37c17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37c17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37c17-122">Authorization</span></span>|<span data-ttu-id="37c17-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37c17-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37c17-124">Accept</span></span>|<span data-ttu-id="37c17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37c17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37c17-126">Request body</span></span>
<span data-ttu-id="37c17-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="37c17-127">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="37c17-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="37c17-128">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="37c17-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37c17-129">Property</span></span>|<span data-ttu-id="37c17-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37c17-130">Type</span></span>|<span data-ttu-id="37c17-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c17-132">id</span><span class="sxs-lookup"><span data-stu-id="37c17-132">id</span></span>|<span data-ttu-id="37c17-133">String</span><span class="sxs-lookup"><span data-stu-id="37c17-133">String</span></span>|<span data-ttu-id="37c17-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37c17-134">Key of the entity.</span></span> <span data-ttu-id="37c17-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37c17-136">lastModifiedDateTime</span></span>|<span data-ttu-id="37c17-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c17-137">DateTimeOffset</span></span>|<span data-ttu-id="37c17-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="37c17-138">DateTime the object was last modified.</span></span> <span data-ttu-id="37c17-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37c17-140">roleScopeTagIds</span></span>|<span data-ttu-id="37c17-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37c17-141">String collection</span></span>|<span data-ttu-id="37c17-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="37c17-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37c17-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37c17-144">supportsScopeTags</span></span>|<span data-ttu-id="37c17-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="37c17-145">Boolean</span></span>|<span data-ttu-id="37c17-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="37c17-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37c17-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="37c17-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37c17-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="37c17-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37c17-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c17-149">This property is read-only.</span></span> <span data-ttu-id="37c17-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37c17-151">createdDateTime</span></span>|<span data-ttu-id="37c17-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c17-152">DateTimeOffset</span></span>|<span data-ttu-id="37c17-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="37c17-153">DateTime the object was created.</span></span> <span data-ttu-id="37c17-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-155">description</span><span class="sxs-lookup"><span data-stu-id="37c17-155">description</span></span>|<span data-ttu-id="37c17-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37c17-156">String</span></span>|<span data-ttu-id="37c17-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37c17-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37c17-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-159">displayName</span><span class="sxs-lookup"><span data-stu-id="37c17-159">displayName</span></span>|<span data-ttu-id="37c17-160">String</span><span class="sxs-lookup"><span data-stu-id="37c17-160">String</span></span>|<span data-ttu-id="37c17-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37c17-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37c17-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-163">version</span><span class="sxs-lookup"><span data-stu-id="37c17-163">version</span></span>|<span data-ttu-id="37c17-164">Int32</span><span class="sxs-lookup"><span data-stu-id="37c17-164">Int32</span></span>|<span data-ttu-id="37c17-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37c17-165">Version of the device configuration.</span></span> <span data-ttu-id="37c17-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c17-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="37c17-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="37c17-168">Int32</span><span class="sxs-lookup"><span data-stu-id="37c17-168">Int32</span></span>|<span data-ttu-id="37c17-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="37c17-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="37c17-170">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="37c17-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="37c17-171">subjectNameFormat</span></span>|[<span data-ttu-id="37c17-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="37c17-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="37c17-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="37c17-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="37c17-174">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="37c17-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="37c17-175">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="37c17-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="37c17-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="37c17-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="37c17-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="37c17-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="37c17-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="37c17-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="37c17-179">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="37c17-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="37c17-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="37c17-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="37c17-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="37c17-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="37c17-182">Int32</span><span class="sxs-lookup"><span data-stu-id="37c17-182">Int32</span></span>|<span data-ttu-id="37c17-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="37c17-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="37c17-184">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="37c17-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="37c17-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="37c17-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="37c17-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="37c17-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="37c17-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="37c17-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="37c17-188">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="37c17-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="37c17-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="37c17-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="37c17-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="37c17-190">certificationAuthority</span></span>|<span data-ttu-id="37c17-191">String</span><span class="sxs-lookup"><span data-stu-id="37c17-191">String</span></span>|<span data-ttu-id="37c17-192">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="37c17-192">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="37c17-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="37c17-193">certificationAuthorityName</span></span>|<span data-ttu-id="37c17-194">String</span><span class="sxs-lookup"><span data-stu-id="37c17-194">String</span></span>|<span data-ttu-id="37c17-195">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="37c17-195">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="37c17-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="37c17-196">certificateTemplateName</span></span>|<span data-ttu-id="37c17-197">String</span><span class="sxs-lookup"><span data-stu-id="37c17-197">String</span></span>|<span data-ttu-id="37c17-198">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="37c17-198">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="37c17-199">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="37c17-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="37c17-200">String</span><span class="sxs-lookup"><span data-stu-id="37c17-200">String</span></span>|<span data-ttu-id="37c17-201">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="37c17-201">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="37c17-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c17-202">Response</span></span>
<span data-ttu-id="37c17-203">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37c17-203">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37c17-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37c17-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="37c17-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37c17-205">Request</span></span>
<span data-ttu-id="37c17-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37c17-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="37c17-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c17-207">Response</span></span>
<span data-ttu-id="37c17-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37c17-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




