---
title: Criar iosPkcsCertificateProfile
description: Criar um novo objeto iosPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a271bfa68f84a41819c011f9acca27d9b183b2d3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37167540"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="1fafc-103">Criar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="1fafc-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="1fafc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1fafc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fafc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fafc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fafc-106">Criar um novo objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1fafc-106">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fafc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fafc-107">Prerequisites</span></span>
<span data-ttu-id="1fafc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fafc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fafc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fafc-110">Permission type</span></span>|<span data-ttu-id="1fafc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fafc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fafc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fafc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fafc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fafc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fafc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fafc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fafc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fafc-115">Not supported.</span></span>|
|<span data-ttu-id="1fafc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fafc-116">Application</span></span>|<span data-ttu-id="1fafc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fafc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fafc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fafc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1fafc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fafc-119">Request headers</span></span>
|<span data-ttu-id="1fafc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1fafc-120">Header</span></span>|<span data-ttu-id="1fafc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1fafc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fafc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fafc-122">Authorization</span></span>|<span data-ttu-id="1fafc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fafc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fafc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1fafc-124">Accept</span></span>|<span data-ttu-id="1fafc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fafc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fafc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fafc-126">Request body</span></span>
<span data-ttu-id="1fafc-127">No corpo da solicitação, forneça uma representação JSON do objeto iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1fafc-127">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="1fafc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1fafc-128">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="1fafc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fafc-129">Property</span></span>|<span data-ttu-id="1fafc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fafc-130">Type</span></span>|<span data-ttu-id="1fafc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fafc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fafc-132">id</span><span class="sxs-lookup"><span data-stu-id="1fafc-132">id</span></span>|<span data-ttu-id="1fafc-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fafc-133">String</span></span>|<span data-ttu-id="1fafc-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1fafc-134">Key of the entity.</span></span> <span data-ttu-id="1fafc-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fafc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1fafc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fafc-137">DateTimeOffset</span></span>|<span data-ttu-id="1fafc-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1fafc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1fafc-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1fafc-140">roleScopeTagIds</span></span>|<span data-ttu-id="1fafc-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fafc-141">String collection</span></span>|<span data-ttu-id="1fafc-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1fafc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1fafc-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1fafc-144">supportsScopeTags</span></span>|<span data-ttu-id="1fafc-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fafc-145">Boolean</span></span>|<span data-ttu-id="1fafc-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1fafc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1fafc-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1fafc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1fafc-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1fafc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1fafc-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1fafc-149">This property is read-only.</span></span> <span data-ttu-id="1fafc-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1fafc-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1fafc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1fafc-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1fafc-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="1fafc-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1fafc-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1fafc-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1fafc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1fafc-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1fafc-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="1fafc-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1fafc-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1fafc-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1fafc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1fafc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1fafc-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="1fafc-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1fafc-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1fafc-163">createdDateTime</span></span>|<span data-ttu-id="1fafc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fafc-164">DateTimeOffset</span></span>|<span data-ttu-id="1fafc-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1fafc-165">DateTime the object was created.</span></span> <span data-ttu-id="1fafc-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-167">descrição</span><span class="sxs-lookup"><span data-stu-id="1fafc-167">description</span></span>|<span data-ttu-id="1fafc-168">String</span><span class="sxs-lookup"><span data-stu-id="1fafc-168">String</span></span>|<span data-ttu-id="1fafc-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fafc-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1fafc-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1fafc-171">displayName</span></span>|<span data-ttu-id="1fafc-172">String</span><span class="sxs-lookup"><span data-stu-id="1fafc-172">String</span></span>|<span data-ttu-id="1fafc-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fafc-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1fafc-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-175">versão</span><span class="sxs-lookup"><span data-stu-id="1fafc-175">version</span></span>|<span data-ttu-id="1fafc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1fafc-176">Int32</span></span>|<span data-ttu-id="1fafc-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fafc-177">Version of the device configuration.</span></span> <span data-ttu-id="1fafc-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fafc-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1fafc-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="1fafc-180">Int32</span><span class="sxs-lookup"><span data-stu-id="1fafc-180">Int32</span></span>|<span data-ttu-id="1fafc-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="1fafc-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1fafc-182">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1fafc-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1fafc-183">subjectNameFormat</span></span>|[<span data-ttu-id="1fafc-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1fafc-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="1fafc-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="1fafc-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="1fafc-186">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1fafc-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="1fafc-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="1fafc-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="1fafc-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1fafc-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1fafc-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1fafc-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1fafc-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="1fafc-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="1fafc-191">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1fafc-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="1fafc-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="1fafc-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1fafc-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1fafc-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1fafc-194">Int32</span><span class="sxs-lookup"><span data-stu-id="1fafc-194">Int32</span></span>|<span data-ttu-id="1fafc-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="1fafc-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="1fafc-196">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1fafc-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1fafc-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1fafc-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1fafc-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1fafc-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1fafc-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="1fafc-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1fafc-200">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1fafc-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="1fafc-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="1fafc-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1fafc-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="1fafc-202">certificationAuthority</span></span>|<span data-ttu-id="1fafc-203">String</span><span class="sxs-lookup"><span data-stu-id="1fafc-203">String</span></span>|<span data-ttu-id="1fafc-204">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="1fafc-204">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="1fafc-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="1fafc-205">certificationAuthorityName</span></span>|<span data-ttu-id="1fafc-206">String</span><span class="sxs-lookup"><span data-stu-id="1fafc-206">String</span></span>|<span data-ttu-id="1fafc-207">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="1fafc-207">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="1fafc-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="1fafc-208">certificateTemplateName</span></span>|<span data-ttu-id="1fafc-209">String</span><span class="sxs-lookup"><span data-stu-id="1fafc-209">String</span></span>|<span data-ttu-id="1fafc-210">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="1fafc-210">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="1fafc-211">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="1fafc-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="1fafc-212">String</span><span class="sxs-lookup"><span data-stu-id="1fafc-212">String</span></span>|<span data-ttu-id="1fafc-213">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="1fafc-213">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="1fafc-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fafc-214">Response</span></span>
<span data-ttu-id="1fafc-215">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fafc-215">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fafc-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fafc-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fafc-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fafc-217">Request</span></span>
<span data-ttu-id="1fafc-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fafc-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1534

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="1fafc-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fafc-219">Response</span></span>
<span data-ttu-id="1fafc-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fafc-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1706

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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




