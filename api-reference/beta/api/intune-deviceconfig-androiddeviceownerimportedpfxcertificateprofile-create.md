---
title: Criar androidDeviceOwnerImportedPFXCertificateProfile
description: Criar um novo objeto androidDeviceOwnerImportedPFXCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bb2dfaf4410ac7e3bb1973dba74c348880033d6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759784"
---
# <a name="create-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="36dbb-103">Criar androidDeviceOwnerImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="36dbb-103">Create androidDeviceOwnerImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="36dbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36dbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36dbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36dbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36dbb-106">Criar um novo objeto [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="36dbb-106">Create a new [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36dbb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36dbb-107">Prerequisites</span></span>
<span data-ttu-id="36dbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36dbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36dbb-110">Permission type</span></span>|<span data-ttu-id="36dbb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36dbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36dbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36dbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36dbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36dbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36dbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36dbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36dbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36dbb-115">Not supported.</span></span>|
|<span data-ttu-id="36dbb-116">Application</span><span class="sxs-lookup"><span data-stu-id="36dbb-116">Application</span></span>|<span data-ttu-id="36dbb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36dbb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36dbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36dbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36dbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36dbb-119">Request headers</span></span>
|<span data-ttu-id="36dbb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36dbb-120">Header</span></span>|<span data-ttu-id="36dbb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="36dbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36dbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="36dbb-122">Authorization</span></span>|<span data-ttu-id="36dbb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36dbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36dbb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36dbb-124">Accept</span></span>|<span data-ttu-id="36dbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36dbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36dbb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36dbb-126">Request body</span></span>
<span data-ttu-id="36dbb-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="36dbb-127">In the request body, supply a JSON representation for the androidDeviceOwnerImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="36dbb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="36dbb-128">The following table shows the properties that are required when you create the androidDeviceOwnerImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="36dbb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36dbb-129">Property</span></span>|<span data-ttu-id="36dbb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="36dbb-130">Type</span></span>|<span data-ttu-id="36dbb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="36dbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36dbb-132">id</span><span class="sxs-lookup"><span data-stu-id="36dbb-132">id</span></span>|<span data-ttu-id="36dbb-133">String</span><span class="sxs-lookup"><span data-stu-id="36dbb-133">String</span></span>|<span data-ttu-id="36dbb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="36dbb-134">Key of the entity.</span></span> <span data-ttu-id="36dbb-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36dbb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="36dbb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36dbb-137">DateTimeOffset</span></span>|<span data-ttu-id="36dbb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="36dbb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="36dbb-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36dbb-140">roleScopeTagIds</span></span>|<span data-ttu-id="36dbb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="36dbb-141">String collection</span></span>|<span data-ttu-id="36dbb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="36dbb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36dbb-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36dbb-144">supportsScopeTags</span></span>|<span data-ttu-id="36dbb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="36dbb-145">Boolean</span></span>|<span data-ttu-id="36dbb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="36dbb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36dbb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="36dbb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36dbb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="36dbb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36dbb-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36dbb-149">This property is read-only.</span></span> <span data-ttu-id="36dbb-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36dbb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="36dbb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36dbb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="36dbb-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="36dbb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="36dbb-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36dbb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="36dbb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36dbb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="36dbb-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="36dbb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="36dbb-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36dbb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="36dbb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36dbb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="36dbb-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="36dbb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="36dbb-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36dbb-163">createdDateTime</span></span>|<span data-ttu-id="36dbb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36dbb-164">DateTimeOffset</span></span>|<span data-ttu-id="36dbb-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="36dbb-165">DateTime the object was created.</span></span> <span data-ttu-id="36dbb-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-167">description</span><span class="sxs-lookup"><span data-stu-id="36dbb-167">description</span></span>|<span data-ttu-id="36dbb-168">String</span><span class="sxs-lookup"><span data-stu-id="36dbb-168">String</span></span>|<span data-ttu-id="36dbb-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36dbb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36dbb-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="36dbb-171">displayName</span></span>|<span data-ttu-id="36dbb-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36dbb-172">String</span></span>|<span data-ttu-id="36dbb-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36dbb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36dbb-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-175">versão</span><span class="sxs-lookup"><span data-stu-id="36dbb-175">version</span></span>|<span data-ttu-id="36dbb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="36dbb-176">Int32</span></span>|<span data-ttu-id="36dbb-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36dbb-177">Version of the device configuration.</span></span> <span data-ttu-id="36dbb-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dbb-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="36dbb-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="36dbb-180">Int32</span><span class="sxs-lookup"><span data-stu-id="36dbb-180">Int32</span></span>|<span data-ttu-id="36dbb-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="36dbb-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="36dbb-182">Valores válidos de 1 a 99 herdados de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-182">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="36dbb-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="36dbb-183">subjectNameFormat</span></span>|[<span data-ttu-id="36dbb-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="36dbb-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="36dbb-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="36dbb-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="36dbb-186">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="36dbb-186">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="36dbb-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="36dbb-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="36dbb-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="36dbb-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="36dbb-189">Int32</span><span class="sxs-lookup"><span data-stu-id="36dbb-189">Int32</span></span>|<span data-ttu-id="36dbb-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="36dbb-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="36dbb-191">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-191">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="36dbb-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="36dbb-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="36dbb-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="36dbb-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="36dbb-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="36dbb-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="36dbb-195">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="36dbb-195">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="36dbb-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="36dbb-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="36dbb-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="36dbb-197">extendedKeyUsages</span></span>|<span data-ttu-id="36dbb-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="36dbb-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="36dbb-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="36dbb-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="36dbb-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="36dbb-201">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="36dbb-201">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="36dbb-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="36dbb-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="36dbb-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="36dbb-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="36dbb-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="36dbb-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="36dbb-205">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="36dbb-205">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="36dbb-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="36dbb-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="36dbb-207">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="36dbb-207">intendedPurpose</span></span>|[<span data-ttu-id="36dbb-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="36dbb-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="36dbb-209">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="36dbb-209">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="36dbb-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="36dbb-210">Response</span></span>
<span data-ttu-id="36dbb-211">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36dbb-211">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36dbb-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36dbb-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="36dbb-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36dbb-213">Request</span></span>
<span data-ttu-id="36dbb-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36dbb-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36dbb-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="36dbb-215">Response</span></span>
<span data-ttu-id="36dbb-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36dbb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




