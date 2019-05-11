---
title: Criar windows10PkcsCertificateProfile
description: Criar um novo objeto windows10PkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eca0bc52b4bccb2e6e572f6b7db15949cd5748fc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918525"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="407cd-103">Criar windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="407cd-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="407cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="407cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="407cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="407cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="407cd-106">Criar um novo objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="407cd-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="407cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="407cd-107">Prerequisites</span></span>
<span data-ttu-id="407cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="407cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="407cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="407cd-110">Permission type</span></span>|<span data-ttu-id="407cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="407cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="407cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="407cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="407cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="407cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="407cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="407cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="407cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="407cd-115">Not supported.</span></span>|
|<span data-ttu-id="407cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="407cd-116">Application</span></span>|<span data-ttu-id="407cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="407cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="407cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="407cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="407cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="407cd-119">Request headers</span></span>
|<span data-ttu-id="407cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="407cd-120">Header</span></span>|<span data-ttu-id="407cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="407cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="407cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="407cd-122">Authorization</span></span>|<span data-ttu-id="407cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="407cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="407cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="407cd-124">Accept</span></span>|<span data-ttu-id="407cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="407cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="407cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="407cd-126">Request body</span></span>
<span data-ttu-id="407cd-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="407cd-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="407cd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="407cd-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="407cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="407cd-129">Property</span></span>|<span data-ttu-id="407cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="407cd-130">Type</span></span>|<span data-ttu-id="407cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="407cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="407cd-132">id</span><span class="sxs-lookup"><span data-stu-id="407cd-132">id</span></span>|<span data-ttu-id="407cd-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="407cd-133">String</span></span>|<span data-ttu-id="407cd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="407cd-134">Key of the entity.</span></span> <span data-ttu-id="407cd-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="407cd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="407cd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="407cd-137">DateTimeOffset</span></span>|<span data-ttu-id="407cd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="407cd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="407cd-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="407cd-140">roleScopeTagIds</span></span>|<span data-ttu-id="407cd-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="407cd-141">String collection</span></span>|<span data-ttu-id="407cd-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="407cd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="407cd-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="407cd-144">supportsScopeTags</span></span>|<span data-ttu-id="407cd-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="407cd-145">Boolean</span></span>|<span data-ttu-id="407cd-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="407cd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="407cd-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="407cd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="407cd-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="407cd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="407cd-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="407cd-149">This property is read-only.</span></span> <span data-ttu-id="407cd-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="407cd-151">createdDateTime</span></span>|<span data-ttu-id="407cd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="407cd-152">DateTimeOffset</span></span>|<span data-ttu-id="407cd-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="407cd-153">DateTime the object was created.</span></span> <span data-ttu-id="407cd-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-155">description</span><span class="sxs-lookup"><span data-stu-id="407cd-155">description</span></span>|<span data-ttu-id="407cd-156">String</span><span class="sxs-lookup"><span data-stu-id="407cd-156">String</span></span>|<span data-ttu-id="407cd-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="407cd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="407cd-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="407cd-159">displayName</span></span>|<span data-ttu-id="407cd-160">String</span><span class="sxs-lookup"><span data-stu-id="407cd-160">String</span></span>|<span data-ttu-id="407cd-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="407cd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="407cd-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-163">versão</span><span class="sxs-lookup"><span data-stu-id="407cd-163">version</span></span>|<span data-ttu-id="407cd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="407cd-164">Int32</span></span>|<span data-ttu-id="407cd-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="407cd-165">Version of the device configuration.</span></span> <span data-ttu-id="407cd-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="407cd-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="407cd-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="407cd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="407cd-168">Int32</span></span>|<span data-ttu-id="407cd-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="407cd-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="407cd-170">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="407cd-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="407cd-171">keyStorageProvider</span></span>|[<span data-ttu-id="407cd-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="407cd-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="407cd-173">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="407cd-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="407cd-174">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="407cd-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="407cd-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="407cd-175">subjectNameFormat</span></span>|[<span data-ttu-id="407cd-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="407cd-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="407cd-177">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="407cd-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="407cd-178">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="407cd-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="407cd-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="407cd-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="407cd-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="407cd-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="407cd-181">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="407cd-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="407cd-182">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="407cd-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="407cd-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="407cd-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="407cd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="407cd-184">Int32</span></span>|<span data-ttu-id="407cd-185">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="407cd-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="407cd-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="407cd-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="407cd-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="407cd-188">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="407cd-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="407cd-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="407cd-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="407cd-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="407cd-190">certificationAuthority</span></span>|<span data-ttu-id="407cd-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="407cd-191">String</span></span>|<span data-ttu-id="407cd-192">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="407cd-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="407cd-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="407cd-193">certificationAuthorityName</span></span>|<span data-ttu-id="407cd-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="407cd-194">String</span></span>|<span data-ttu-id="407cd-195">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="407cd-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="407cd-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="407cd-196">certificateTemplateName</span></span>|<span data-ttu-id="407cd-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="407cd-197">String</span></span>|<span data-ttu-id="407cd-198">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="407cd-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="407cd-199">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="407cd-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="407cd-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="407cd-200">String</span></span>|<span data-ttu-id="407cd-201">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="407cd-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="407cd-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="407cd-202">extendedKeyUsages</span></span>|<span data-ttu-id="407cd-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="407cd-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="407cd-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="407cd-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="407cd-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="407cd-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="407cd-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="407cd-206">Response</span></span>
<span data-ttu-id="407cd-207">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="407cd-207">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="407cd-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="407cd-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="407cd-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="407cd-209">Request</span></span>
<span data-ttu-id="407cd-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="407cd-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1011

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="407cd-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="407cd-211">Response</span></span>
<span data-ttu-id="407cd-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="407cd-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1183

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```




