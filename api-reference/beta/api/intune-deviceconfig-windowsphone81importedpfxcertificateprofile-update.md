---
title: Atualizar windowsPhone81ImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto windowsPhone81ImportedPFXCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11851dd2c6efb87f5187e552865cfc8860cde03e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42733851"
---
# <a name="update-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="6724b-103">Atualizar windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6724b-103">Update windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="6724b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6724b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6724b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6724b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6724b-106">Atualiza as propriedades de um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6724b-106">Update the properties of a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6724b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6724b-107">Prerequisites</span></span>
<span data-ttu-id="6724b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6724b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6724b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6724b-110">Permission type</span></span>|<span data-ttu-id="6724b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6724b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6724b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6724b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6724b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6724b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6724b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6724b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6724b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6724b-115">Not supported.</span></span>|
|<span data-ttu-id="6724b-116">Application</span><span class="sxs-lookup"><span data-stu-id="6724b-116">Application</span></span>|<span data-ttu-id="6724b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6724b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6724b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6724b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6724b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6724b-119">Request headers</span></span>
|<span data-ttu-id="6724b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6724b-120">Header</span></span>|<span data-ttu-id="6724b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6724b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6724b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6724b-122">Authorization</span></span>|<span data-ttu-id="6724b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6724b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6724b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6724b-124">Accept</span></span>|<span data-ttu-id="6724b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6724b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6724b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6724b-126">Request body</span></span>
<span data-ttu-id="6724b-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6724b-127">In the request body, supply a JSON representation for the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="6724b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6724b-128">The following table shows the properties that are required when you create the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="6724b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6724b-129">Property</span></span>|<span data-ttu-id="6724b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6724b-130">Type</span></span>|<span data-ttu-id="6724b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6724b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6724b-132">id</span><span class="sxs-lookup"><span data-stu-id="6724b-132">id</span></span>|<span data-ttu-id="6724b-133">String</span><span class="sxs-lookup"><span data-stu-id="6724b-133">String</span></span>|<span data-ttu-id="6724b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6724b-134">Key of the entity.</span></span> <span data-ttu-id="6724b-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6724b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6724b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6724b-137">DateTimeOffset</span></span>|<span data-ttu-id="6724b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6724b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6724b-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6724b-140">roleScopeTagIds</span></span>|<span data-ttu-id="6724b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6724b-141">String collection</span></span>|<span data-ttu-id="6724b-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6724b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6724b-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6724b-144">supportsScopeTags</span></span>|<span data-ttu-id="6724b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6724b-145">Boolean</span></span>|<span data-ttu-id="6724b-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6724b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6724b-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6724b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6724b-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6724b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6724b-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6724b-149">This property is read-only.</span></span> <span data-ttu-id="6724b-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6724b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6724b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6724b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6724b-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6724b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6724b-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6724b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6724b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6724b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6724b-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6724b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6724b-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6724b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6724b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6724b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6724b-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6724b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6724b-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6724b-163">createdDateTime</span></span>|<span data-ttu-id="6724b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6724b-164">DateTimeOffset</span></span>|<span data-ttu-id="6724b-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6724b-165">DateTime the object was created.</span></span> <span data-ttu-id="6724b-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-167">description</span><span class="sxs-lookup"><span data-stu-id="6724b-167">description</span></span>|<span data-ttu-id="6724b-168">String</span><span class="sxs-lookup"><span data-stu-id="6724b-168">String</span></span>|<span data-ttu-id="6724b-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6724b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6724b-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6724b-171">displayName</span></span>|<span data-ttu-id="6724b-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6724b-172">String</span></span>|<span data-ttu-id="6724b-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6724b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6724b-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-175">versão</span><span class="sxs-lookup"><span data-stu-id="6724b-175">version</span></span>|<span data-ttu-id="6724b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6724b-176">Int32</span></span>|<span data-ttu-id="6724b-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6724b-177">Version of the device configuration.</span></span> <span data-ttu-id="6724b-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6724b-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6724b-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="6724b-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6724b-180">Int32</span></span>|<span data-ttu-id="6724b-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="6724b-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6724b-182">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6724b-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="6724b-183">keyStorageProvider</span></span>|[<span data-ttu-id="6724b-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="6724b-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="6724b-185">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6724b-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6724b-186">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="6724b-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="6724b-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6724b-187">subjectNameFormat</span></span>|[<span data-ttu-id="6724b-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6724b-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6724b-189">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6724b-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6724b-190">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6724b-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6724b-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6724b-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6724b-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6724b-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6724b-193">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6724b-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6724b-194">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6724b-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6724b-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6724b-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6724b-196">Int32</span><span class="sxs-lookup"><span data-stu-id="6724b-196">Int32</span></span>|<span data-ttu-id="6724b-197">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6724b-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6724b-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6724b-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6724b-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6724b-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6724b-200">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6724b-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6724b-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6724b-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6724b-202">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="6724b-202">intendedPurpose</span></span>|[<span data-ttu-id="6724b-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="6724b-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="6724b-204">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="6724b-204">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="6724b-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="6724b-205">Response</span></span>
<span data-ttu-id="6724b-206">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6724b-206">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6724b-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6724b-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="6724b-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6724b-208">Request</span></span>
<span data-ttu-id="6724b-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6724b-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="6724b-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="6724b-210">Response</span></span>
<span data-ttu-id="6724b-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6724b-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




