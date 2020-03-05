---
title: Atualizar macOSPkcsCertificateProfile
description: Atualiza as propriedades de um objeto macOSPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a44851cfedd710eeab5a70c67a0e3f54fa529f2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442240"
---
# <a name="update-macospkcscertificateprofile"></a><span data-ttu-id="53956-103">Atualizar macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="53956-103">Update macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="53956-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53956-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53956-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53956-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53956-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53956-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53956-107">Atualiza as propriedades de um objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="53956-107">Update the properties of a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53956-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53956-108">Prerequisites</span></span>
<span data-ttu-id="53956-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53956-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53956-111">Permission type</span></span>|<span data-ttu-id="53956-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53956-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53956-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53956-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53956-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53956-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53956-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53956-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53956-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53956-116">Not supported.</span></span>|
|<span data-ttu-id="53956-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53956-117">Application</span></span>|<span data-ttu-id="53956-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53956-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53956-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53956-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="53956-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53956-120">Request headers</span></span>
|<span data-ttu-id="53956-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53956-121">Header</span></span>|<span data-ttu-id="53956-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53956-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53956-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53956-123">Authorization</span></span>|<span data-ttu-id="53956-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53956-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53956-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53956-125">Accept</span></span>|<span data-ttu-id="53956-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53956-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53956-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53956-127">Request body</span></span>
<span data-ttu-id="53956-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="53956-128">In the request body, supply a JSON representation for the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="53956-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="53956-129">The following table shows the properties that are required when you create the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="53956-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53956-130">Property</span></span>|<span data-ttu-id="53956-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53956-131">Type</span></span>|<span data-ttu-id="53956-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53956-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53956-133">id</span><span class="sxs-lookup"><span data-stu-id="53956-133">id</span></span>|<span data-ttu-id="53956-134">String</span><span class="sxs-lookup"><span data-stu-id="53956-134">String</span></span>|<span data-ttu-id="53956-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53956-135">Key of the entity.</span></span> <span data-ttu-id="53956-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53956-137">lastModifiedDateTime</span></span>|<span data-ttu-id="53956-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53956-138">DateTimeOffset</span></span>|<span data-ttu-id="53956-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="53956-139">DateTime the object was last modified.</span></span> <span data-ttu-id="53956-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53956-141">roleScopeTagIds</span></span>|<span data-ttu-id="53956-142">String collection</span><span class="sxs-lookup"><span data-stu-id="53956-142">String collection</span></span>|<span data-ttu-id="53956-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="53956-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="53956-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="53956-145">supportsScopeTags</span></span>|<span data-ttu-id="53956-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="53956-146">Boolean</span></span>|<span data-ttu-id="53956-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="53956-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="53956-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="53956-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="53956-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="53956-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="53956-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53956-150">This property is read-only.</span></span> <span data-ttu-id="53956-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="53956-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="53956-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="53956-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="53956-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="53956-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="53956-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="53956-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="53956-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="53956-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="53956-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="53956-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="53956-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="53956-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="53956-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="53956-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="53956-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="53956-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="53956-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53956-164">createdDateTime</span></span>|<span data-ttu-id="53956-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53956-165">DateTimeOffset</span></span>|<span data-ttu-id="53956-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="53956-166">DateTime the object was created.</span></span> <span data-ttu-id="53956-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-168">description</span><span class="sxs-lookup"><span data-stu-id="53956-168">description</span></span>|<span data-ttu-id="53956-169">String</span><span class="sxs-lookup"><span data-stu-id="53956-169">String</span></span>|<span data-ttu-id="53956-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53956-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53956-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-172">displayName</span><span class="sxs-lookup"><span data-stu-id="53956-172">displayName</span></span>|<span data-ttu-id="53956-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53956-173">String</span></span>|<span data-ttu-id="53956-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53956-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53956-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-176">versão</span><span class="sxs-lookup"><span data-stu-id="53956-176">version</span></span>|<span data-ttu-id="53956-177">Int32</span><span class="sxs-lookup"><span data-stu-id="53956-177">Int32</span></span>|<span data-ttu-id="53956-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53956-178">Version of the device configuration.</span></span> <span data-ttu-id="53956-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53956-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53956-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="53956-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="53956-181">Int32</span><span class="sxs-lookup"><span data-stu-id="53956-181">Int32</span></span>|<span data-ttu-id="53956-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="53956-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="53956-183">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="53956-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="53956-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="53956-184">subjectNameFormat</span></span>|[<span data-ttu-id="53956-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="53956-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="53956-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="53956-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="53956-187">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53956-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="53956-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="53956-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="53956-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="53956-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="53956-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="53956-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="53956-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="53956-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="53956-192">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53956-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="53956-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="53956-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="53956-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="53956-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="53956-195">Int32</span><span class="sxs-lookup"><span data-stu-id="53956-195">Int32</span></span>|<span data-ttu-id="53956-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="53956-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="53956-197">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="53956-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="53956-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="53956-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="53956-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="53956-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="53956-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="53956-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="53956-201">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53956-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="53956-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="53956-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="53956-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="53956-203">certificationAuthority</span></span>|<span data-ttu-id="53956-204">String</span><span class="sxs-lookup"><span data-stu-id="53956-204">String</span></span>|<span data-ttu-id="53956-205">FQDN da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="53956-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="53956-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="53956-206">certificationAuthorityName</span></span>|<span data-ttu-id="53956-207">String</span><span class="sxs-lookup"><span data-stu-id="53956-207">String</span></span>|<span data-ttu-id="53956-208">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="53956-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="53956-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="53956-209">certificateTemplateName</span></span>|<span data-ttu-id="53956-210">String</span><span class="sxs-lookup"><span data-stu-id="53956-210">String</span></span>|<span data-ttu-id="53956-211">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="53956-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="53956-212">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="53956-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="53956-213">String</span><span class="sxs-lookup"><span data-stu-id="53956-213">String</span></span>|<span data-ttu-id="53956-214">Cadeia de caracteres de formato que define o nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="53956-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="53956-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="53956-215">subjectNameFormatString</span></span>|<span data-ttu-id="53956-216">String</span><span class="sxs-lookup"><span data-stu-id="53956-216">String</span></span>|<span data-ttu-id="53956-217">Cadeia de caracteres de formato que define o nome da entidade.</span><span class="sxs-lookup"><span data-stu-id="53956-217">Format string that defines the subject name.</span></span> <span data-ttu-id="53956-218">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="53956-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="53956-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="53956-219">certificateStore</span></span>|[<span data-ttu-id="53956-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="53956-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="53956-221">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="53956-221">Target store certificate.</span></span> <span data-ttu-id="53956-222">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="53956-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="53956-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="53956-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="53956-224">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="53956-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="53956-225">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="53956-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="53956-226">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="53956-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="53956-227">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="53956-227">allowAllAppsAccess</span></span>|<span data-ttu-id="53956-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="53956-228">Boolean</span></span>|<span data-ttu-id="53956-229">Configuração AllowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="53956-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="53956-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="53956-230">Response</span></span>
<span data-ttu-id="53956-231">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53956-231">If successful, this method returns a `200 OK` response code and an updated [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53956-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53956-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="53956-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53956-233">Request</span></span>
<span data-ttu-id="53956-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53956-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="53956-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="53956-235">Response</span></span>
<span data-ttu-id="53956-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53956-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





