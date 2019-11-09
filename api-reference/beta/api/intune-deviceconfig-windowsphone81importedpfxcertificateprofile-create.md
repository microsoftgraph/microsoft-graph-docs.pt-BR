---
title: Criar windowsPhone81ImportedPFXCertificateProfile
description: Criar um novo objeto windowsPhone81ImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06a39a627c8477f482d4eb50c4fe6af57457d72e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087899"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="48a7f-103">Criar windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="48a7f-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="48a7f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48a7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48a7f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48a7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48a7f-106">Criar um novo objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="48a7f-106">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48a7f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48a7f-107">Prerequisites</span></span>
<span data-ttu-id="48a7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48a7f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48a7f-110">Permission type</span></span>|<span data-ttu-id="48a7f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48a7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48a7f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48a7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48a7f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a7f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48a7f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48a7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48a7f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48a7f-115">Not supported.</span></span>|
|<span data-ttu-id="48a7f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48a7f-116">Application</span></span>|<span data-ttu-id="48a7f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a7f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48a7f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48a7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48a7f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48a7f-119">Request headers</span></span>
|<span data-ttu-id="48a7f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48a7f-120">Header</span></span>|<span data-ttu-id="48a7f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="48a7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48a7f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48a7f-122">Authorization</span></span>|<span data-ttu-id="48a7f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48a7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48a7f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48a7f-124">Accept</span></span>|<span data-ttu-id="48a7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48a7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48a7f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48a7f-126">Request body</span></span>
<span data-ttu-id="48a7f-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="48a7f-127">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="48a7f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="48a7f-128">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="48a7f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48a7f-129">Property</span></span>|<span data-ttu-id="48a7f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="48a7f-130">Type</span></span>|<span data-ttu-id="48a7f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="48a7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48a7f-132">id</span><span class="sxs-lookup"><span data-stu-id="48a7f-132">id</span></span>|<span data-ttu-id="48a7f-133">String</span><span class="sxs-lookup"><span data-stu-id="48a7f-133">String</span></span>|<span data-ttu-id="48a7f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48a7f-134">Key of the entity.</span></span> <span data-ttu-id="48a7f-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48a7f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="48a7f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48a7f-137">DateTimeOffset</span></span>|<span data-ttu-id="48a7f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="48a7f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="48a7f-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48a7f-140">roleScopeTagIds</span></span>|<span data-ttu-id="48a7f-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="48a7f-141">String collection</span></span>|<span data-ttu-id="48a7f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="48a7f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="48a7f-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="48a7f-144">supportsScopeTags</span></span>|<span data-ttu-id="48a7f-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="48a7f-145">Boolean</span></span>|<span data-ttu-id="48a7f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="48a7f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="48a7f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="48a7f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="48a7f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="48a7f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="48a7f-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48a7f-149">This property is read-only.</span></span> <span data-ttu-id="48a7f-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="48a7f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="48a7f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="48a7f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="48a7f-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="48a7f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="48a7f-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="48a7f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="48a7f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="48a7f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="48a7f-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="48a7f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="48a7f-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48a7f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="48a7f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48a7f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="48a7f-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="48a7f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="48a7f-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48a7f-163">createdDateTime</span></span>|<span data-ttu-id="48a7f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48a7f-164">DateTimeOffset</span></span>|<span data-ttu-id="48a7f-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="48a7f-165">DateTime the object was created.</span></span> <span data-ttu-id="48a7f-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-167">descrição</span><span class="sxs-lookup"><span data-stu-id="48a7f-167">description</span></span>|<span data-ttu-id="48a7f-168">String</span><span class="sxs-lookup"><span data-stu-id="48a7f-168">String</span></span>|<span data-ttu-id="48a7f-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48a7f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48a7f-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="48a7f-171">displayName</span></span>|<span data-ttu-id="48a7f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48a7f-172">String</span></span>|<span data-ttu-id="48a7f-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48a7f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48a7f-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-175">versão</span><span class="sxs-lookup"><span data-stu-id="48a7f-175">version</span></span>|<span data-ttu-id="48a7f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="48a7f-176">Int32</span></span>|<span data-ttu-id="48a7f-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48a7f-177">Version of the device configuration.</span></span> <span data-ttu-id="48a7f-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48a7f-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="48a7f-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="48a7f-180">Int32</span><span class="sxs-lookup"><span data-stu-id="48a7f-180">Int32</span></span>|<span data-ttu-id="48a7f-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="48a7f-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="48a7f-182">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="48a7f-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="48a7f-183">keyStorageProvider</span></span>|[<span data-ttu-id="48a7f-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="48a7f-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="48a7f-185">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="48a7f-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="48a7f-186">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="48a7f-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="48a7f-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="48a7f-187">subjectNameFormat</span></span>|[<span data-ttu-id="48a7f-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="48a7f-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="48a7f-189">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="48a7f-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="48a7f-190">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="48a7f-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="48a7f-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="48a7f-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="48a7f-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="48a7f-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="48a7f-193">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="48a7f-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="48a7f-194">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="48a7f-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="48a7f-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="48a7f-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="48a7f-196">Int32</span><span class="sxs-lookup"><span data-stu-id="48a7f-196">Int32</span></span>|<span data-ttu-id="48a7f-197">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="48a7f-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="48a7f-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="48a7f-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="48a7f-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="48a7f-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="48a7f-200">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="48a7f-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="48a7f-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="48a7f-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="48a7f-202">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="48a7f-202">intendedPurpose</span></span>|[<span data-ttu-id="48a7f-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="48a7f-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="48a7f-204">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="48a7f-204">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="48a7f-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a7f-205">Response</span></span>
<span data-ttu-id="48a7f-206">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48a7f-206">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48a7f-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48a7f-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="48a7f-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a7f-208">Request</span></span>
<span data-ttu-id="48a7f-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48a7f-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1364

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="48a7f-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a7f-210">Response</span></span>
<span data-ttu-id="48a7f-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48a7f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1536

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```






