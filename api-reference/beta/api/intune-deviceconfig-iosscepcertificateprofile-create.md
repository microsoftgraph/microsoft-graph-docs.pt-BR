---
title: Criar iosScepCertificateProfile
description: Criar um novo objeto iosScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63080a27eb5fb504ae5c9f336e596b5b363c1192
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963685"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="81ee8-103">Criar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="81ee8-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="81ee8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81ee8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81ee8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81ee8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ee8-106">Criar um novo objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="81ee8-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ee8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81ee8-107">Prerequisites</span></span>
<span data-ttu-id="81ee8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ee8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81ee8-110">Permission type</span></span>|<span data-ttu-id="81ee8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81ee8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ee8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81ee8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81ee8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81ee8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81ee8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81ee8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ee8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81ee8-115">Not supported.</span></span>|
|<span data-ttu-id="81ee8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81ee8-116">Application</span></span>|<span data-ttu-id="81ee8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81ee8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ee8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81ee8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="81ee8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81ee8-119">Request headers</span></span>
|<span data-ttu-id="81ee8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81ee8-120">Header</span></span>|<span data-ttu-id="81ee8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81ee8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81ee8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81ee8-122">Authorization</span></span>|<span data-ttu-id="81ee8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81ee8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81ee8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81ee8-124">Accept</span></span>|<span data-ttu-id="81ee8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81ee8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ee8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81ee8-126">Request body</span></span>
<span data-ttu-id="81ee8-127">No corpo da solicitação, forneça uma representação JSON do objeto iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="81ee8-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="81ee8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="81ee8-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="81ee8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81ee8-129">Property</span></span>|<span data-ttu-id="81ee8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="81ee8-130">Type</span></span>|<span data-ttu-id="81ee8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ee8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ee8-132">id</span><span class="sxs-lookup"><span data-stu-id="81ee8-132">id</span></span>|<span data-ttu-id="81ee8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81ee8-133">String</span></span>|<span data-ttu-id="81ee8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="81ee8-134">Key of the entity.</span></span> <span data-ttu-id="81ee8-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81ee8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="81ee8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ee8-137">DateTimeOffset</span></span>|<span data-ttu-id="81ee8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="81ee8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="81ee8-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81ee8-140">roleScopeTagIds</span></span>|<span data-ttu-id="81ee8-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="81ee8-141">String collection</span></span>|<span data-ttu-id="81ee8-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="81ee8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="81ee8-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="81ee8-144">supportsScopeTags</span></span>|<span data-ttu-id="81ee8-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="81ee8-145">Boolean</span></span>|<span data-ttu-id="81ee8-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="81ee8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="81ee8-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="81ee8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="81ee8-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="81ee8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="81ee8-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81ee8-149">This property is read-only.</span></span> <span data-ttu-id="81ee8-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="81ee8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="81ee8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="81ee8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="81ee8-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="81ee8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="81ee8-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="81ee8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="81ee8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="81ee8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="81ee8-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="81ee8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="81ee8-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="81ee8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="81ee8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="81ee8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="81ee8-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="81ee8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="81ee8-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81ee8-163">createdDateTime</span></span>|<span data-ttu-id="81ee8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ee8-164">DateTimeOffset</span></span>|<span data-ttu-id="81ee8-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="81ee8-165">DateTime the object was created.</span></span> <span data-ttu-id="81ee8-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-167">descrição</span><span class="sxs-lookup"><span data-stu-id="81ee8-167">description</span></span>|<span data-ttu-id="81ee8-168">String</span><span class="sxs-lookup"><span data-stu-id="81ee8-168">String</span></span>|<span data-ttu-id="81ee8-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81ee8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="81ee8-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="81ee8-171">displayName</span></span>|<span data-ttu-id="81ee8-172">String</span><span class="sxs-lookup"><span data-stu-id="81ee8-172">String</span></span>|<span data-ttu-id="81ee8-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81ee8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="81ee8-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-175">versão</span><span class="sxs-lookup"><span data-stu-id="81ee8-175">version</span></span>|<span data-ttu-id="81ee8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="81ee8-176">Int32</span></span>|<span data-ttu-id="81ee8-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81ee8-177">Version of the device configuration.</span></span> <span data-ttu-id="81ee8-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81ee8-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="81ee8-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="81ee8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="81ee8-180">Int32</span></span>|<span data-ttu-id="81ee8-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="81ee8-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="81ee8-182">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="81ee8-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="81ee8-183">subjectNameFormat</span></span>|[<span data-ttu-id="81ee8-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="81ee8-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="81ee8-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="81ee8-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="81ee8-186">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="81ee8-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="81ee8-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="81ee8-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="81ee8-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="81ee8-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="81ee8-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="81ee8-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="81ee8-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="81ee8-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="81ee8-191">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="81ee8-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="81ee8-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="81ee8-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="81ee8-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="81ee8-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="81ee8-194">Int32</span><span class="sxs-lookup"><span data-stu-id="81ee8-194">Int32</span></span>|<span data-ttu-id="81ee8-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="81ee8-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="81ee8-196">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="81ee8-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="81ee8-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="81ee8-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="81ee8-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="81ee8-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="81ee8-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="81ee8-200">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="81ee8-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="81ee8-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="81ee8-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="81ee8-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="81ee8-202">scepServerUrls</span></span>|<span data-ttu-id="81ee8-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="81ee8-203">String collection</span></span>|<span data-ttu-id="81ee8-204">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="81ee8-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="81ee8-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="81ee8-205">subjectNameFormatString</span></span>|<span data-ttu-id="81ee8-206">String</span><span class="sxs-lookup"><span data-stu-id="81ee8-206">String</span></span>|<span data-ttu-id="81ee8-207">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="81ee8-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="81ee8-208">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="81ee8-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="81ee8-209">uso de</span><span class="sxs-lookup"><span data-stu-id="81ee8-209">keyUsage</span></span>|[<span data-ttu-id="81ee8-210">usos de</span><span class="sxs-lookup"><span data-stu-id="81ee8-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="81ee8-211">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="81ee8-211">SCEP Key Usage.</span></span> <span data-ttu-id="81ee8-212">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="81ee8-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="81ee8-213">keySize</span><span class="sxs-lookup"><span data-stu-id="81ee8-213">keySize</span></span>|[<span data-ttu-id="81ee8-214">keySize</span><span class="sxs-lookup"><span data-stu-id="81ee8-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="81ee8-215">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="81ee8-215">SCEP Key Size.</span></span> <span data-ttu-id="81ee8-216">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="81ee8-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="81ee8-217">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="81ee8-217">extendedKeyUsages</span></span>|<span data-ttu-id="81ee8-218">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="81ee8-219">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="81ee8-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="81ee8-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81ee8-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="81ee8-221">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="81ee8-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="81ee8-222">String</span><span class="sxs-lookup"><span data-stu-id="81ee8-222">String</span></span>|<span data-ttu-id="81ee8-223">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="81ee8-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="81ee8-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="81ee8-224">certificateStore</span></span>|[<span data-ttu-id="81ee8-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="81ee8-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="81ee8-226">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="81ee8-226">Target store certificate.</span></span> <span data-ttu-id="81ee8-227">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="81ee8-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="81ee8-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="81ee8-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="81ee8-229">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="81ee8-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="81ee8-230">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="81ee8-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="81ee8-231">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81ee8-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="81ee8-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ee8-232">Response</span></span>
<span data-ttu-id="81ee8-233">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81ee8-233">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ee8-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81ee8-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="81ee8-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81ee8-235">Request</span></span>
<span data-ttu-id="81ee8-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81ee8-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="81ee8-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ee8-237">Response</span></span>
<span data-ttu-id="81ee8-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81ee8-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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





