---
title: Criar windows81SCEPCertificateProfile
description: Criar um novo objeto windows81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7aa1a220e581076005b010995496afb1e8931cdb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977783"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="f135c-103">Criar windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f135c-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="f135c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f135c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f135c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f135c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f135c-106">Criar um novo objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f135c-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f135c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f135c-107">Prerequisites</span></span>
<span data-ttu-id="f135c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f135c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f135c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f135c-110">Permission type</span></span>|<span data-ttu-id="f135c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f135c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f135c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f135c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f135c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f135c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f135c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f135c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f135c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f135c-115">Not supported.</span></span>|
|<span data-ttu-id="f135c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f135c-116">Application</span></span>|<span data-ttu-id="f135c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f135c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f135c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f135c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f135c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f135c-119">Request headers</span></span>
|<span data-ttu-id="f135c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f135c-120">Header</span></span>|<span data-ttu-id="f135c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f135c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f135c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f135c-122">Authorization</span></span>|<span data-ttu-id="f135c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f135c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f135c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f135c-124">Accept</span></span>|<span data-ttu-id="f135c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f135c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f135c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f135c-126">Request body</span></span>
<span data-ttu-id="f135c-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f135c-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="f135c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f135c-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="f135c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f135c-129">Property</span></span>|<span data-ttu-id="f135c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f135c-130">Type</span></span>|<span data-ttu-id="f135c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f135c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f135c-132">id</span><span class="sxs-lookup"><span data-stu-id="f135c-132">id</span></span>|<span data-ttu-id="f135c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f135c-133">String</span></span>|<span data-ttu-id="f135c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f135c-134">Key of the entity.</span></span> <span data-ttu-id="f135c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f135c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f135c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f135c-137">DateTimeOffset</span></span>|<span data-ttu-id="f135c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f135c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f135c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f135c-140">roleScopeTagIds</span></span>|<span data-ttu-id="f135c-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f135c-141">String collection</span></span>|<span data-ttu-id="f135c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f135c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f135c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f135c-144">supportsScopeTags</span></span>|<span data-ttu-id="f135c-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="f135c-145">Boolean</span></span>|<span data-ttu-id="f135c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f135c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f135c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f135c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f135c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f135c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f135c-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f135c-149">This property is read-only.</span></span> <span data-ttu-id="f135c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f135c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f135c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f135c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f135c-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f135c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f135c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f135c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f135c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f135c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f135c-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f135c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f135c-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f135c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f135c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f135c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f135c-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f135c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f135c-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f135c-163">createdDateTime</span></span>|<span data-ttu-id="f135c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f135c-164">DateTimeOffset</span></span>|<span data-ttu-id="f135c-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f135c-165">DateTime the object was created.</span></span> <span data-ttu-id="f135c-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-167">descrição</span><span class="sxs-lookup"><span data-stu-id="f135c-167">description</span></span>|<span data-ttu-id="f135c-168">String</span><span class="sxs-lookup"><span data-stu-id="f135c-168">String</span></span>|<span data-ttu-id="f135c-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f135c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f135c-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f135c-171">displayName</span></span>|<span data-ttu-id="f135c-172">String</span><span class="sxs-lookup"><span data-stu-id="f135c-172">String</span></span>|<span data-ttu-id="f135c-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f135c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f135c-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-175">versão</span><span class="sxs-lookup"><span data-stu-id="f135c-175">version</span></span>|<span data-ttu-id="f135c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f135c-176">Int32</span></span>|<span data-ttu-id="f135c-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f135c-177">Version of the device configuration.</span></span> <span data-ttu-id="f135c-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f135c-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f135c-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="f135c-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f135c-180">Int32</span></span>|<span data-ttu-id="f135c-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="f135c-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f135c-182">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f135c-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f135c-183">keyStorageProvider</span></span>|[<span data-ttu-id="f135c-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f135c-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f135c-185">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f135c-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f135c-186">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="f135c-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f135c-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f135c-187">subjectNameFormat</span></span>|[<span data-ttu-id="f135c-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f135c-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f135c-189">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f135c-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f135c-190">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f135c-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f135c-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f135c-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f135c-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f135c-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f135c-193">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f135c-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f135c-194">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f135c-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f135c-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f135c-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f135c-196">Int32</span><span class="sxs-lookup"><span data-stu-id="f135c-196">Int32</span></span>|<span data-ttu-id="f135c-197">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f135c-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f135c-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f135c-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f135c-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f135c-200">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f135c-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f135c-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f135c-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f135c-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f135c-202">extendedKeyUsages</span></span>|<span data-ttu-id="f135c-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f135c-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="f135c-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f135c-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f135c-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f135c-206">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-206">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f135c-207">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f135c-207">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f135c-208">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-208">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f135c-209">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="f135c-209">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f135c-210">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f135c-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f135c-211">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f135c-211">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f135c-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f135c-212">scepServerUrls</span></span>|<span data-ttu-id="f135c-213">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f135c-213">String collection</span></span>|<span data-ttu-id="f135c-214">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="f135c-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f135c-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f135c-215">subjectNameFormatString</span></span>|<span data-ttu-id="f135c-216">String</span><span class="sxs-lookup"><span data-stu-id="f135c-216">String</span></span>|<span data-ttu-id="f135c-217">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="f135c-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f135c-218">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="f135c-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f135c-219">uso de</span><span class="sxs-lookup"><span data-stu-id="f135c-219">keyUsage</span></span>|[<span data-ttu-id="f135c-220">usos de</span><span class="sxs-lookup"><span data-stu-id="f135c-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f135c-221">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f135c-221">SCEP Key Usage.</span></span> <span data-ttu-id="f135c-222">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f135c-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f135c-223">keySize</span><span class="sxs-lookup"><span data-stu-id="f135c-223">keySize</span></span>|[<span data-ttu-id="f135c-224">keySize</span><span class="sxs-lookup"><span data-stu-id="f135c-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f135c-225">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="f135c-225">SCEP Key Size.</span></span> <span data-ttu-id="f135c-226">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="f135c-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f135c-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f135c-227">hashAlgorithm</span></span>|[<span data-ttu-id="f135c-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f135c-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f135c-229">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f135c-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f135c-230">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f135c-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f135c-231">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="f135c-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f135c-232">String</span><span class="sxs-lookup"><span data-stu-id="f135c-232">String</span></span>|<span data-ttu-id="f135c-233">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="f135c-233">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f135c-234">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f135c-234">certificateStore</span></span>|[<span data-ttu-id="f135c-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f135c-235">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f135c-236">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="f135c-236">Target store certificate.</span></span> <span data-ttu-id="f135c-237">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="f135c-237">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="f135c-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="f135c-238">Response</span></span>
<span data-ttu-id="f135c-239">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f135c-239">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f135c-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f135c-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="f135c-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f135c-241">Request</span></span>
<span data-ttu-id="f135c-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f135c-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f135c-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="f135c-243">Response</span></span>
<span data-ttu-id="f135c-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f135c-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





