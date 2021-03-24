---
title: Criar windows10PkcsCertificateProfile
description: Crie um novo objeto windows10PkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cab742e45413a038b4ddfa79e662ce6993675323
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127533"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="13beb-103">Criar windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="13beb-103">Create windows10PkcsCertificateProfile</span></span>

<span data-ttu-id="13beb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13beb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13beb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13beb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13beb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13beb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13beb-107">Crie um novo [objeto windows10PkcsCertificateProfile.](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13beb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13beb-108">Prerequisites</span></span>
<span data-ttu-id="13beb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13beb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13beb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13beb-111">Permission type</span></span>|<span data-ttu-id="13beb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13beb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13beb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13beb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13beb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13beb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13beb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13beb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13beb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13beb-116">Not supported.</span></span>|
|<span data-ttu-id="13beb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13beb-117">Application</span></span>|<span data-ttu-id="13beb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13beb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13beb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13beb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13beb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13beb-120">Request headers</span></span>
|<span data-ttu-id="13beb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13beb-121">Header</span></span>|<span data-ttu-id="13beb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13beb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13beb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13beb-123">Authorization</span></span>|<span data-ttu-id="13beb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13beb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13beb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13beb-125">Accept</span></span>|<span data-ttu-id="13beb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13beb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13beb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13beb-127">Request body</span></span>
<span data-ttu-id="13beb-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="13beb-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="13beb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="13beb-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="13beb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13beb-130">Property</span></span>|<span data-ttu-id="13beb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13beb-131">Type</span></span>|<span data-ttu-id="13beb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13beb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13beb-133">id</span><span class="sxs-lookup"><span data-stu-id="13beb-133">id</span></span>|<span data-ttu-id="13beb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-134">String</span></span>|<span data-ttu-id="13beb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="13beb-135">Key of the entity.</span></span> <span data-ttu-id="13beb-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13beb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="13beb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13beb-138">DateTimeOffset</span></span>|<span data-ttu-id="13beb-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="13beb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="13beb-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13beb-141">roleScopeTagIds</span></span>|<span data-ttu-id="13beb-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-142">String collection</span></span>|<span data-ttu-id="13beb-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="13beb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13beb-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="13beb-145">supportsScopeTags</span></span>|<span data-ttu-id="13beb-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="13beb-146">Boolean</span></span>|<span data-ttu-id="13beb-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="13beb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="13beb-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="13beb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="13beb-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="13beb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="13beb-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13beb-150">This property is read-only.</span></span> <span data-ttu-id="13beb-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="13beb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="13beb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="13beb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="13beb-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="13beb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="13beb-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="13beb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="13beb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="13beb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="13beb-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="13beb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="13beb-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="13beb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="13beb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="13beb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="13beb-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="13beb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="13beb-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13beb-164">createdDateTime</span></span>|<span data-ttu-id="13beb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13beb-165">DateTimeOffset</span></span>|<span data-ttu-id="13beb-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="13beb-166">DateTime the object was created.</span></span> <span data-ttu-id="13beb-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-168">descrição</span><span class="sxs-lookup"><span data-stu-id="13beb-168">description</span></span>|<span data-ttu-id="13beb-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-169">String</span></span>|<span data-ttu-id="13beb-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13beb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13beb-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="13beb-172">displayName</span></span>|<span data-ttu-id="13beb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-173">String</span></span>|<span data-ttu-id="13beb-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13beb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13beb-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-176">versão</span><span class="sxs-lookup"><span data-stu-id="13beb-176">version</span></span>|<span data-ttu-id="13beb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="13beb-177">Int32</span></span>|<span data-ttu-id="13beb-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13beb-178">Version of the device configuration.</span></span> <span data-ttu-id="13beb-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13beb-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="13beb-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="13beb-181">Int32</span><span class="sxs-lookup"><span data-stu-id="13beb-181">Int32</span></span>|<span data-ttu-id="13beb-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="13beb-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="13beb-183">Valores válidos de 1 a 99 Herdados do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="13beb-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="13beb-184">keyStorageProvider</span></span>|[<span data-ttu-id="13beb-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="13beb-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="13beb-186">KSP (Provedor de Armazenamento de Chaves) Herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13beb-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="13beb-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="13beb-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="13beb-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="13beb-188">subjectNameFormat</span></span>|[<span data-ttu-id="13beb-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="13beb-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="13beb-190">Formato de Nome do Assunto de Certificado Herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13beb-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="13beb-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="13beb-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="13beb-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="13beb-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="13beb-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="13beb-193">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="13beb-194">Tipo de nome alternativo do assunto do certificado herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13beb-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="13beb-195">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="13beb-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="13beb-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="13beb-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="13beb-197">Int32</span><span class="sxs-lookup"><span data-stu-id="13beb-197">Int32</span></span>|<span data-ttu-id="13beb-198">Valor para o Período de Validade do Certificado Herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="13beb-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="13beb-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="13beb-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="13beb-200">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="13beb-201">Dimensione para o Período de Validade do Certificado Herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13beb-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="13beb-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="13beb-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="13beb-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="13beb-203">certificationAuthority</span></span>|<span data-ttu-id="13beb-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-204">String</span></span>|<span data-ttu-id="13beb-205">Autoridade de Certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="13beb-205">PKCS Certification Authority</span></span>|
|<span data-ttu-id="13beb-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="13beb-206">certificationAuthorityName</span></span>|<span data-ttu-id="13beb-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-207">String</span></span>|<span data-ttu-id="13beb-208">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="13beb-208">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="13beb-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="13beb-209">certificateTemplateName</span></span>|<span data-ttu-id="13beb-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-210">String</span></span>|<span data-ttu-id="13beb-211">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="13beb-211">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="13beb-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="13beb-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="13beb-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-213">String</span></span>|<span data-ttu-id="13beb-214">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="13beb-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="13beb-215">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="13beb-215">extendedKeyUsages</span></span>|<span data-ttu-id="13beb-216">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-216">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="13beb-217">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="13beb-217">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="13beb-218">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="13beb-218">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="13beb-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="13beb-219">subjectNameFormatString</span></span>|<span data-ttu-id="13beb-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13beb-220">String</span></span>|<span data-ttu-id="13beb-221">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="13beb-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="13beb-222">Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="13beb-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="13beb-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="13beb-223">certificateStore</span></span>|[<span data-ttu-id="13beb-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="13beb-224">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="13beb-225">Certificado de armazenamento de destino.</span><span class="sxs-lookup"><span data-stu-id="13beb-225">Target store certificate.</span></span> <span data-ttu-id="13beb-226">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="13beb-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="13beb-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="13beb-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="13beb-228">[Coleção customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="13beb-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="13beb-229">Configurações personalizadas de nome alternativo do assunto.</span><span class="sxs-lookup"><span data-stu-id="13beb-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="13beb-230">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="13beb-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="13beb-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="13beb-231">Response</span></span>
<span data-ttu-id="13beb-232">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13beb-232">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13beb-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13beb-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="13beb-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13beb-234">Request</span></span>
<span data-ttu-id="13beb-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13beb-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2074

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="13beb-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="13beb-236">Response</span></span>
<span data-ttu-id="13beb-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13beb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2246

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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




