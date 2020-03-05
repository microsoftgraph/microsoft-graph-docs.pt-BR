---
title: Atualizar windows10ImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto windows10ImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 172ff6e442685dbadf3dd84e796ee1783864b3c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42479363"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="9278c-103">Atualizar windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9278c-103">Update windows10ImportedPFXCertificateProfile</span></span>

<span data-ttu-id="9278c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9278c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9278c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9278c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9278c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9278c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9278c-107">Atualiza as propriedades de um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9278c-107">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9278c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9278c-108">Prerequisites</span></span>
<span data-ttu-id="9278c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9278c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9278c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9278c-111">Permission type</span></span>|<span data-ttu-id="9278c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9278c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9278c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9278c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9278c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9278c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9278c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9278c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9278c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9278c-116">Not supported.</span></span>|
|<span data-ttu-id="9278c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9278c-117">Application</span></span>|<span data-ttu-id="9278c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9278c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9278c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9278c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9278c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9278c-120">Request headers</span></span>
|<span data-ttu-id="9278c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9278c-121">Header</span></span>|<span data-ttu-id="9278c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9278c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9278c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9278c-123">Authorization</span></span>|<span data-ttu-id="9278c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9278c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9278c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9278c-125">Accept</span></span>|<span data-ttu-id="9278c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9278c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9278c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9278c-127">Request body</span></span>
<span data-ttu-id="9278c-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9278c-128">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="9278c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9278c-129">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="9278c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9278c-130">Property</span></span>|<span data-ttu-id="9278c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9278c-131">Type</span></span>|<span data-ttu-id="9278c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9278c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9278c-133">id</span><span class="sxs-lookup"><span data-stu-id="9278c-133">id</span></span>|<span data-ttu-id="9278c-134">String</span><span class="sxs-lookup"><span data-stu-id="9278c-134">String</span></span>|<span data-ttu-id="9278c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9278c-135">Key of the entity.</span></span> <span data-ttu-id="9278c-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9278c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9278c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9278c-138">DateTimeOffset</span></span>|<span data-ttu-id="9278c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9278c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9278c-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9278c-141">roleScopeTagIds</span></span>|<span data-ttu-id="9278c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9278c-142">String collection</span></span>|<span data-ttu-id="9278c-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9278c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9278c-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9278c-145">supportsScopeTags</span></span>|<span data-ttu-id="9278c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9278c-146">Boolean</span></span>|<span data-ttu-id="9278c-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9278c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9278c-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9278c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9278c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9278c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9278c-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9278c-150">This property is read-only.</span></span> <span data-ttu-id="9278c-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9278c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9278c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9278c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9278c-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9278c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9278c-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9278c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9278c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9278c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9278c-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9278c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9278c-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9278c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9278c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9278c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9278c-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9278c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9278c-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9278c-164">createdDateTime</span></span>|<span data-ttu-id="9278c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9278c-165">DateTimeOffset</span></span>|<span data-ttu-id="9278c-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9278c-166">DateTime the object was created.</span></span> <span data-ttu-id="9278c-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-168">description</span><span class="sxs-lookup"><span data-stu-id="9278c-168">description</span></span>|<span data-ttu-id="9278c-169">String</span><span class="sxs-lookup"><span data-stu-id="9278c-169">String</span></span>|<span data-ttu-id="9278c-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9278c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9278c-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9278c-172">displayName</span></span>|<span data-ttu-id="9278c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9278c-173">String</span></span>|<span data-ttu-id="9278c-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9278c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9278c-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-176">versão</span><span class="sxs-lookup"><span data-stu-id="9278c-176">version</span></span>|<span data-ttu-id="9278c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9278c-177">Int32</span></span>|<span data-ttu-id="9278c-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9278c-178">Version of the device configuration.</span></span> <span data-ttu-id="9278c-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9278c-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9278c-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="9278c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="9278c-181">Int32</span></span>|<span data-ttu-id="9278c-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="9278c-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9278c-183">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9278c-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="9278c-184">keyStorageProvider</span></span>|[<span data-ttu-id="9278c-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="9278c-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="9278c-186">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9278c-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9278c-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="9278c-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="9278c-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9278c-188">subjectNameFormat</span></span>|[<span data-ttu-id="9278c-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9278c-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9278c-190">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9278c-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9278c-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="9278c-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9278c-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9278c-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9278c-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9278c-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9278c-194">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9278c-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9278c-195">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="9278c-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9278c-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9278c-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9278c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="9278c-197">Int32</span></span>|<span data-ttu-id="9278c-198">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9278c-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9278c-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9278c-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9278c-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9278c-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9278c-201">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9278c-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9278c-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="9278c-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9278c-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="9278c-203">intendedPurpose</span></span>|[<span data-ttu-id="9278c-204">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="9278c-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="9278c-205">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="9278c-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="9278c-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="9278c-206">Response</span></span>
<span data-ttu-id="9278c-207">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9278c-207">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9278c-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9278c-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="9278c-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9278c-209">Request</span></span>
<span data-ttu-id="9278c-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9278c-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1359

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="9278c-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="9278c-211">Response</span></span>
<span data-ttu-id="9278c-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9278c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1531

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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





