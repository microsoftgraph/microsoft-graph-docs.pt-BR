---
title: Atualizar androidForWorkImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 474f7d8d800572a569b3d3835d5cbbd5e88b831f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43345924"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="22a32-103">Atualizar androidForWorkImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="22a32-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

<span data-ttu-id="22a32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22a32-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22a32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22a32-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22a32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a32-107">Atualiza as propriedades de um objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="22a32-107">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22a32-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22a32-108">Prerequisites</span></span>
<span data-ttu-id="22a32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a32-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22a32-111">Permission type</span></span>|<span data-ttu-id="22a32-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22a32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a32-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22a32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22a32-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22a32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a32-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a32-116">Not supported.</span></span>|
|<span data-ttu-id="22a32-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22a32-117">Application</span></span>|<span data-ttu-id="22a32-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a32-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a32-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22a32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="22a32-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22a32-120">Request headers</span></span>
|<span data-ttu-id="22a32-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22a32-121">Header</span></span>|<span data-ttu-id="22a32-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22a32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a32-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22a32-123">Authorization</span></span>|<span data-ttu-id="22a32-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22a32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a32-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22a32-125">Accept</span></span>|<span data-ttu-id="22a32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22a32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a32-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22a32-127">Request body</span></span>
<span data-ttu-id="22a32-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="22a32-128">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="22a32-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="22a32-129">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="22a32-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a32-130">Property</span></span>|<span data-ttu-id="22a32-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a32-131">Type</span></span>|<span data-ttu-id="22a32-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a32-133">id</span><span class="sxs-lookup"><span data-stu-id="22a32-133">id</span></span>|<span data-ttu-id="22a32-134">String</span><span class="sxs-lookup"><span data-stu-id="22a32-134">String</span></span>|<span data-ttu-id="22a32-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22a32-135">Key of the entity.</span></span> <span data-ttu-id="22a32-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22a32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22a32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a32-138">DateTimeOffset</span></span>|<span data-ttu-id="22a32-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22a32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22a32-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22a32-141">roleScopeTagIds</span></span>|<span data-ttu-id="22a32-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="22a32-142">String collection</span></span>|<span data-ttu-id="22a32-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="22a32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22a32-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="22a32-145">supportsScopeTags</span></span>|<span data-ttu-id="22a32-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a32-146">Boolean</span></span>|<span data-ttu-id="22a32-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="22a32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22a32-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="22a32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22a32-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="22a32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22a32-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a32-150">This property is read-only.</span></span> <span data-ttu-id="22a32-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22a32-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22a32-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22a32-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22a32-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="22a32-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22a32-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22a32-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22a32-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22a32-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22a32-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="22a32-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22a32-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22a32-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22a32-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22a32-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22a32-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="22a32-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22a32-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22a32-164">createdDateTime</span></span>|<span data-ttu-id="22a32-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a32-165">DateTimeOffset</span></span>|<span data-ttu-id="22a32-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22a32-166">DateTime the object was created.</span></span> <span data-ttu-id="22a32-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-168">description</span><span class="sxs-lookup"><span data-stu-id="22a32-168">description</span></span>|<span data-ttu-id="22a32-169">String</span><span class="sxs-lookup"><span data-stu-id="22a32-169">String</span></span>|<span data-ttu-id="22a32-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a32-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22a32-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-172">displayName</span><span class="sxs-lookup"><span data-stu-id="22a32-172">displayName</span></span>|<span data-ttu-id="22a32-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22a32-173">String</span></span>|<span data-ttu-id="22a32-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a32-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22a32-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-176">versão</span><span class="sxs-lookup"><span data-stu-id="22a32-176">version</span></span>|<span data-ttu-id="22a32-177">Int32</span><span class="sxs-lookup"><span data-stu-id="22a32-177">Int32</span></span>|<span data-ttu-id="22a32-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a32-178">Version of the device configuration.</span></span> <span data-ttu-id="22a32-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a32-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="22a32-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="22a32-181">Int32</span><span class="sxs-lookup"><span data-stu-id="22a32-181">Int32</span></span>|<span data-ttu-id="22a32-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="22a32-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="22a32-183">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="22a32-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="22a32-184">subjectNameFormat</span></span>|[<span data-ttu-id="22a32-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="22a32-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="22a32-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="22a32-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="22a32-187">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22a32-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="22a32-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="22a32-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="22a32-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="22a32-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="22a32-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="22a32-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="22a32-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="22a32-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="22a32-192">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22a32-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="22a32-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="22a32-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="22a32-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="22a32-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="22a32-195">Int32</span><span class="sxs-lookup"><span data-stu-id="22a32-195">Int32</span></span>|<span data-ttu-id="22a32-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="22a32-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="22a32-197">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="22a32-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="22a32-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="22a32-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="22a32-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="22a32-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="22a32-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="22a32-201">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22a32-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="22a32-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="22a32-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="22a32-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="22a32-203">extendedKeyUsages</span></span>|<span data-ttu-id="22a32-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="22a32-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="22a32-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="22a32-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="22a32-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="22a32-207">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="22a32-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="22a32-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="22a32-208">intendedPurpose</span></span>|[<span data-ttu-id="22a32-209">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="22a32-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="22a32-210">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="22a32-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="22a32-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a32-211">Response</span></span>
<span data-ttu-id="22a32-212">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a32-212">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a32-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22a32-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="22a32-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22a32-214">Request</span></span>
<span data-ttu-id="22a32-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22a32-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22a32-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a32-216">Response</span></span>
<span data-ttu-id="22a32-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22a32-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



