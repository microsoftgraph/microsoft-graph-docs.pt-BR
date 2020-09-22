---
title: Criar windowsPhone81ImportedPFXCertificateProfile
description: Criar um novo objeto windowsPhone81ImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de0afddd30a46f74d7053b36724821008e8cbf72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990071"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="70653-103">Criar windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="70653-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

<span data-ttu-id="70653-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70653-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70653-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70653-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70653-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70653-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70653-107">Criar um novo objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="70653-107">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70653-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70653-108">Prerequisites</span></span>
<span data-ttu-id="70653-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70653-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70653-111">Permission type</span></span>|<span data-ttu-id="70653-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70653-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70653-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70653-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70653-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70653-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70653-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70653-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70653-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70653-116">Not supported.</span></span>|
|<span data-ttu-id="70653-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70653-117">Application</span></span>|<span data-ttu-id="70653-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70653-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70653-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70653-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="70653-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70653-120">Request headers</span></span>
|<span data-ttu-id="70653-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70653-121">Header</span></span>|<span data-ttu-id="70653-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70653-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70653-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70653-123">Authorization</span></span>|<span data-ttu-id="70653-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70653-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70653-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70653-125">Accept</span></span>|<span data-ttu-id="70653-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70653-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70653-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70653-127">Request body</span></span>
<span data-ttu-id="70653-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="70653-128">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="70653-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="70653-129">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="70653-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70653-130">Property</span></span>|<span data-ttu-id="70653-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="70653-131">Type</span></span>|<span data-ttu-id="70653-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="70653-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70653-133">id</span><span class="sxs-lookup"><span data-stu-id="70653-133">id</span></span>|<span data-ttu-id="70653-134">String</span><span class="sxs-lookup"><span data-stu-id="70653-134">String</span></span>|<span data-ttu-id="70653-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70653-135">Key of the entity.</span></span> <span data-ttu-id="70653-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70653-137">lastModifiedDateTime</span></span>|<span data-ttu-id="70653-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70653-138">DateTimeOffset</span></span>|<span data-ttu-id="70653-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="70653-139">DateTime the object was last modified.</span></span> <span data-ttu-id="70653-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70653-141">roleScopeTagIds</span></span>|<span data-ttu-id="70653-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70653-142">String collection</span></span>|<span data-ttu-id="70653-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="70653-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70653-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="70653-145">supportsScopeTags</span></span>|<span data-ttu-id="70653-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="70653-146">Boolean</span></span>|<span data-ttu-id="70653-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="70653-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="70653-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="70653-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="70653-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="70653-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="70653-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70653-150">This property is read-only.</span></span> <span data-ttu-id="70653-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70653-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="70653-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70653-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="70653-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="70653-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="70653-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70653-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="70653-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70653-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="70653-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="70653-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="70653-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="70653-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="70653-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="70653-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="70653-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="70653-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="70653-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70653-164">createdDateTime</span></span>|<span data-ttu-id="70653-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70653-165">DateTimeOffset</span></span>|<span data-ttu-id="70653-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="70653-166">DateTime the object was created.</span></span> <span data-ttu-id="70653-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-168">description</span><span class="sxs-lookup"><span data-stu-id="70653-168">description</span></span>|<span data-ttu-id="70653-169">String</span><span class="sxs-lookup"><span data-stu-id="70653-169">String</span></span>|<span data-ttu-id="70653-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="70653-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70653-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-172">displayName</span><span class="sxs-lookup"><span data-stu-id="70653-172">displayName</span></span>|<span data-ttu-id="70653-173">String</span><span class="sxs-lookup"><span data-stu-id="70653-173">String</span></span>|<span data-ttu-id="70653-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="70653-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70653-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-176">versão</span><span class="sxs-lookup"><span data-stu-id="70653-176">version</span></span>|<span data-ttu-id="70653-177">Int32</span><span class="sxs-lookup"><span data-stu-id="70653-177">Int32</span></span>|<span data-ttu-id="70653-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="70653-178">Version of the device configuration.</span></span> <span data-ttu-id="70653-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70653-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70653-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="70653-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="70653-181">Int32</span><span class="sxs-lookup"><span data-stu-id="70653-181">Int32</span></span>|<span data-ttu-id="70653-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="70653-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="70653-183">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="70653-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="70653-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="70653-184">keyStorageProvider</span></span>|[<span data-ttu-id="70653-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="70653-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="70653-186">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="70653-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="70653-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="70653-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="70653-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="70653-188">subjectNameFormat</span></span>|[<span data-ttu-id="70653-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="70653-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="70653-190">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="70653-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="70653-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="70653-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="70653-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="70653-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="70653-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="70653-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="70653-194">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="70653-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="70653-195">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="70653-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="70653-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="70653-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="70653-197">Int32</span><span class="sxs-lookup"><span data-stu-id="70653-197">Int32</span></span>|<span data-ttu-id="70653-198">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="70653-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="70653-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="70653-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="70653-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="70653-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="70653-201">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="70653-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="70653-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="70653-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="70653-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="70653-203">intendedPurpose</span></span>|[<span data-ttu-id="70653-204">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="70653-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="70653-205">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são: `unassigned` , `smimeEncryption` , `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="70653-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="70653-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="70653-206">Response</span></span>
<span data-ttu-id="70653-207">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70653-207">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70653-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70653-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="70653-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70653-209">Request</span></span>
<span data-ttu-id="70653-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70653-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70653-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="70653-211">Response</span></span>
<span data-ttu-id="70653-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70653-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






