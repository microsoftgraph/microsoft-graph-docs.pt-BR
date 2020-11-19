---
title: Criar androidDeviceOwnerImportedPFXCertificateProfile
description: Criar um novo objeto androidDeviceOwnerImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29de44f7d88b01c9b0453dd5b318b98dc9546c59
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240828"
---
# <a name="create-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="54454-103">Criar androidDeviceOwnerImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="54454-103">Create androidDeviceOwnerImportedPFXCertificateProfile</span></span>

<span data-ttu-id="54454-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54454-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54454-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54454-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54454-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54454-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54454-107">Criar um novo objeto [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="54454-107">Create a new [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54454-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54454-108">Prerequisites</span></span>
<span data-ttu-id="54454-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54454-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54454-111">Permission type</span></span>|<span data-ttu-id="54454-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54454-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54454-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54454-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54454-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54454-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54454-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54454-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54454-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54454-116">Not supported.</span></span>|
|<span data-ttu-id="54454-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54454-117">Application</span></span>|<span data-ttu-id="54454-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54454-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54454-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54454-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54454-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54454-120">Request headers</span></span>
|<span data-ttu-id="54454-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54454-121">Header</span></span>|<span data-ttu-id="54454-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54454-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54454-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54454-123">Authorization</span></span>|<span data-ttu-id="54454-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54454-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54454-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54454-125">Accept</span></span>|<span data-ttu-id="54454-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54454-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54454-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54454-127">Request body</span></span>
<span data-ttu-id="54454-128">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="54454-128">In the request body, supply a JSON representation for the androidDeviceOwnerImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="54454-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="54454-129">The following table shows the properties that are required when you create the androidDeviceOwnerImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="54454-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54454-130">Property</span></span>|<span data-ttu-id="54454-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54454-131">Type</span></span>|<span data-ttu-id="54454-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54454-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54454-133">id</span><span class="sxs-lookup"><span data-stu-id="54454-133">id</span></span>|<span data-ttu-id="54454-134">String</span><span class="sxs-lookup"><span data-stu-id="54454-134">String</span></span>|<span data-ttu-id="54454-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54454-135">Key of the entity.</span></span> <span data-ttu-id="54454-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54454-137">lastModifiedDateTime</span></span>|<span data-ttu-id="54454-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54454-138">DateTimeOffset</span></span>|<span data-ttu-id="54454-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="54454-139">DateTime the object was last modified.</span></span> <span data-ttu-id="54454-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54454-141">roleScopeTagIds</span></span>|<span data-ttu-id="54454-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54454-142">String collection</span></span>|<span data-ttu-id="54454-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="54454-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54454-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54454-145">supportsScopeTags</span></span>|<span data-ttu-id="54454-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="54454-146">Boolean</span></span>|<span data-ttu-id="54454-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="54454-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54454-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="54454-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54454-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="54454-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54454-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54454-150">This property is read-only.</span></span> <span data-ttu-id="54454-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54454-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="54454-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54454-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="54454-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="54454-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="54454-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54454-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="54454-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54454-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="54454-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="54454-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="54454-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54454-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="54454-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54454-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="54454-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="54454-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="54454-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54454-164">createdDateTime</span></span>|<span data-ttu-id="54454-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54454-165">DateTimeOffset</span></span>|<span data-ttu-id="54454-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="54454-166">DateTime the object was created.</span></span> <span data-ttu-id="54454-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-168">description</span><span class="sxs-lookup"><span data-stu-id="54454-168">description</span></span>|<span data-ttu-id="54454-169">String</span><span class="sxs-lookup"><span data-stu-id="54454-169">String</span></span>|<span data-ttu-id="54454-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54454-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54454-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-172">displayName</span><span class="sxs-lookup"><span data-stu-id="54454-172">displayName</span></span>|<span data-ttu-id="54454-173">String</span><span class="sxs-lookup"><span data-stu-id="54454-173">String</span></span>|<span data-ttu-id="54454-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54454-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54454-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-176">versão</span><span class="sxs-lookup"><span data-stu-id="54454-176">version</span></span>|<span data-ttu-id="54454-177">Int32</span><span class="sxs-lookup"><span data-stu-id="54454-177">Int32</span></span>|<span data-ttu-id="54454-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54454-178">Version of the device configuration.</span></span> <span data-ttu-id="54454-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54454-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54454-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="54454-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="54454-181">Int32</span><span class="sxs-lookup"><span data-stu-id="54454-181">Int32</span></span>|<span data-ttu-id="54454-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="54454-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="54454-183">Valores válidos de 1 a 99 herdados de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="54454-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="54454-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="54454-184">subjectNameFormat</span></span>|[<span data-ttu-id="54454-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="54454-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="54454-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="54454-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="54454-187">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="54454-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="54454-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="54454-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="54454-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="54454-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="54454-190">Int32</span><span class="sxs-lookup"><span data-stu-id="54454-190">Int32</span></span>|<span data-ttu-id="54454-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="54454-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="54454-192">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="54454-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="54454-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="54454-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="54454-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="54454-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="54454-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="54454-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="54454-196">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="54454-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="54454-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="54454-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="54454-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="54454-198">extendedKeyUsages</span></span>|<span data-ttu-id="54454-199">coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="54454-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="54454-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="54454-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="54454-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="54454-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="54454-202">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="54454-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="54454-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="54454-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="54454-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="54454-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="54454-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="54454-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="54454-206">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="54454-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="54454-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="54454-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="54454-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="54454-208">intendedPurpose</span></span>|[<span data-ttu-id="54454-209">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="54454-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="54454-210">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são: `unassigned` , `smimeEncryption` , `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="54454-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="54454-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="54454-211">Response</span></span>
<span data-ttu-id="54454-212">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54454-212">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54454-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54454-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="54454-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54454-214">Request</span></span>
<span data-ttu-id="54454-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54454-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1503

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="54454-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="54454-216">Response</span></span>
<span data-ttu-id="54454-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54454-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1675

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
  "id": "8d46d3c7-d3c7-8d46-c7d3-468dc7d3468d",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "intendedPurpose": "smimeEncryption"
}
```




