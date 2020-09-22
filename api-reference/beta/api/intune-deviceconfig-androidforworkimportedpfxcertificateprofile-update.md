---
title: Atualizar androidForWorkImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 203a8add84bce7e43528387e9bcea7fb7e0da1d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005534"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="41e44-103">Atualizar androidForWorkImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="41e44-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

<span data-ttu-id="41e44-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="41e44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41e44-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41e44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41e44-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41e44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41e44-107">Atualiza as propriedades de um objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="41e44-107">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41e44-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41e44-108">Prerequisites</span></span>
<span data-ttu-id="41e44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41e44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e44-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41e44-111">Permission type</span></span>|<span data-ttu-id="41e44-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41e44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e44-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41e44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41e44-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e44-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41e44-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41e44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41e44-116">Not supported.</span></span>|
|<span data-ttu-id="41e44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41e44-117">Application</span></span>|<span data-ttu-id="41e44-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e44-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41e44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="41e44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41e44-120">Request headers</span></span>
|<span data-ttu-id="41e44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41e44-121">Header</span></span>|<span data-ttu-id="41e44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41e44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41e44-123">Authorization</span></span>|<span data-ttu-id="41e44-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41e44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e44-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41e44-125">Accept</span></span>|<span data-ttu-id="41e44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41e44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41e44-127">Request body</span></span>
<span data-ttu-id="41e44-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="41e44-128">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="41e44-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="41e44-129">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="41e44-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41e44-130">Property</span></span>|<span data-ttu-id="41e44-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="41e44-131">Type</span></span>|<span data-ttu-id="41e44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="41e44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e44-133">id</span><span class="sxs-lookup"><span data-stu-id="41e44-133">id</span></span>|<span data-ttu-id="41e44-134">String</span><span class="sxs-lookup"><span data-stu-id="41e44-134">String</span></span>|<span data-ttu-id="41e44-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="41e44-135">Key of the entity.</span></span> <span data-ttu-id="41e44-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41e44-137">lastModifiedDateTime</span></span>|<span data-ttu-id="41e44-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41e44-138">DateTimeOffset</span></span>|<span data-ttu-id="41e44-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="41e44-139">DateTime the object was last modified.</span></span> <span data-ttu-id="41e44-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41e44-141">roleScopeTagIds</span></span>|<span data-ttu-id="41e44-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="41e44-142">String collection</span></span>|<span data-ttu-id="41e44-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="41e44-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41e44-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="41e44-145">supportsScopeTags</span></span>|<span data-ttu-id="41e44-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="41e44-146">Boolean</span></span>|<span data-ttu-id="41e44-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="41e44-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="41e44-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="41e44-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="41e44-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="41e44-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="41e44-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41e44-150">This property is read-only.</span></span> <span data-ttu-id="41e44-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41e44-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="41e44-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41e44-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="41e44-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="41e44-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="41e44-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41e44-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="41e44-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41e44-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="41e44-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="41e44-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="41e44-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="41e44-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="41e44-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="41e44-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="41e44-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="41e44-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="41e44-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41e44-164">createdDateTime</span></span>|<span data-ttu-id="41e44-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41e44-165">DateTimeOffset</span></span>|<span data-ttu-id="41e44-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="41e44-166">DateTime the object was created.</span></span> <span data-ttu-id="41e44-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-168">description</span><span class="sxs-lookup"><span data-stu-id="41e44-168">description</span></span>|<span data-ttu-id="41e44-169">String</span><span class="sxs-lookup"><span data-stu-id="41e44-169">String</span></span>|<span data-ttu-id="41e44-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41e44-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41e44-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-172">displayName</span><span class="sxs-lookup"><span data-stu-id="41e44-172">displayName</span></span>|<span data-ttu-id="41e44-173">String</span><span class="sxs-lookup"><span data-stu-id="41e44-173">String</span></span>|<span data-ttu-id="41e44-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41e44-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41e44-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-176">versão</span><span class="sxs-lookup"><span data-stu-id="41e44-176">version</span></span>|<span data-ttu-id="41e44-177">Int32</span><span class="sxs-lookup"><span data-stu-id="41e44-177">Int32</span></span>|<span data-ttu-id="41e44-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41e44-178">Version of the device configuration.</span></span> <span data-ttu-id="41e44-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e44-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="41e44-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="41e44-181">Int32</span><span class="sxs-lookup"><span data-stu-id="41e44-181">Int32</span></span>|<span data-ttu-id="41e44-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="41e44-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="41e44-183">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="41e44-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="41e44-184">subjectNameFormat</span></span>|[<span data-ttu-id="41e44-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="41e44-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="41e44-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="41e44-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="41e44-187">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="41e44-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="41e44-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="41e44-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="41e44-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="41e44-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="41e44-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="41e44-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="41e44-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="41e44-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="41e44-192">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="41e44-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="41e44-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="41e44-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="41e44-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="41e44-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="41e44-195">Int32</span><span class="sxs-lookup"><span data-stu-id="41e44-195">Int32</span></span>|<span data-ttu-id="41e44-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="41e44-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="41e44-197">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="41e44-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="41e44-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="41e44-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="41e44-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="41e44-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="41e44-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="41e44-201">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="41e44-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="41e44-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="41e44-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="41e44-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="41e44-203">extendedKeyUsages</span></span>|<span data-ttu-id="41e44-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="41e44-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="41e44-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="41e44-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="41e44-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="41e44-207">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="41e44-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="41e44-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="41e44-208">intendedPurpose</span></span>|[<span data-ttu-id="41e44-209">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="41e44-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="41e44-210">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são: `unassigned` , `smimeEncryption` , `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="41e44-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="41e44-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="41e44-211">Response</span></span>
<span data-ttu-id="41e44-212">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41e44-212">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e44-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41e44-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="41e44-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41e44-214">Request</span></span>
<span data-ttu-id="41e44-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41e44-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="41e44-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="41e44-216">Response</span></span>
<span data-ttu-id="41e44-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41e44-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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






