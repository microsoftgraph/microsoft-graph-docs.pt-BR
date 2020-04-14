---
title: Criar windows81SCEPCertificateProfile
description: Criar um novo objeto windows81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8eedf4b5ec94812fbfcb5ff25fa8bf754f89b24
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430320"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="c3475-103">Criar windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c3475-103">Create windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="c3475-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3475-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3475-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3475-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3475-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3475-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3475-107">Criar um novo objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c3475-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3475-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3475-108">Prerequisites</span></span>
<span data-ttu-id="c3475-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3475-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3475-111">Permission type</span></span>|<span data-ttu-id="c3475-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c3475-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3475-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3475-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3475-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3475-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3475-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3475-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3475-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3475-116">Not supported.</span></span>|
|<span data-ttu-id="c3475-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3475-117">Application</span></span>|<span data-ttu-id="c3475-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3475-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3475-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3475-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3475-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3475-120">Request headers</span></span>
|<span data-ttu-id="c3475-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3475-121">Header</span></span>|<span data-ttu-id="c3475-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c3475-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3475-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3475-123">Authorization</span></span>|<span data-ttu-id="c3475-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3475-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3475-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3475-125">Accept</span></span>|<span data-ttu-id="c3475-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3475-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3475-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3475-127">Request body</span></span>
<span data-ttu-id="c3475-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c3475-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="c3475-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c3475-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="c3475-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3475-130">Property</span></span>|<span data-ttu-id="c3475-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3475-131">Type</span></span>|<span data-ttu-id="c3475-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3475-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3475-133">id</span><span class="sxs-lookup"><span data-stu-id="c3475-133">id</span></span>|<span data-ttu-id="c3475-134">String</span><span class="sxs-lookup"><span data-stu-id="c3475-134">String</span></span>|<span data-ttu-id="c3475-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c3475-135">Key of the entity.</span></span> <span data-ttu-id="c3475-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3475-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c3475-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3475-138">DateTimeOffset</span></span>|<span data-ttu-id="c3475-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c3475-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c3475-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3475-141">roleScopeTagIds</span></span>|<span data-ttu-id="c3475-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c3475-142">String collection</span></span>|<span data-ttu-id="c3475-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c3475-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3475-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c3475-145">supportsScopeTags</span></span>|<span data-ttu-id="c3475-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3475-146">Boolean</span></span>|<span data-ttu-id="c3475-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c3475-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c3475-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c3475-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c3475-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c3475-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c3475-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3475-150">This property is read-only.</span></span> <span data-ttu-id="c3475-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3475-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c3475-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3475-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c3475-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c3475-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c3475-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3475-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c3475-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3475-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c3475-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c3475-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c3475-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c3475-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c3475-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c3475-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c3475-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c3475-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c3475-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3475-164">createdDateTime</span></span>|<span data-ttu-id="c3475-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3475-165">DateTimeOffset</span></span>|<span data-ttu-id="c3475-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c3475-166">DateTime the object was created.</span></span> <span data-ttu-id="c3475-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-168">description</span><span class="sxs-lookup"><span data-stu-id="c3475-168">description</span></span>|<span data-ttu-id="c3475-169">String</span><span class="sxs-lookup"><span data-stu-id="c3475-169">String</span></span>|<span data-ttu-id="c3475-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3475-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3475-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c3475-172">displayName</span></span>|<span data-ttu-id="c3475-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3475-173">String</span></span>|<span data-ttu-id="c3475-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3475-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3475-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-176">versão</span><span class="sxs-lookup"><span data-stu-id="c3475-176">version</span></span>|<span data-ttu-id="c3475-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c3475-177">Int32</span></span>|<span data-ttu-id="c3475-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3475-178">Version of the device configuration.</span></span> <span data-ttu-id="c3475-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3475-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c3475-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c3475-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c3475-181">Int32</span></span>|<span data-ttu-id="c3475-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="c3475-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c3475-183">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3475-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="c3475-184">keyStorageProvider</span></span>|[<span data-ttu-id="c3475-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="c3475-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="c3475-186">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3475-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c3475-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="c3475-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="c3475-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c3475-188">subjectNameFormat</span></span>|[<span data-ttu-id="c3475-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c3475-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c3475-190">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3475-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c3475-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c3475-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c3475-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c3475-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c3475-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c3475-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c3475-194">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3475-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c3475-195">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c3475-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c3475-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c3475-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c3475-197">Int32</span><span class="sxs-lookup"><span data-stu-id="c3475-197">Int32</span></span>|<span data-ttu-id="c3475-198">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3475-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c3475-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c3475-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c3475-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c3475-201">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3475-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c3475-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c3475-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c3475-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c3475-203">extendedKeyUsages</span></span>|<span data-ttu-id="c3475-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c3475-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="c3475-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c3475-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c3475-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c3475-207">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3475-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="c3475-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="c3475-209">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="c3475-210">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="c3475-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="c3475-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c3475-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c3475-212">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3475-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3475-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c3475-213">scepServerUrls</span></span>|<span data-ttu-id="c3475-214">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c3475-214">String collection</span></span>|<span data-ttu-id="c3475-215">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3475-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="c3475-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c3475-216">subjectNameFormatString</span></span>|<span data-ttu-id="c3475-217">String</span><span class="sxs-lookup"><span data-stu-id="c3475-217">String</span></span>|<span data-ttu-id="c3475-218">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="c3475-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c3475-219">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="c3475-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c3475-220">uso de</span><span class="sxs-lookup"><span data-stu-id="c3475-220">keyUsage</span></span>|[<span data-ttu-id="c3475-221">usos de</span><span class="sxs-lookup"><span data-stu-id="c3475-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c3475-222">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3475-222">SCEP Key Usage.</span></span> <span data-ttu-id="c3475-223">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c3475-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c3475-224">keySize</span><span class="sxs-lookup"><span data-stu-id="c3475-224">keySize</span></span>|[<span data-ttu-id="c3475-225">keySize</span><span class="sxs-lookup"><span data-stu-id="c3475-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c3475-226">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3475-226">SCEP Key Size.</span></span> <span data-ttu-id="c3475-227">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="c3475-227">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c3475-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c3475-228">hashAlgorithm</span></span>|[<span data-ttu-id="c3475-229">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c3475-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="c3475-230">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3475-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c3475-231">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c3475-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c3475-232">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="c3475-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c3475-233">String</span><span class="sxs-lookup"><span data-stu-id="c3475-233">String</span></span>|<span data-ttu-id="c3475-234">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="c3475-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c3475-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c3475-235">certificateStore</span></span>|[<span data-ttu-id="c3475-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c3475-236">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="c3475-237">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="c3475-237">Target store certificate.</span></span> <span data-ttu-id="c3475-238">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="c3475-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3475-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3475-239">Response</span></span>
<span data-ttu-id="c3475-240">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3475-240">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3475-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3475-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3475-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3475-242">Request</span></span>
<span data-ttu-id="c3475-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3475-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3475-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3475-244">Response</span></span>
<span data-ttu-id="c3475-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3475-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



