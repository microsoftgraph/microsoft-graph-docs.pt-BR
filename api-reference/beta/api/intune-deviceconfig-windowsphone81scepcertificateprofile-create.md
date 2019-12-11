---
title: Criar windowsPhone81SCEPCertificateProfile
description: Criar um novo objeto windowsPhone81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fedef02ccf2ceaebdc26185cfc0bc402af39178
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946557"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="011a6-103">Criar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="011a6-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="011a6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="011a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="011a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="011a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="011a6-106">Criar um novo objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="011a6-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="011a6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="011a6-107">Prerequisites</span></span>
<span data-ttu-id="011a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="011a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="011a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="011a6-110">Permission type</span></span>|<span data-ttu-id="011a6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="011a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="011a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="011a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="011a6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="011a6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="011a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="011a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="011a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="011a6-115">Not supported.</span></span>|
|<span data-ttu-id="011a6-116">Application</span><span class="sxs-lookup"><span data-stu-id="011a6-116">Application</span></span>|<span data-ttu-id="011a6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="011a6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="011a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="011a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="011a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="011a6-119">Request headers</span></span>
|<span data-ttu-id="011a6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="011a6-120">Header</span></span>|<span data-ttu-id="011a6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="011a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="011a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="011a6-122">Authorization</span></span>|<span data-ttu-id="011a6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="011a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="011a6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="011a6-124">Accept</span></span>|<span data-ttu-id="011a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="011a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="011a6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="011a6-126">Request body</span></span>
<span data-ttu-id="011a6-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="011a6-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="011a6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="011a6-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="011a6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="011a6-129">Property</span></span>|<span data-ttu-id="011a6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="011a6-130">Type</span></span>|<span data-ttu-id="011a6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="011a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="011a6-132">id</span><span class="sxs-lookup"><span data-stu-id="011a6-132">id</span></span>|<span data-ttu-id="011a6-133">String</span><span class="sxs-lookup"><span data-stu-id="011a6-133">String</span></span>|<span data-ttu-id="011a6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="011a6-134">Key of the entity.</span></span> <span data-ttu-id="011a6-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="011a6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="011a6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="011a6-137">DateTimeOffset</span></span>|<span data-ttu-id="011a6-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="011a6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="011a6-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="011a6-140">roleScopeTagIds</span></span>|<span data-ttu-id="011a6-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="011a6-141">String collection</span></span>|<span data-ttu-id="011a6-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="011a6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="011a6-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="011a6-144">supportsScopeTags</span></span>|<span data-ttu-id="011a6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="011a6-145">Boolean</span></span>|<span data-ttu-id="011a6-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="011a6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="011a6-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="011a6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="011a6-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="011a6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="011a6-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="011a6-149">This property is read-only.</span></span> <span data-ttu-id="011a6-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="011a6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="011a6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="011a6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="011a6-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="011a6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="011a6-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="011a6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="011a6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="011a6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="011a6-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="011a6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="011a6-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="011a6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="011a6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="011a6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="011a6-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="011a6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="011a6-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="011a6-163">createdDateTime</span></span>|<span data-ttu-id="011a6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="011a6-164">DateTimeOffset</span></span>|<span data-ttu-id="011a6-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="011a6-165">DateTime the object was created.</span></span> <span data-ttu-id="011a6-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-167">description</span><span class="sxs-lookup"><span data-stu-id="011a6-167">description</span></span>|<span data-ttu-id="011a6-168">String</span><span class="sxs-lookup"><span data-stu-id="011a6-168">String</span></span>|<span data-ttu-id="011a6-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="011a6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="011a6-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="011a6-171">displayName</span></span>|<span data-ttu-id="011a6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="011a6-172">String</span></span>|<span data-ttu-id="011a6-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="011a6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="011a6-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-175">versão</span><span class="sxs-lookup"><span data-stu-id="011a6-175">version</span></span>|<span data-ttu-id="011a6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="011a6-176">Int32</span></span>|<span data-ttu-id="011a6-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="011a6-177">Version of the device configuration.</span></span> <span data-ttu-id="011a6-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="011a6-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="011a6-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="011a6-180">Int32</span><span class="sxs-lookup"><span data-stu-id="011a6-180">Int32</span></span>|<span data-ttu-id="011a6-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="011a6-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="011a6-182">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-182">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="011a6-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="011a6-183">keyStorageProvider</span></span>|[<span data-ttu-id="011a6-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="011a6-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="011a6-185">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="011a6-185">Key Storage Provider (KSP).</span></span> <span data-ttu-id="011a6-186">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="011a6-186">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="011a6-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="011a6-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="011a6-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="011a6-188">subjectNameFormat</span></span>|[<span data-ttu-id="011a6-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="011a6-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="011a6-190">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="011a6-190">Certificate Subject Name Format.</span></span> <span data-ttu-id="011a6-191">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="011a6-191">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="011a6-192">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="011a6-192">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="011a6-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="011a6-193">subjectAlternativeNameType</span></span>|[<span data-ttu-id="011a6-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="011a6-194">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="011a6-195">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="011a6-195">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="011a6-196">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="011a6-196">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="011a6-197">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="011a6-197">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="011a6-198">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="011a6-198">certificateValidityPeriodValue</span></span>|<span data-ttu-id="011a6-199">Int32</span><span class="sxs-lookup"><span data-stu-id="011a6-199">Int32</span></span>|<span data-ttu-id="011a6-200">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="011a6-200">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="011a6-201">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-201">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="011a6-202">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="011a6-202">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="011a6-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="011a6-203">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="011a6-204">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="011a6-204">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="011a6-205">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="011a6-205">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="011a6-206">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="011a6-206">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="011a6-207">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="011a6-207">extendedKeyUsages</span></span>|<span data-ttu-id="011a6-208">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-208">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="011a6-209">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="011a6-209">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="011a6-210">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="011a6-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="011a6-211">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="011a6-211">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="011a6-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="011a6-212">scepServerUrls</span></span>|<span data-ttu-id="011a6-213">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="011a6-213">String collection</span></span>|<span data-ttu-id="011a6-214">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="011a6-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="011a6-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="011a6-215">subjectNameFormatString</span></span>|<span data-ttu-id="011a6-216">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="011a6-216">String</span></span>|<span data-ttu-id="011a6-217">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="011a6-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="011a6-218">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="011a6-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="011a6-219">uso de</span><span class="sxs-lookup"><span data-stu-id="011a6-219">keyUsage</span></span>|[<span data-ttu-id="011a6-220">usos de</span><span class="sxs-lookup"><span data-stu-id="011a6-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="011a6-221">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="011a6-221">SCEP Key Usage.</span></span> <span data-ttu-id="011a6-222">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="011a6-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="011a6-223">keySize</span><span class="sxs-lookup"><span data-stu-id="011a6-223">keySize</span></span>|[<span data-ttu-id="011a6-224">keySize</span><span class="sxs-lookup"><span data-stu-id="011a6-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="011a6-225">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="011a6-225">SCEP Key Size.</span></span> <span data-ttu-id="011a6-226">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="011a6-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="011a6-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="011a6-227">hashAlgorithm</span></span>|[<span data-ttu-id="011a6-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="011a6-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="011a6-229">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="011a6-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="011a6-230">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="011a6-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="011a6-231">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="011a6-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="011a6-232">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="011a6-232">String</span></span>|<span data-ttu-id="011a6-233">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="011a6-233">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="011a6-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="011a6-234">Response</span></span>
<span data-ttu-id="011a6-235">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="011a6-235">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="011a6-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="011a6-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="011a6-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="011a6-237">Request</span></span>
<span data-ttu-id="011a6-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="011a6-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="011a6-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="011a6-239">Response</span></span>
<span data-ttu-id="011a6-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="011a6-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





