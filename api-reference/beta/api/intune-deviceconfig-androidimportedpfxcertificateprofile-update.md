---
title: Atualizar androidImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto androidImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c97e692b660317d70320ac88175eb9c686ebb534
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084787"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="50d61-103">Atualizar androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="50d61-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="50d61-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50d61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50d61-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50d61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50d61-106">Atualiza as propriedades de um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="50d61-106">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50d61-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50d61-107">Prerequisites</span></span>
<span data-ttu-id="50d61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50d61-110">Permission type</span></span>|<span data-ttu-id="50d61-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50d61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50d61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50d61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50d61-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d61-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50d61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50d61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50d61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50d61-115">Not supported.</span></span>|
|<span data-ttu-id="50d61-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50d61-116">Application</span></span>|<span data-ttu-id="50d61-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d61-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50d61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50d61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="50d61-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50d61-119">Request headers</span></span>
|<span data-ttu-id="50d61-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50d61-120">Header</span></span>|<span data-ttu-id="50d61-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50d61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50d61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50d61-122">Authorization</span></span>|<span data-ttu-id="50d61-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50d61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50d61-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50d61-124">Accept</span></span>|<span data-ttu-id="50d61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50d61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50d61-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50d61-126">Request body</span></span>
<span data-ttu-id="50d61-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="50d61-127">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="50d61-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="50d61-128">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="50d61-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50d61-129">Property</span></span>|<span data-ttu-id="50d61-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50d61-130">Type</span></span>|<span data-ttu-id="50d61-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50d61-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50d61-132">id</span><span class="sxs-lookup"><span data-stu-id="50d61-132">id</span></span>|<span data-ttu-id="50d61-133">String</span><span class="sxs-lookup"><span data-stu-id="50d61-133">String</span></span>|<span data-ttu-id="50d61-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50d61-134">Key of the entity.</span></span> <span data-ttu-id="50d61-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50d61-136">lastModifiedDateTime</span></span>|<span data-ttu-id="50d61-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d61-137">DateTimeOffset</span></span>|<span data-ttu-id="50d61-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="50d61-138">DateTime the object was last modified.</span></span> <span data-ttu-id="50d61-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50d61-140">roleScopeTagIds</span></span>|<span data-ttu-id="50d61-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="50d61-141">String collection</span></span>|<span data-ttu-id="50d61-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="50d61-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50d61-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="50d61-144">supportsScopeTags</span></span>|<span data-ttu-id="50d61-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="50d61-145">Boolean</span></span>|<span data-ttu-id="50d61-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="50d61-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50d61-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="50d61-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50d61-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="50d61-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50d61-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50d61-149">This property is read-only.</span></span> <span data-ttu-id="50d61-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50d61-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="50d61-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50d61-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="50d61-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="50d61-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="50d61-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50d61-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="50d61-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50d61-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="50d61-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="50d61-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="50d61-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="50d61-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="50d61-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="50d61-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="50d61-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="50d61-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="50d61-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50d61-163">createdDateTime</span></span>|<span data-ttu-id="50d61-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d61-164">DateTimeOffset</span></span>|<span data-ttu-id="50d61-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="50d61-165">DateTime the object was created.</span></span> <span data-ttu-id="50d61-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-167">descrição</span><span class="sxs-lookup"><span data-stu-id="50d61-167">description</span></span>|<span data-ttu-id="50d61-168">String</span><span class="sxs-lookup"><span data-stu-id="50d61-168">String</span></span>|<span data-ttu-id="50d61-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50d61-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50d61-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-171">displayName</span><span class="sxs-lookup"><span data-stu-id="50d61-171">displayName</span></span>|<span data-ttu-id="50d61-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50d61-172">String</span></span>|<span data-ttu-id="50d61-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50d61-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50d61-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-175">versão</span><span class="sxs-lookup"><span data-stu-id="50d61-175">version</span></span>|<span data-ttu-id="50d61-176">Int32</span><span class="sxs-lookup"><span data-stu-id="50d61-176">Int32</span></span>|<span data-ttu-id="50d61-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50d61-177">Version of the device configuration.</span></span> <span data-ttu-id="50d61-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d61-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="50d61-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="50d61-180">Int32</span><span class="sxs-lookup"><span data-stu-id="50d61-180">Int32</span></span>|<span data-ttu-id="50d61-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="50d61-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="50d61-182">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50d61-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="50d61-183">subjectNameFormat</span></span>|[<span data-ttu-id="50d61-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="50d61-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="50d61-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50d61-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="50d61-186">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50d61-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="50d61-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="50d61-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="50d61-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="50d61-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="50d61-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="50d61-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="50d61-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50d61-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="50d61-191">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50d61-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="50d61-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="50d61-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="50d61-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="50d61-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="50d61-194">Int32</span><span class="sxs-lookup"><span data-stu-id="50d61-194">Int32</span></span>|<span data-ttu-id="50d61-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50d61-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="50d61-196">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50d61-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="50d61-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="50d61-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="50d61-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="50d61-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50d61-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="50d61-200">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50d61-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="50d61-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="50d61-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="50d61-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="50d61-202">extendedKeyUsages</span></span>|<span data-ttu-id="50d61-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="50d61-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="50d61-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="50d61-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="50d61-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="50d61-206">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50d61-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50d61-207">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="50d61-207">intendedPurpose</span></span>|[<span data-ttu-id="50d61-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="50d61-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="50d61-209">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="50d61-209">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="50d61-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d61-210">Response</span></span>
<span data-ttu-id="50d61-211">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50d61-211">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d61-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50d61-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="50d61-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50d61-213">Request</span></span>
<span data-ttu-id="50d61-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50d61-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1492

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="50d61-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d61-215">Response</span></span>
<span data-ttu-id="50d61-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50d61-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```






