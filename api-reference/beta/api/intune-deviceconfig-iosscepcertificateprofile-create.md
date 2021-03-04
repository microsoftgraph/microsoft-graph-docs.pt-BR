---
title: Criar iosScepCertificateProfile
description: Crie um novo objeto iosScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 297e2ca51b4df2735065d4ca556a8ba1d0c94ece
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441638"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="388c8-103">Criar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="388c8-103">Create iosScepCertificateProfile</span></span>

<span data-ttu-id="388c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="388c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="388c8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="388c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="388c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="388c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="388c8-107">Crie um novo [objeto iosScepCertificateProfile.](../resources/intune-deviceconfig-iosscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="388c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="388c8-108">Prerequisites</span></span>
<span data-ttu-id="388c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="388c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="388c8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="388c8-111">Permission type</span></span>|<span data-ttu-id="388c8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="388c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="388c8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="388c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="388c8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="388c8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="388c8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="388c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="388c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="388c8-116">Not supported.</span></span>|
|<span data-ttu-id="388c8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="388c8-117">Application</span></span>|<span data-ttu-id="388c8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="388c8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="388c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="388c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="388c8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="388c8-120">Request headers</span></span>
|<span data-ttu-id="388c8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="388c8-121">Header</span></span>|<span data-ttu-id="388c8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="388c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="388c8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="388c8-123">Authorization</span></span>|<span data-ttu-id="388c8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="388c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="388c8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="388c8-125">Accept</span></span>|<span data-ttu-id="388c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="388c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="388c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="388c8-127">Request body</span></span>
<span data-ttu-id="388c8-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="388c8-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="388c8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="388c8-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="388c8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="388c8-130">Property</span></span>|<span data-ttu-id="388c8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="388c8-131">Type</span></span>|<span data-ttu-id="388c8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="388c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="388c8-133">id</span><span class="sxs-lookup"><span data-stu-id="388c8-133">id</span></span>|<span data-ttu-id="388c8-134">String</span><span class="sxs-lookup"><span data-stu-id="388c8-134">String</span></span>|<span data-ttu-id="388c8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="388c8-135">Key of the entity.</span></span> <span data-ttu-id="388c8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="388c8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="388c8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="388c8-138">DateTimeOffset</span></span>|<span data-ttu-id="388c8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="388c8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="388c8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="388c8-141">roleScopeTagIds</span></span>|<span data-ttu-id="388c8-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="388c8-142">String collection</span></span>|<span data-ttu-id="388c8-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="388c8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="388c8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="388c8-145">supportsScopeTags</span></span>|<span data-ttu-id="388c8-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="388c8-146">Boolean</span></span>|<span data-ttu-id="388c8-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="388c8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="388c8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="388c8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="388c8-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="388c8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="388c8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="388c8-150">This property is read-only.</span></span> <span data-ttu-id="388c8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="388c8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="388c8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="388c8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="388c8-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="388c8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="388c8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="388c8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="388c8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="388c8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="388c8-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="388c8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="388c8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="388c8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="388c8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="388c8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="388c8-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="388c8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="388c8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="388c8-164">createdDateTime</span></span>|<span data-ttu-id="388c8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="388c8-165">DateTimeOffset</span></span>|<span data-ttu-id="388c8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="388c8-166">DateTime the object was created.</span></span> <span data-ttu-id="388c8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-168">descrição</span><span class="sxs-lookup"><span data-stu-id="388c8-168">description</span></span>|<span data-ttu-id="388c8-169">String</span><span class="sxs-lookup"><span data-stu-id="388c8-169">String</span></span>|<span data-ttu-id="388c8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="388c8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="388c8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="388c8-172">displayName</span></span>|<span data-ttu-id="388c8-173">String</span><span class="sxs-lookup"><span data-stu-id="388c8-173">String</span></span>|<span data-ttu-id="388c8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="388c8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="388c8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-176">versão</span><span class="sxs-lookup"><span data-stu-id="388c8-176">version</span></span>|<span data-ttu-id="388c8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="388c8-177">Int32</span></span>|<span data-ttu-id="388c8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="388c8-178">Version of the device configuration.</span></span> <span data-ttu-id="388c8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="388c8-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="388c8-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="388c8-181">Int32</span><span class="sxs-lookup"><span data-stu-id="388c8-181">Int32</span></span>|<span data-ttu-id="388c8-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="388c8-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="388c8-183">Valores válidos de 1 a 99 Herdados [de iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="388c8-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="388c8-184">subjectNameFormat</span></span>|[<span data-ttu-id="388c8-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="388c8-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="388c8-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="388c8-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="388c8-187">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="388c8-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="388c8-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="388c8-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="388c8-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="388c8-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="388c8-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="388c8-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="388c8-191">Tipo de Nome Alternativo do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="388c8-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="388c8-192">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="388c8-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="388c8-193">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="388c8-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="388c8-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="388c8-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="388c8-195">Int32</span><span class="sxs-lookup"><span data-stu-id="388c8-195">Int32</span></span>|<span data-ttu-id="388c8-196">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="388c8-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="388c8-197">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="388c8-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="388c8-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="388c8-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="388c8-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="388c8-200">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="388c8-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="388c8-201">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="388c8-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="388c8-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="388c8-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="388c8-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="388c8-203">scepServerUrls</span></span>|<span data-ttu-id="388c8-204">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="388c8-204">String collection</span></span>|<span data-ttu-id="388c8-205">Url(s) do servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="388c8-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="388c8-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="388c8-206">subjectNameFormatString</span></span>|<span data-ttu-id="388c8-207">String</span><span class="sxs-lookup"><span data-stu-id="388c8-207">String</span></span>|<span data-ttu-id="388c8-208">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="388c8-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="388c8-209">Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="388c8-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="388c8-210">keyUsage</span><span class="sxs-lookup"><span data-stu-id="388c8-210">keyUsage</span></span>|[<span data-ttu-id="388c8-211">keyUsages</span><span class="sxs-lookup"><span data-stu-id="388c8-211">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="388c8-212">Uso da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="388c8-212">SCEP Key Usage.</span></span> <span data-ttu-id="388c8-213">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="388c8-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="388c8-214">keySize</span><span class="sxs-lookup"><span data-stu-id="388c8-214">keySize</span></span>|[<span data-ttu-id="388c8-215">keySize</span><span class="sxs-lookup"><span data-stu-id="388c8-215">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="388c8-216">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="388c8-216">SCEP Key Size.</span></span> <span data-ttu-id="388c8-217">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="388c8-217">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="388c8-218">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="388c8-218">extendedKeyUsages</span></span>|<span data-ttu-id="388c8-219">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-219">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="388c8-220">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="388c8-220">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="388c8-221">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="388c8-221">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="388c8-222">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="388c8-222">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="388c8-223">String</span><span class="sxs-lookup"><span data-stu-id="388c8-223">String</span></span>|<span data-ttu-id="388c8-224">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="388c8-224">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="388c8-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="388c8-225">certificateStore</span></span>|[<span data-ttu-id="388c8-226">certificateStore</span><span class="sxs-lookup"><span data-stu-id="388c8-226">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="388c8-227">Certificado de armazenamento de destino.</span><span class="sxs-lookup"><span data-stu-id="388c8-227">Target store certificate.</span></span> <span data-ttu-id="388c8-228">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="388c8-228">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="388c8-229">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="388c8-229">customSubjectAlternativeNames</span></span>|<span data-ttu-id="388c8-230">[Coleção customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="388c8-230">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="388c8-231">Configurações personalizadas de nome alternativo do assunto.</span><span class="sxs-lookup"><span data-stu-id="388c8-231">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="388c8-232">A variável OnPremisesUserPrincipalName é suportada, bem como outras documentadas aqui: http://go.microsoft.com/fwlink/?LinkId=2027630 .</span><span class="sxs-lookup"><span data-stu-id="388c8-232">The OnPremisesUserPrincipalName variable is support as well as others documented here: http://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="388c8-233">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="388c8-233">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="388c8-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="388c8-234">Response</span></span>
<span data-ttu-id="388c8-235">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="388c8-235">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="388c8-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="388c8-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="388c8-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="388c8-237">Request</span></span>
<span data-ttu-id="388c8-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="388c8-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="388c8-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="388c8-239">Response</span></span>
<span data-ttu-id="388c8-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="388c8-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




