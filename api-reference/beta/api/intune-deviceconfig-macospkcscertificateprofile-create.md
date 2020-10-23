---
title: Criar macOSPkcsCertificateProfile
description: Criar um novo objeto macOSPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3f821b1b201c6927ad3a84bd7e0b4b6631c03bf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731852"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="ddb38-103">Criar macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ddb38-103">Create macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="ddb38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddb38-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ddb38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb38-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddb38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb38-107">Criar um novo objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ddb38-107">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddb38-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddb38-108">Prerequisites</span></span>
<span data-ttu-id="ddb38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb38-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddb38-111">Permission type</span></span>|<span data-ttu-id="ddb38-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddb38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddb38-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddb38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddb38-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb38-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddb38-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddb38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddb38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddb38-116">Not supported.</span></span>|
|<span data-ttu-id="ddb38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddb38-117">Application</span></span>|<span data-ttu-id="ddb38-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb38-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddb38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ddb38-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb38-120">Request headers</span></span>
|<span data-ttu-id="ddb38-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddb38-121">Header</span></span>|<span data-ttu-id="ddb38-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ddb38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddb38-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddb38-123">Authorization</span></span>|<span data-ttu-id="ddb38-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddb38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddb38-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddb38-125">Accept</span></span>|<span data-ttu-id="ddb38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddb38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb38-127">Request body</span></span>
<span data-ttu-id="ddb38-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="ddb38-128">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="ddb38-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="ddb38-129">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="ddb38-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddb38-130">Property</span></span>|<span data-ttu-id="ddb38-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddb38-131">Type</span></span>|<span data-ttu-id="ddb38-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb38-133">id</span><span class="sxs-lookup"><span data-stu-id="ddb38-133">id</span></span>|<span data-ttu-id="ddb38-134">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-134">String</span></span>|<span data-ttu-id="ddb38-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ddb38-135">Key of the entity.</span></span> <span data-ttu-id="ddb38-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb38-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ddb38-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb38-138">DateTimeOffset</span></span>|<span data-ttu-id="ddb38-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ddb38-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ddb38-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddb38-141">roleScopeTagIds</span></span>|<span data-ttu-id="ddb38-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddb38-142">String collection</span></span>|<span data-ttu-id="ddb38-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ddb38-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ddb38-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ddb38-145">supportsScopeTags</span></span>|<span data-ttu-id="ddb38-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddb38-146">Boolean</span></span>|<span data-ttu-id="ddb38-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ddb38-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ddb38-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ddb38-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ddb38-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ddb38-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ddb38-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddb38-150">This property is read-only.</span></span> <span data-ttu-id="ddb38-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddb38-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ddb38-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddb38-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ddb38-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ddb38-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ddb38-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddb38-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ddb38-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddb38-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ddb38-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ddb38-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ddb38-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddb38-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ddb38-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddb38-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ddb38-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ddb38-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ddb38-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb38-164">createdDateTime</span></span>|<span data-ttu-id="ddb38-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb38-165">DateTimeOffset</span></span>|<span data-ttu-id="ddb38-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ddb38-166">DateTime the object was created.</span></span> <span data-ttu-id="ddb38-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-168">description</span><span class="sxs-lookup"><span data-stu-id="ddb38-168">description</span></span>|<span data-ttu-id="ddb38-169">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-169">String</span></span>|<span data-ttu-id="ddb38-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ddb38-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddb38-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb38-172">displayName</span></span>|<span data-ttu-id="ddb38-173">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-173">String</span></span>|<span data-ttu-id="ddb38-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ddb38-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddb38-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-176">versão</span><span class="sxs-lookup"><span data-stu-id="ddb38-176">version</span></span>|<span data-ttu-id="ddb38-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb38-177">Int32</span></span>|<span data-ttu-id="ddb38-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ddb38-178">Version of the device configuration.</span></span> <span data-ttu-id="ddb38-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb38-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ddb38-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="ddb38-181">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb38-181">Int32</span></span>|<span data-ttu-id="ddb38-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="ddb38-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ddb38-183">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ddb38-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ddb38-184">subjectNameFormat</span></span>|[<span data-ttu-id="ddb38-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ddb38-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="ddb38-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ddb38-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="ddb38-187">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ddb38-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ddb38-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="ddb38-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="ddb38-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ddb38-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ddb38-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ddb38-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ddb38-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ddb38-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ddb38-192">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ddb38-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ddb38-193">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="ddb38-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="ddb38-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ddb38-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ddb38-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb38-195">Int32</span></span>|<span data-ttu-id="ddb38-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ddb38-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ddb38-197">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ddb38-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ddb38-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ddb38-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ddb38-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ddb38-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ddb38-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ddb38-201">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ddb38-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ddb38-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ddb38-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ddb38-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="ddb38-203">certificationAuthority</span></span>|<span data-ttu-id="ddb38-204">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-204">String</span></span>|<span data-ttu-id="ddb38-205">FQDN da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="ddb38-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="ddb38-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="ddb38-206">certificationAuthorityName</span></span>|<span data-ttu-id="ddb38-207">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-207">String</span></span>|<span data-ttu-id="ddb38-208">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="ddb38-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="ddb38-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="ddb38-209">certificateTemplateName</span></span>|<span data-ttu-id="ddb38-210">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-210">String</span></span>|<span data-ttu-id="ddb38-211">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="ddb38-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="ddb38-212">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="ddb38-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ddb38-213">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-213">String</span></span>|<span data-ttu-id="ddb38-214">Cadeia de caracteres de formato que define o nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="ddb38-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="ddb38-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ddb38-215">subjectNameFormatString</span></span>|<span data-ttu-id="ddb38-216">String</span><span class="sxs-lookup"><span data-stu-id="ddb38-216">String</span></span>|<span data-ttu-id="ddb38-217">Cadeia de caracteres de formato que define o nome da entidade.</span><span class="sxs-lookup"><span data-stu-id="ddb38-217">Format string that defines the subject name.</span></span> <span data-ttu-id="ddb38-218">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="ddb38-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ddb38-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ddb38-219">certificateStore</span></span>|[<span data-ttu-id="ddb38-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ddb38-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ddb38-221">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="ddb38-221">Target store certificate.</span></span> <span data-ttu-id="ddb38-222">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="ddb38-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ddb38-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ddb38-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ddb38-224">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="ddb38-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ddb38-225">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="ddb38-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ddb38-226">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ddb38-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ddb38-227">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="ddb38-227">allowAllAppsAccess</span></span>|<span data-ttu-id="ddb38-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddb38-228">Boolean</span></span>|<span data-ttu-id="ddb38-229">Configuração AllowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="ddb38-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="ddb38-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb38-230">Response</span></span>
<span data-ttu-id="ddb38-231">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb38-231">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddb38-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddb38-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddb38-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb38-233">Request</span></span>
<span data-ttu-id="ddb38-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddb38-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSPkcsCertificateProfile",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "allowAllAppsAccess": true
}
```

### <a name="response"></a><span data-ttu-id="ddb38-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb38-235">Response</span></span>
<span data-ttu-id="ddb38-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddb38-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSPkcsCertificateProfile",
  "id": "4b489237-9237-4b48-3792-484b3792484b",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "allowAllAppsAccess": true
}
```





