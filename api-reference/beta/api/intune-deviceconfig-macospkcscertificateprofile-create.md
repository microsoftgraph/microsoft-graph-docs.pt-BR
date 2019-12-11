---
title: Criar macOSPkcsCertificateProfile
description: Criar um novo objeto macOSPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7eddb0e927968048261cb658b8a46aed1fc1c68
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948209"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="8d9bc-103">Criar macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8d9bc-103">Create macOSPkcsCertificateProfile</span></span>

> <span data-ttu-id="8d9bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d9bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d9bc-106">Criar um novo objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8d9bc-106">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d9bc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d9bc-107">Prerequisites</span></span>
<span data-ttu-id="8d9bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d9bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d9bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d9bc-110">Permission type</span></span>|<span data-ttu-id="8d9bc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d9bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d9bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d9bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d9bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d9bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-115">Not supported.</span></span>|
|<span data-ttu-id="8d9bc-116">Application</span><span class="sxs-lookup"><span data-stu-id="8d9bc-116">Application</span></span>|<span data-ttu-id="8d9bc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d9bc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d9bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d9bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d9bc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d9bc-119">Request headers</span></span>
|<span data-ttu-id="8d9bc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d9bc-120">Header</span></span>|<span data-ttu-id="8d9bc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8d9bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d9bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d9bc-122">Authorization</span></span>|<span data-ttu-id="8d9bc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d9bc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d9bc-124">Accept</span></span>|<span data-ttu-id="8d9bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d9bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d9bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d9bc-126">Request body</span></span>
<span data-ttu-id="8d9bc-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-127">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="8d9bc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-128">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="8d9bc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d9bc-129">Property</span></span>|<span data-ttu-id="8d9bc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d9bc-130">Type</span></span>|<span data-ttu-id="8d9bc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d9bc-132">id</span><span class="sxs-lookup"><span data-stu-id="8d9bc-132">id</span></span>|<span data-ttu-id="8d9bc-133">String</span><span class="sxs-lookup"><span data-stu-id="8d9bc-133">String</span></span>|<span data-ttu-id="8d9bc-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-134">Key of the entity.</span></span> <span data-ttu-id="8d9bc-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d9bc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d9bc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d9bc-137">DateTimeOffset</span></span>|<span data-ttu-id="8d9bc-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8d9bc-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d9bc-140">roleScopeTagIds</span></span>|<span data-ttu-id="8d9bc-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-141">String collection</span></span>|<span data-ttu-id="8d9bc-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d9bc-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8d9bc-144">supportsScopeTags</span></span>|<span data-ttu-id="8d9bc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d9bc-145">Boolean</span></span>|<span data-ttu-id="8d9bc-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d9bc-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d9bc-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d9bc-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-149">This property is read-only.</span></span> <span data-ttu-id="8d9bc-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8d9bc-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8d9bc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8d9bc-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8d9bc-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8d9bc-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8d9bc-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8d9bc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8d9bc-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8d9bc-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8d9bc-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8d9bc-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8d9bc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8d9bc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8d9bc-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8d9bc-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d9bc-163">createdDateTime</span></span>|<span data-ttu-id="8d9bc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d9bc-164">DateTimeOffset</span></span>|<span data-ttu-id="8d9bc-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-165">DateTime the object was created.</span></span> <span data-ttu-id="8d9bc-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-167">description</span><span class="sxs-lookup"><span data-stu-id="8d9bc-167">description</span></span>|<span data-ttu-id="8d9bc-168">String</span><span class="sxs-lookup"><span data-stu-id="8d9bc-168">String</span></span>|<span data-ttu-id="8d9bc-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d9bc-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8d9bc-171">displayName</span></span>|<span data-ttu-id="8d9bc-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-172">String</span></span>|<span data-ttu-id="8d9bc-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d9bc-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-175">versão</span><span class="sxs-lookup"><span data-stu-id="8d9bc-175">version</span></span>|<span data-ttu-id="8d9bc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8d9bc-176">Int32</span></span>|<span data-ttu-id="8d9bc-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-177">Version of the device configuration.</span></span> <span data-ttu-id="8d9bc-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d9bc-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8d9bc-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="8d9bc-180">Int32</span><span class="sxs-lookup"><span data-stu-id="8d9bc-180">Int32</span></span>|<span data-ttu-id="8d9bc-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8d9bc-182">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8d9bc-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8d9bc-183">subjectNameFormat</span></span>|[<span data-ttu-id="8d9bc-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8d9bc-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="8d9bc-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="8d9bc-186">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d9bc-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="8d9bc-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="8d9bc-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8d9bc-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8d9bc-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8d9bc-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8d9bc-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="8d9bc-191">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d9bc-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="8d9bc-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8d9bc-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8d9bc-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8d9bc-194">Int32</span><span class="sxs-lookup"><span data-stu-id="8d9bc-194">Int32</span></span>|<span data-ttu-id="8d9bc-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8d9bc-196">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8d9bc-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8d9bc-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8d9bc-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8d9bc-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8d9bc-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8d9bc-200">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d9bc-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="8d9bc-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8d9bc-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="8d9bc-202">certificationAuthority</span></span>|<span data-ttu-id="8d9bc-203">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-203">String</span></span>|<span data-ttu-id="8d9bc-204">FQDN da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-204">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="8d9bc-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="8d9bc-205">certificationAuthorityName</span></span>|<span data-ttu-id="8d9bc-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-206">String</span></span>|<span data-ttu-id="8d9bc-207">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-207">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="8d9bc-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="8d9bc-208">certificateTemplateName</span></span>|<span data-ttu-id="8d9bc-209">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-209">String</span></span>|<span data-ttu-id="8d9bc-210">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-210">PKCS certificate template name.</span></span>|
|<span data-ttu-id="8d9bc-211">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="8d9bc-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8d9bc-212">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-212">String</span></span>|<span data-ttu-id="8d9bc-213">Cadeia de caracteres de formato que define o nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-213">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="8d9bc-214">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8d9bc-214">subjectNameFormatString</span></span>|<span data-ttu-id="8d9bc-215">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9bc-215">String</span></span>|<span data-ttu-id="8d9bc-216">Cadeia de caracteres de formato que define o nome da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-216">Format string that defines the subject name.</span></span> <span data-ttu-id="8d9bc-217">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="8d9bc-217">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8d9bc-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8d9bc-218">certificateStore</span></span>|[<span data-ttu-id="8d9bc-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8d9bc-219">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="8d9bc-220">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-220">Target store certificate.</span></span> <span data-ttu-id="8d9bc-221">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-221">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="8d9bc-222">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="8d9bc-222">customSubjectAlternativeNames</span></span>|<span data-ttu-id="8d9bc-223">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="8d9bc-223">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="8d9bc-224">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-224">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="8d9bc-225">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8d9bc-226">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="8d9bc-226">allowAllAppsAccess</span></span>|<span data-ttu-id="8d9bc-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d9bc-227">Boolean</span></span>|<span data-ttu-id="8d9bc-228">Configuração AllowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="8d9bc-228">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="8d9bc-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d9bc-229">Response</span></span>
<span data-ttu-id="8d9bc-230">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-230">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d9bc-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d9bc-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d9bc-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d9bc-232">Request</span></span>
<span data-ttu-id="8d9bc-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d9bc-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d9bc-234">Response</span></span>
<span data-ttu-id="8d9bc-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d9bc-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





