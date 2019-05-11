---
title: Criar windows81SCEPCertificateProfile
description: Criar um novo objeto windows81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74498b693f98a47211d3c7222e58e5473258ac84
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918231"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="be4bb-103">Criar windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="be4bb-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="be4bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be4bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be4bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be4bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be4bb-106">Criar um novo objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="be4bb-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be4bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be4bb-107">Prerequisites</span></span>
<span data-ttu-id="be4bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be4bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be4bb-110">Permission type</span></span>|<span data-ttu-id="be4bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be4bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be4bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be4bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be4bb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4bb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be4bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be4bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be4bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be4bb-115">Not supported.</span></span>|
|<span data-ttu-id="be4bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be4bb-116">Application</span></span>|<span data-ttu-id="be4bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be4bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be4bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be4bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="be4bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be4bb-119">Request headers</span></span>
|<span data-ttu-id="be4bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be4bb-120">Header</span></span>|<span data-ttu-id="be4bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="be4bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be4bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="be4bb-122">Authorization</span></span>|<span data-ttu-id="be4bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be4bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be4bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be4bb-124">Accept</span></span>|<span data-ttu-id="be4bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be4bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be4bb-126">Request body</span></span>
<span data-ttu-id="be4bb-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="be4bb-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="be4bb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="be4bb-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="be4bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be4bb-129">Property</span></span>|<span data-ttu-id="be4bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="be4bb-130">Type</span></span>|<span data-ttu-id="be4bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be4bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4bb-132">id</span><span class="sxs-lookup"><span data-stu-id="be4bb-132">id</span></span>|<span data-ttu-id="be4bb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4bb-133">String</span></span>|<span data-ttu-id="be4bb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="be4bb-134">Key of the entity.</span></span> <span data-ttu-id="be4bb-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be4bb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="be4bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4bb-137">DateTimeOffset</span></span>|<span data-ttu-id="be4bb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="be4bb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="be4bb-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be4bb-140">roleScopeTagIds</span></span>|<span data-ttu-id="be4bb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4bb-141">String collection</span></span>|<span data-ttu-id="be4bb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="be4bb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="be4bb-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="be4bb-144">supportsScopeTags</span></span>|<span data-ttu-id="be4bb-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="be4bb-145">Boolean</span></span>|<span data-ttu-id="be4bb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="be4bb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="be4bb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="be4bb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="be4bb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="be4bb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="be4bb-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be4bb-149">This property is read-only.</span></span> <span data-ttu-id="be4bb-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be4bb-151">createdDateTime</span></span>|<span data-ttu-id="be4bb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4bb-152">DateTimeOffset</span></span>|<span data-ttu-id="be4bb-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="be4bb-153">DateTime the object was created.</span></span> <span data-ttu-id="be4bb-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-155">description</span><span class="sxs-lookup"><span data-stu-id="be4bb-155">description</span></span>|<span data-ttu-id="be4bb-156">String</span><span class="sxs-lookup"><span data-stu-id="be4bb-156">String</span></span>|<span data-ttu-id="be4bb-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be4bb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be4bb-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="be4bb-159">displayName</span></span>|<span data-ttu-id="be4bb-160">String</span><span class="sxs-lookup"><span data-stu-id="be4bb-160">String</span></span>|<span data-ttu-id="be4bb-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be4bb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be4bb-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-163">versão</span><span class="sxs-lookup"><span data-stu-id="be4bb-163">version</span></span>|<span data-ttu-id="be4bb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="be4bb-164">Int32</span></span>|<span data-ttu-id="be4bb-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be4bb-165">Version of the device configuration.</span></span> <span data-ttu-id="be4bb-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be4bb-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="be4bb-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="be4bb-168">Int32</span><span class="sxs-lookup"><span data-stu-id="be4bb-168">Int32</span></span>|<span data-ttu-id="be4bb-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="be4bb-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="be4bb-170">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="be4bb-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="be4bb-171">keyStorageProvider</span></span>|[<span data-ttu-id="be4bb-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="be4bb-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="be4bb-173">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be4bb-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="be4bb-174">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="be4bb-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="be4bb-175">subjectNameFormat</span></span>|[<span data-ttu-id="be4bb-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="be4bb-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="be4bb-177">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be4bb-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="be4bb-178">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="be4bb-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="be4bb-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="be4bb-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="be4bb-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="be4bb-181">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be4bb-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="be4bb-182">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="be4bb-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="be4bb-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="be4bb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="be4bb-184">Int32</span></span>|<span data-ttu-id="be4bb-185">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="be4bb-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="be4bb-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="be4bb-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="be4bb-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="be4bb-188">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be4bb-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="be4bb-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="be4bb-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="be4bb-190">extendedKeyUsages</span></span>|<span data-ttu-id="be4bb-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="be4bb-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="be4bb-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="be4bb-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="be4bb-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="be4bb-194">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-194">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="be4bb-195">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="be4bb-195">customSubjectAlternativeNames</span></span>|<span data-ttu-id="be4bb-196">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="be4bb-197">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="be4bb-197">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="be4bb-198">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="be4bb-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="be4bb-199">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be4bb-199">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="be4bb-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="be4bb-200">scepServerUrls</span></span>|<span data-ttu-id="be4bb-201">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4bb-201">String collection</span></span>|<span data-ttu-id="be4bb-202">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="be4bb-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="be4bb-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="be4bb-203">subjectNameFormatString</span></span>|<span data-ttu-id="be4bb-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4bb-204">String</span></span>|<span data-ttu-id="be4bb-205">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="be4bb-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="be4bb-206">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="be4bb-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="be4bb-207">uso de</span><span class="sxs-lookup"><span data-stu-id="be4bb-207">keyUsage</span></span>|[<span data-ttu-id="be4bb-208">usos de</span><span class="sxs-lookup"><span data-stu-id="be4bb-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="be4bb-209">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="be4bb-209">SCEP Key Usage.</span></span> <span data-ttu-id="be4bb-210">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="be4bb-211">keySize</span><span class="sxs-lookup"><span data-stu-id="be4bb-211">keySize</span></span>|[<span data-ttu-id="be4bb-212">keySize</span><span class="sxs-lookup"><span data-stu-id="be4bb-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="be4bb-213">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="be4bb-213">SCEP Key Size.</span></span> <span data-ttu-id="be4bb-214">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="be4bb-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="be4bb-215">hashAlgorithm</span></span>|[<span data-ttu-id="be4bb-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="be4bb-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="be4bb-217">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="be4bb-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="be4bb-218">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="be4bb-219">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="be4bb-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="be4bb-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4bb-220">String</span></span>|<span data-ttu-id="be4bb-221">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="be4bb-221">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="be4bb-222">certificateStore</span><span class="sxs-lookup"><span data-stu-id="be4bb-222">certificateStore</span></span>|[<span data-ttu-id="be4bb-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="be4bb-223">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="be4bb-224">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="be4bb-224">Target store certificate.</span></span> <span data-ttu-id="be4bb-225">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="be4bb-225">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="be4bb-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="be4bb-226">Response</span></span>
<span data-ttu-id="be4bb-227">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be4bb-227">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be4bb-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be4bb-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="be4bb-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be4bb-229">Request</span></span>
<span data-ttu-id="be4bb-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be4bb-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1251

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="be4bb-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="be4bb-231">Response</span></span>
<span data-ttu-id="be4bb-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be4bb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```




