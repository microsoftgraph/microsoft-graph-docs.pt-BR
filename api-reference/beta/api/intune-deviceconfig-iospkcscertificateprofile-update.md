---
title: Atualizar iosPkcsCertificateProfile
description: Atualize as propriedades de um objeto iosPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 555a329f6f36144969627ff5803127310254a610
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147781"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="6abce-103">Atualizar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6abce-103">Update iosPkcsCertificateProfile</span></span>

<span data-ttu-id="6abce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6abce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6abce-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6abce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6abce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6abce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6abce-107">Atualize as propriedades de um [objeto iosPkcsCertificateProfile.](../resources/intune-deviceconfig-iospkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-107">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6abce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6abce-108">Prerequisites</span></span>
<span data-ttu-id="6abce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6abce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6abce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6abce-111">Permission type</span></span>|<span data-ttu-id="6abce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6abce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6abce-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6abce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6abce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6abce-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6abce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6abce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6abce-116">Not supported.</span></span>|
|<span data-ttu-id="6abce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6abce-117">Application</span></span>|<span data-ttu-id="6abce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6abce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6abce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6abce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6abce-120">Request headers</span></span>
|<span data-ttu-id="6abce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6abce-121">Header</span></span>|<span data-ttu-id="6abce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6abce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6abce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6abce-123">Authorization</span></span>|<span data-ttu-id="6abce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6abce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6abce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6abce-125">Accept</span></span>|<span data-ttu-id="6abce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6abce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6abce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6abce-127">Request body</span></span>
<span data-ttu-id="6abce-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosPkcsCertificateProfile.](../resources/intune-deviceconfig-iospkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-128">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="6abce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6abce-129">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="6abce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6abce-130">Property</span></span>|<span data-ttu-id="6abce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6abce-131">Type</span></span>|<span data-ttu-id="6abce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6abce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6abce-133">id</span><span class="sxs-lookup"><span data-stu-id="6abce-133">id</span></span>|<span data-ttu-id="6abce-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-134">String</span></span>|<span data-ttu-id="6abce-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6abce-135">Key of the entity.</span></span> <span data-ttu-id="6abce-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6abce-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6abce-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6abce-138">DateTimeOffset</span></span>|<span data-ttu-id="6abce-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6abce-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6abce-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6abce-141">roleScopeTagIds</span></span>|<span data-ttu-id="6abce-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-142">String collection</span></span>|<span data-ttu-id="6abce-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="6abce-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6abce-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6abce-145">supportsScopeTags</span></span>|<span data-ttu-id="6abce-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="6abce-146">Boolean</span></span>|<span data-ttu-id="6abce-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6abce-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6abce-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6abce-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6abce-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6abce-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6abce-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6abce-150">This property is read-only.</span></span> <span data-ttu-id="6abce-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6abce-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6abce-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6abce-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6abce-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6abce-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6abce-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6abce-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6abce-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6abce-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6abce-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6abce-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6abce-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6abce-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6abce-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6abce-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6abce-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6abce-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6abce-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6abce-164">createdDateTime</span></span>|<span data-ttu-id="6abce-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6abce-165">DateTimeOffset</span></span>|<span data-ttu-id="6abce-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6abce-166">DateTime the object was created.</span></span> <span data-ttu-id="6abce-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-168">descrição</span><span class="sxs-lookup"><span data-stu-id="6abce-168">description</span></span>|<span data-ttu-id="6abce-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-169">String</span></span>|<span data-ttu-id="6abce-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6abce-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6abce-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6abce-172">displayName</span></span>|<span data-ttu-id="6abce-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-173">String</span></span>|<span data-ttu-id="6abce-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6abce-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6abce-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-176">versão</span><span class="sxs-lookup"><span data-stu-id="6abce-176">version</span></span>|<span data-ttu-id="6abce-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6abce-177">Int32</span></span>|<span data-ttu-id="6abce-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6abce-178">Version of the device configuration.</span></span> <span data-ttu-id="6abce-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6abce-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6abce-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="6abce-181">Int32</span><span class="sxs-lookup"><span data-stu-id="6abce-181">Int32</span></span>|<span data-ttu-id="6abce-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="6abce-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6abce-183">Valores válidos de 1 a 99 Herdados [de iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6abce-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6abce-184">subjectNameFormat</span></span>|[<span data-ttu-id="6abce-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6abce-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="6abce-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="6abce-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="6abce-187">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6abce-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="6abce-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="6abce-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="6abce-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6abce-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6abce-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6abce-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="6abce-191">Tipo de Nome Alternativo do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="6abce-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="6abce-192">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6abce-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="6abce-193">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="6abce-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="6abce-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6abce-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6abce-195">Int32</span><span class="sxs-lookup"><span data-stu-id="6abce-195">Int32</span></span>|<span data-ttu-id="6abce-196">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="6abce-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6abce-197">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6abce-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6abce-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6abce-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6abce-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="6abce-200">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="6abce-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6abce-201">Herdado do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6abce-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="6abce-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6abce-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6abce-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="6abce-203">certificationAuthority</span></span>|<span data-ttu-id="6abce-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-204">String</span></span>|<span data-ttu-id="6abce-205">Autoridade de Certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="6abce-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="6abce-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="6abce-206">certificationAuthorityName</span></span>|<span data-ttu-id="6abce-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-207">String</span></span>|<span data-ttu-id="6abce-208">Nome da Autoridade de Certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="6abce-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="6abce-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="6abce-209">certificateTemplateName</span></span>|<span data-ttu-id="6abce-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-210">String</span></span>|<span data-ttu-id="6abce-211">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="6abce-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="6abce-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6abce-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6abce-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-213">String</span></span>|<span data-ttu-id="6abce-214">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="6abce-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="6abce-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6abce-215">subjectNameFormatString</span></span>|<span data-ttu-id="6abce-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abce-216">String</span></span>|<span data-ttu-id="6abce-217">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="6abce-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="6abce-218">Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="6abce-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="6abce-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="6abce-219">certificateStore</span></span>|[<span data-ttu-id="6abce-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="6abce-220">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="6abce-221">Certificado de armazenamento de destino.</span><span class="sxs-lookup"><span data-stu-id="6abce-221">Target store certificate.</span></span> <span data-ttu-id="6abce-222">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="6abce-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="6abce-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="6abce-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="6abce-224">[Coleção customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="6abce-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="6abce-225">Configurações personalizadas de nome alternativo do assunto.</span><span class="sxs-lookup"><span data-stu-id="6abce-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="6abce-226">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6abce-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6abce-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="6abce-227">Response</span></span>
<span data-ttu-id="6abce-228">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6abce-228">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6abce-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6abce-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="6abce-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6abce-230">Request</span></span>
<span data-ttu-id="6abce-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6abce-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1824

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
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

### <a name="response"></a><span data-ttu-id="6abce-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="6abce-232">Response</span></span>
<span data-ttu-id="6abce-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6abce-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1996

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
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




