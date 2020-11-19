---
title: Criar windows81SCEPCertificateProfile
description: Criar um novo objeto windows81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95a2c44d65201105cd449ef10c94309e9b20677d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49204416"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="a8b06-103">Criar windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a8b06-103">Create windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="a8b06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8b06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8b06-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8b06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8b06-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8b06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b06-107">Criar um novo objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a8b06-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8b06-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8b06-108">Prerequisites</span></span>
<span data-ttu-id="a8b06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8b06-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8b06-111">Permission type</span></span>|<span data-ttu-id="a8b06-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8b06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8b06-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8b06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8b06-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8b06-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8b06-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8b06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8b06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8b06-116">Not supported.</span></span>|
|<span data-ttu-id="a8b06-117">Application</span><span class="sxs-lookup"><span data-stu-id="a8b06-117">Application</span></span>|<span data-ttu-id="a8b06-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8b06-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8b06-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8b06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8b06-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b06-120">Request headers</span></span>
|<span data-ttu-id="a8b06-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8b06-121">Header</span></span>|<span data-ttu-id="a8b06-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8b06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8b06-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8b06-123">Authorization</span></span>|<span data-ttu-id="a8b06-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8b06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8b06-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8b06-125">Accept</span></span>|<span data-ttu-id="a8b06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8b06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8b06-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b06-127">Request body</span></span>
<span data-ttu-id="a8b06-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a8b06-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="a8b06-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a8b06-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="a8b06-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b06-130">Property</span></span>|<span data-ttu-id="a8b06-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b06-131">Type</span></span>|<span data-ttu-id="a8b06-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b06-133">id</span><span class="sxs-lookup"><span data-stu-id="a8b06-133">id</span></span>|<span data-ttu-id="a8b06-134">String</span><span class="sxs-lookup"><span data-stu-id="a8b06-134">String</span></span>|<span data-ttu-id="a8b06-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8b06-135">Key of the entity.</span></span> <span data-ttu-id="a8b06-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8b06-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a8b06-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8b06-138">DateTimeOffset</span></span>|<span data-ttu-id="a8b06-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a8b06-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a8b06-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8b06-141">roleScopeTagIds</span></span>|<span data-ttu-id="a8b06-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b06-142">String collection</span></span>|<span data-ttu-id="a8b06-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a8b06-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8b06-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a8b06-145">supportsScopeTags</span></span>|<span data-ttu-id="a8b06-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8b06-146">Boolean</span></span>|<span data-ttu-id="a8b06-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a8b06-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8b06-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a8b06-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8b06-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a8b06-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8b06-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8b06-150">This property is read-only.</span></span> <span data-ttu-id="a8b06-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8b06-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a8b06-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8b06-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a8b06-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a8b06-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a8b06-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8b06-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a8b06-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8b06-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a8b06-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a8b06-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a8b06-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8b06-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a8b06-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8b06-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a8b06-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a8b06-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a8b06-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8b06-164">createdDateTime</span></span>|<span data-ttu-id="a8b06-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8b06-165">DateTimeOffset</span></span>|<span data-ttu-id="a8b06-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a8b06-166">DateTime the object was created.</span></span> <span data-ttu-id="a8b06-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-168">description</span><span class="sxs-lookup"><span data-stu-id="a8b06-168">description</span></span>|<span data-ttu-id="a8b06-169">String</span><span class="sxs-lookup"><span data-stu-id="a8b06-169">String</span></span>|<span data-ttu-id="a8b06-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8b06-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8b06-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a8b06-172">displayName</span></span>|<span data-ttu-id="a8b06-173">String</span><span class="sxs-lookup"><span data-stu-id="a8b06-173">String</span></span>|<span data-ttu-id="a8b06-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8b06-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8b06-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-176">versão</span><span class="sxs-lookup"><span data-stu-id="a8b06-176">version</span></span>|<span data-ttu-id="a8b06-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b06-177">Int32</span></span>|<span data-ttu-id="a8b06-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8b06-178">Version of the device configuration.</span></span> <span data-ttu-id="a8b06-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8b06-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a8b06-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="a8b06-181">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b06-181">Int32</span></span>|<span data-ttu-id="a8b06-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="a8b06-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a8b06-183">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a8b06-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a8b06-184">keyStorageProvider</span></span>|[<span data-ttu-id="a8b06-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a8b06-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="a8b06-186">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a8b06-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8b06-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a8b06-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a8b06-188">subjectNameFormat</span></span>|[<span data-ttu-id="a8b06-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a8b06-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a8b06-190">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a8b06-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8b06-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a8b06-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a8b06-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a8b06-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a8b06-193">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="a8b06-194">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a8b06-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8b06-195">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="a8b06-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a8b06-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a8b06-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b06-197">Int32</span></span>|<span data-ttu-id="a8b06-198">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a8b06-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a8b06-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a8b06-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a8b06-200">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="a8b06-201">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a8b06-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8b06-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a8b06-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a8b06-203">extendedKeyUsages</span></span>|<span data-ttu-id="a8b06-204">coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a8b06-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="a8b06-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a8b06-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8b06-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a8b06-207">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a8b06-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="a8b06-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="a8b06-209">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="a8b06-210">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="a8b06-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="a8b06-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8b06-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a8b06-212">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a8b06-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a8b06-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a8b06-213">scepServerUrls</span></span>|<span data-ttu-id="a8b06-214">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b06-214">String collection</span></span>|<span data-ttu-id="a8b06-215">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="a8b06-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="a8b06-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a8b06-216">subjectNameFormatString</span></span>|<span data-ttu-id="a8b06-217">String</span><span class="sxs-lookup"><span data-stu-id="a8b06-217">String</span></span>|<span data-ttu-id="a8b06-218">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a8b06-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a8b06-219">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="a8b06-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a8b06-220">uso de</span><span class="sxs-lookup"><span data-stu-id="a8b06-220">keyUsage</span></span>|[<span data-ttu-id="a8b06-221">usos de</span><span class="sxs-lookup"><span data-stu-id="a8b06-221">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="a8b06-222">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="a8b06-222">SCEP Key Usage.</span></span> <span data-ttu-id="a8b06-223">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a8b06-224">keySize</span><span class="sxs-lookup"><span data-stu-id="a8b06-224">keySize</span></span>|[<span data-ttu-id="a8b06-225">keySize</span><span class="sxs-lookup"><span data-stu-id="a8b06-225">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="a8b06-226">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="a8b06-226">SCEP Key Size.</span></span> <span data-ttu-id="a8b06-227">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="a8b06-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a8b06-228">hashAlgorithm</span></span>|[<span data-ttu-id="a8b06-229">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a8b06-229">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="a8b06-230">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="a8b06-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a8b06-231">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a8b06-232">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="a8b06-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a8b06-233">String</span><span class="sxs-lookup"><span data-stu-id="a8b06-233">String</span></span>|<span data-ttu-id="a8b06-234">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="a8b06-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="a8b06-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="a8b06-235">certificateStore</span></span>|[<span data-ttu-id="a8b06-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="a8b06-236">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="a8b06-237">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="a8b06-237">Target store certificate.</span></span> <span data-ttu-id="a8b06-238">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="a8b06-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="a8b06-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8b06-239">Response</span></span>
<span data-ttu-id="a8b06-240">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8b06-240">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8b06-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8b06-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8b06-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b06-242">Request</span></span>
<span data-ttu-id="a8b06-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8b06-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="a8b06-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8b06-244">Response</span></span>
<span data-ttu-id="a8b06-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8b06-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```




