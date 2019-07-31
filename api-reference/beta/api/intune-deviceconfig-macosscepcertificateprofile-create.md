---
title: Criar macOSScepCertificateProfile
description: Criar um novo objeto macOSScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c42c15d5b6dc6c5b7dc3edc0cb472298a91576d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947113"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="58f01-103">Criar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="58f01-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="58f01-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58f01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58f01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58f01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58f01-106">Criar um novo objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="58f01-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58f01-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58f01-107">Prerequisites</span></span>
<span data-ttu-id="58f01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f01-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58f01-110">Permission type</span></span>|<span data-ttu-id="58f01-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58f01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58f01-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58f01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58f01-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58f01-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58f01-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58f01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58f01-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58f01-115">Not supported.</span></span>|
|<span data-ttu-id="58f01-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58f01-116">Application</span></span>|<span data-ttu-id="58f01-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58f01-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58f01-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58f01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="58f01-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58f01-119">Request headers</span></span>
|<span data-ttu-id="58f01-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58f01-120">Header</span></span>|<span data-ttu-id="58f01-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58f01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58f01-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58f01-122">Authorization</span></span>|<span data-ttu-id="58f01-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58f01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58f01-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58f01-124">Accept</span></span>|<span data-ttu-id="58f01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58f01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f01-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58f01-126">Request body</span></span>
<span data-ttu-id="58f01-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="58f01-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="58f01-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="58f01-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="58f01-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58f01-129">Property</span></span>|<span data-ttu-id="58f01-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58f01-130">Type</span></span>|<span data-ttu-id="58f01-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f01-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58f01-132">id</span><span class="sxs-lookup"><span data-stu-id="58f01-132">id</span></span>|<span data-ttu-id="58f01-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58f01-133">String</span></span>|<span data-ttu-id="58f01-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="58f01-134">Key of the entity.</span></span> <span data-ttu-id="58f01-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58f01-136">lastModifiedDateTime</span></span>|<span data-ttu-id="58f01-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58f01-137">DateTimeOffset</span></span>|<span data-ttu-id="58f01-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="58f01-138">DateTime the object was last modified.</span></span> <span data-ttu-id="58f01-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58f01-140">roleScopeTagIds</span></span>|<span data-ttu-id="58f01-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="58f01-141">String collection</span></span>|<span data-ttu-id="58f01-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="58f01-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58f01-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="58f01-144">supportsScopeTags</span></span>|<span data-ttu-id="58f01-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="58f01-145">Boolean</span></span>|<span data-ttu-id="58f01-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="58f01-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58f01-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="58f01-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58f01-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="58f01-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58f01-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58f01-149">This property is read-only.</span></span> <span data-ttu-id="58f01-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="58f01-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="58f01-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="58f01-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="58f01-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="58f01-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="58f01-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="58f01-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="58f01-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="58f01-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="58f01-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="58f01-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="58f01-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="58f01-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="58f01-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="58f01-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="58f01-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="58f01-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="58f01-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58f01-163">createdDateTime</span></span>|<span data-ttu-id="58f01-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58f01-164">DateTimeOffset</span></span>|<span data-ttu-id="58f01-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="58f01-165">DateTime the object was created.</span></span> <span data-ttu-id="58f01-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-167">descrição</span><span class="sxs-lookup"><span data-stu-id="58f01-167">description</span></span>|<span data-ttu-id="58f01-168">String</span><span class="sxs-lookup"><span data-stu-id="58f01-168">String</span></span>|<span data-ttu-id="58f01-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58f01-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58f01-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-171">displayName</span><span class="sxs-lookup"><span data-stu-id="58f01-171">displayName</span></span>|<span data-ttu-id="58f01-172">String</span><span class="sxs-lookup"><span data-stu-id="58f01-172">String</span></span>|<span data-ttu-id="58f01-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58f01-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58f01-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-175">versão</span><span class="sxs-lookup"><span data-stu-id="58f01-175">version</span></span>|<span data-ttu-id="58f01-176">Int32</span><span class="sxs-lookup"><span data-stu-id="58f01-176">Int32</span></span>|<span data-ttu-id="58f01-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58f01-177">Version of the device configuration.</span></span> <span data-ttu-id="58f01-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58f01-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="58f01-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="58f01-180">Int32</span><span class="sxs-lookup"><span data-stu-id="58f01-180">Int32</span></span>|<span data-ttu-id="58f01-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="58f01-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="58f01-182">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="58f01-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="58f01-183">subjectNameFormat</span></span>|[<span data-ttu-id="58f01-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="58f01-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="58f01-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="58f01-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="58f01-186">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58f01-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="58f01-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="58f01-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="58f01-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="58f01-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="58f01-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="58f01-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="58f01-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="58f01-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="58f01-191">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58f01-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="58f01-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="58f01-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="58f01-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="58f01-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="58f01-194">Int32</span><span class="sxs-lookup"><span data-stu-id="58f01-194">Int32</span></span>|<span data-ttu-id="58f01-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="58f01-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="58f01-196">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="58f01-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="58f01-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="58f01-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="58f01-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="58f01-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="58f01-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="58f01-200">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58f01-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="58f01-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="58f01-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="58f01-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="58f01-202">scepServerUrls</span></span>|<span data-ttu-id="58f01-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="58f01-203">String collection</span></span>|<span data-ttu-id="58f01-204">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="58f01-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="58f01-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="58f01-205">subjectNameFormatString</span></span>|<span data-ttu-id="58f01-206">String</span><span class="sxs-lookup"><span data-stu-id="58f01-206">String</span></span>|<span data-ttu-id="58f01-207">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="58f01-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="58f01-208">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="58f01-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="58f01-209">uso de</span><span class="sxs-lookup"><span data-stu-id="58f01-209">keyUsage</span></span>|[<span data-ttu-id="58f01-210">usos de</span><span class="sxs-lookup"><span data-stu-id="58f01-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="58f01-211">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="58f01-211">SCEP Key Usage.</span></span> <span data-ttu-id="58f01-212">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="58f01-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="58f01-213">keySize</span><span class="sxs-lookup"><span data-stu-id="58f01-213">keySize</span></span>|[<span data-ttu-id="58f01-214">keySize</span><span class="sxs-lookup"><span data-stu-id="58f01-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="58f01-215">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="58f01-215">SCEP Key Size.</span></span> <span data-ttu-id="58f01-216">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="58f01-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="58f01-217">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="58f01-217">hashAlgorithm</span></span>|[<span data-ttu-id="58f01-218">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="58f01-218">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="58f01-219">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="58f01-219">SCEP Hash Algorithm.</span></span> <span data-ttu-id="58f01-220">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="58f01-220">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="58f01-221">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="58f01-221">extendedKeyUsages</span></span>|<span data-ttu-id="58f01-222">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="58f01-223">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="58f01-223">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="58f01-224">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="58f01-224">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="58f01-225">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="58f01-225">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="58f01-226">String</span><span class="sxs-lookup"><span data-stu-id="58f01-226">String</span></span>|<span data-ttu-id="58f01-227">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="58f01-227">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="58f01-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="58f01-228">certificateStore</span></span>|[<span data-ttu-id="58f01-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="58f01-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="58f01-230">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="58f01-230">Target store certificate.</span></span> <span data-ttu-id="58f01-231">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="58f01-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="58f01-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="58f01-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="58f01-233">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="58f01-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="58f01-234">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="58f01-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="58f01-235">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="58f01-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="58f01-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="58f01-236">Response</span></span>
<span data-ttu-id="58f01-237">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58f01-237">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58f01-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58f01-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="58f01-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58f01-239">Request</span></span>
<span data-ttu-id="58f01-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58f01-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1962

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="58f01-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="58f01-241">Response</span></span>
<span data-ttu-id="58f01-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58f01-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2134

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```





