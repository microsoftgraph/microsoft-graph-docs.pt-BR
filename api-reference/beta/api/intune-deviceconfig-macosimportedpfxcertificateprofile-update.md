---
title: Atualizar macOSImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto macOSImportedPFXCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 440e18ca9258ae9a2467e18d405b930259c34118
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42745370"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="f1026-103">Atualizar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f1026-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="f1026-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1026-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1026-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1026-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1026-106">Atualiza as propriedades de um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f1026-106">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1026-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1026-107">Prerequisites</span></span>
<span data-ttu-id="f1026-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1026-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1026-110">Permission type</span></span>|<span data-ttu-id="f1026-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1026-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1026-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1026-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1026-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1026-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1026-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1026-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1026-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1026-115">Not supported.</span></span>|
|<span data-ttu-id="f1026-116">Application</span><span class="sxs-lookup"><span data-stu-id="f1026-116">Application</span></span>|<span data-ttu-id="f1026-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1026-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1026-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1026-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1026-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1026-119">Request headers</span></span>
|<span data-ttu-id="f1026-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1026-120">Header</span></span>|<span data-ttu-id="f1026-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1026-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1026-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1026-122">Authorization</span></span>|<span data-ttu-id="f1026-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1026-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1026-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1026-124">Accept</span></span>|<span data-ttu-id="f1026-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1026-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1026-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1026-126">Request body</span></span>
<span data-ttu-id="f1026-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f1026-127">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="f1026-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f1026-128">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="f1026-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1026-129">Property</span></span>|<span data-ttu-id="f1026-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1026-130">Type</span></span>|<span data-ttu-id="f1026-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1026-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1026-132">id</span><span class="sxs-lookup"><span data-stu-id="f1026-132">id</span></span>|<span data-ttu-id="f1026-133">String</span><span class="sxs-lookup"><span data-stu-id="f1026-133">String</span></span>|<span data-ttu-id="f1026-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1026-134">Key of the entity.</span></span> <span data-ttu-id="f1026-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1026-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f1026-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1026-137">DateTimeOffset</span></span>|<span data-ttu-id="f1026-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f1026-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f1026-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1026-140">roleScopeTagIds</span></span>|<span data-ttu-id="f1026-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1026-141">String collection</span></span>|<span data-ttu-id="f1026-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f1026-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1026-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1026-144">supportsScopeTags</span></span>|<span data-ttu-id="f1026-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1026-145">Boolean</span></span>|<span data-ttu-id="f1026-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f1026-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1026-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f1026-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1026-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f1026-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1026-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1026-149">This property is read-only.</span></span> <span data-ttu-id="f1026-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1026-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f1026-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1026-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f1026-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f1026-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f1026-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1026-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f1026-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1026-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f1026-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f1026-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f1026-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1026-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f1026-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1026-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f1026-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f1026-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f1026-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1026-163">createdDateTime</span></span>|<span data-ttu-id="f1026-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1026-164">DateTimeOffset</span></span>|<span data-ttu-id="f1026-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f1026-165">DateTime the object was created.</span></span> <span data-ttu-id="f1026-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-167">description</span><span class="sxs-lookup"><span data-stu-id="f1026-167">description</span></span>|<span data-ttu-id="f1026-168">String</span><span class="sxs-lookup"><span data-stu-id="f1026-168">String</span></span>|<span data-ttu-id="f1026-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1026-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1026-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f1026-171">displayName</span></span>|<span data-ttu-id="f1026-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1026-172">String</span></span>|<span data-ttu-id="f1026-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1026-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1026-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-175">versão</span><span class="sxs-lookup"><span data-stu-id="f1026-175">version</span></span>|<span data-ttu-id="f1026-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f1026-176">Int32</span></span>|<span data-ttu-id="f1026-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1026-177">Version of the device configuration.</span></span> <span data-ttu-id="f1026-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1026-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f1026-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="f1026-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f1026-180">Int32</span></span>|<span data-ttu-id="f1026-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="f1026-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f1026-182">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f1026-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f1026-183">subjectNameFormat</span></span>|[<span data-ttu-id="f1026-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f1026-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f1026-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f1026-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="f1026-186">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f1026-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f1026-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f1026-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f1026-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f1026-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f1026-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f1026-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f1026-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f1026-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f1026-191">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f1026-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f1026-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f1026-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f1026-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f1026-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f1026-194">Int32</span><span class="sxs-lookup"><span data-stu-id="f1026-194">Int32</span></span>|<span data-ttu-id="f1026-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f1026-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f1026-196">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f1026-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f1026-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f1026-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f1026-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f1026-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f1026-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f1026-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f1026-200">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f1026-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f1026-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f1026-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f1026-202">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="f1026-202">intendedPurpose</span></span>|[<span data-ttu-id="f1026-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="f1026-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="f1026-204">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="f1026-204">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="f1026-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1026-205">Response</span></span>
<span data-ttu-id="f1026-206">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1026-206">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1026-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1026-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1026-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1026-208">Request</span></span>
<span data-ttu-id="f1026-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1026-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1297

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="f1026-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1026-210">Response</span></span>
<span data-ttu-id="f1026-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1026-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1469

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




