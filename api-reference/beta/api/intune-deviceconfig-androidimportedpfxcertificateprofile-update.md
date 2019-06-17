---
title: Atualizar androidImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto androidImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c13a5d5e9b0437b0c022c31437204971ba9e1358
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970111"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="b6e11-103">Atualizar androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b6e11-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="b6e11-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6e11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6e11-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6e11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6e11-106">Atualiza as propriedades de um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b6e11-106">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6e11-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6e11-107">Prerequisites</span></span>
<span data-ttu-id="b6e11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6e11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6e11-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6e11-110">Permission type</span></span>|<span data-ttu-id="b6e11-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6e11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6e11-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6e11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6e11-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e11-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6e11-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6e11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6e11-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e11-115">Not supported.</span></span>|
|<span data-ttu-id="b6e11-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6e11-116">Application</span></span>|<span data-ttu-id="b6e11-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e11-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6e11-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6e11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b6e11-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e11-119">Request headers</span></span>
|<span data-ttu-id="b6e11-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6e11-120">Header</span></span>|<span data-ttu-id="b6e11-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b6e11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6e11-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6e11-122">Authorization</span></span>|<span data-ttu-id="b6e11-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6e11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6e11-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6e11-124">Accept</span></span>|<span data-ttu-id="b6e11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6e11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6e11-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e11-126">Request body</span></span>
<span data-ttu-id="b6e11-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b6e11-127">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="b6e11-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b6e11-128">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="b6e11-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6e11-129">Property</span></span>|<span data-ttu-id="b6e11-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6e11-130">Type</span></span>|<span data-ttu-id="b6e11-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6e11-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e11-132">id</span><span class="sxs-lookup"><span data-stu-id="b6e11-132">id</span></span>|<span data-ttu-id="b6e11-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e11-133">String</span></span>|<span data-ttu-id="b6e11-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6e11-134">Key of the entity.</span></span> <span data-ttu-id="b6e11-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e11-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b6e11-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e11-137">DateTimeOffset</span></span>|<span data-ttu-id="b6e11-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b6e11-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b6e11-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6e11-140">roleScopeTagIds</span></span>|<span data-ttu-id="b6e11-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e11-141">String collection</span></span>|<span data-ttu-id="b6e11-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b6e11-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6e11-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6e11-144">supportsScopeTags</span></span>|<span data-ttu-id="b6e11-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6e11-145">Boolean</span></span>|<span data-ttu-id="b6e11-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b6e11-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b6e11-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b6e11-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b6e11-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b6e11-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b6e11-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6e11-149">This property is read-only.</span></span> <span data-ttu-id="b6e11-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6e11-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b6e11-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6e11-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b6e11-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b6e11-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b6e11-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6e11-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b6e11-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6e11-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b6e11-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b6e11-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b6e11-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b6e11-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b6e11-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b6e11-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b6e11-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b6e11-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b6e11-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e11-163">createdDateTime</span></span>|<span data-ttu-id="b6e11-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e11-164">DateTimeOffset</span></span>|<span data-ttu-id="b6e11-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-165">DateTime the object was created.</span></span> <span data-ttu-id="b6e11-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b6e11-167">description</span></span>|<span data-ttu-id="b6e11-168">String</span><span class="sxs-lookup"><span data-stu-id="b6e11-168">String</span></span>|<span data-ttu-id="b6e11-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6e11-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6e11-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b6e11-171">displayName</span></span>|<span data-ttu-id="b6e11-172">String</span><span class="sxs-lookup"><span data-stu-id="b6e11-172">String</span></span>|<span data-ttu-id="b6e11-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6e11-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6e11-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-175">versão</span><span class="sxs-lookup"><span data-stu-id="b6e11-175">version</span></span>|<span data-ttu-id="b6e11-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b6e11-176">Int32</span></span>|<span data-ttu-id="b6e11-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6e11-177">Version of the device configuration.</span></span> <span data-ttu-id="b6e11-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6e11-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b6e11-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="b6e11-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b6e11-180">Int32</span></span>|<span data-ttu-id="b6e11-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b6e11-182">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b6e11-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b6e11-183">subjectNameFormat</span></span>|[<span data-ttu-id="b6e11-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b6e11-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b6e11-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="b6e11-186">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b6e11-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b6e11-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b6e11-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b6e11-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b6e11-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b6e11-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b6e11-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b6e11-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b6e11-191">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b6e11-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b6e11-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b6e11-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b6e11-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b6e11-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b6e11-194">Int32</span><span class="sxs-lookup"><span data-stu-id="b6e11-194">Int32</span></span>|<span data-ttu-id="b6e11-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b6e11-196">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b6e11-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b6e11-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b6e11-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b6e11-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b6e11-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b6e11-200">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b6e11-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b6e11-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b6e11-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b6e11-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b6e11-202">extendedKeyUsages</span></span>|<span data-ttu-id="b6e11-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b6e11-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="b6e11-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b6e11-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b6e11-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b6e11-206">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b6e11-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b6e11-207">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="b6e11-207">intendedPurpose</span></span>|[<span data-ttu-id="b6e11-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="b6e11-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="b6e11-209">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="b6e11-209">Not yet documented.</span></span> <span data-ttu-id="b6e11-210">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="b6e11-210">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="b6e11-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e11-211">Response</span></span>
<span data-ttu-id="b6e11-212">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6e11-212">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6e11-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6e11-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6e11-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e11-214">Request</span></span>
<span data-ttu-id="b6e11-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6e11-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6e11-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e11-216">Response</span></span>
<span data-ttu-id="b6e11-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6e11-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





