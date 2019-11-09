---
title: Criar macOSImportedPFXCertificateProfile
description: Criar um novo objeto macOSImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 365d38a519563d13babf323561ec7af334144f95
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083701"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="82a95-103">Criar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="82a95-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="82a95-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82a95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82a95-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82a95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82a95-106">Criar um novo objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="82a95-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82a95-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82a95-107">Prerequisites</span></span>
<span data-ttu-id="82a95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82a95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82a95-110">Permission type</span></span>|<span data-ttu-id="82a95-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82a95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82a95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82a95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82a95-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82a95-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82a95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82a95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82a95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82a95-115">Not supported.</span></span>|
|<span data-ttu-id="82a95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82a95-116">Application</span></span>|<span data-ttu-id="82a95-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82a95-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82a95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82a95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82a95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82a95-119">Request headers</span></span>
|<span data-ttu-id="82a95-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82a95-120">Header</span></span>|<span data-ttu-id="82a95-121">Valor</span><span class="sxs-lookup"><span data-stu-id="82a95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82a95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="82a95-122">Authorization</span></span>|<span data-ttu-id="82a95-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82a95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82a95-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82a95-124">Accept</span></span>|<span data-ttu-id="82a95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82a95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82a95-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82a95-126">Request body</span></span>
<span data-ttu-id="82a95-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="82a95-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="82a95-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="82a95-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="82a95-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82a95-129">Property</span></span>|<span data-ttu-id="82a95-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="82a95-130">Type</span></span>|<span data-ttu-id="82a95-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="82a95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82a95-132">id</span><span class="sxs-lookup"><span data-stu-id="82a95-132">id</span></span>|<span data-ttu-id="82a95-133">String</span><span class="sxs-lookup"><span data-stu-id="82a95-133">String</span></span>|<span data-ttu-id="82a95-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="82a95-134">Key of the entity.</span></span> <span data-ttu-id="82a95-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82a95-136">lastModifiedDateTime</span></span>|<span data-ttu-id="82a95-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82a95-137">DateTimeOffset</span></span>|<span data-ttu-id="82a95-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="82a95-138">DateTime the object was last modified.</span></span> <span data-ttu-id="82a95-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82a95-140">roleScopeTagIds</span></span>|<span data-ttu-id="82a95-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="82a95-141">String collection</span></span>|<span data-ttu-id="82a95-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="82a95-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82a95-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="82a95-144">supportsScopeTags</span></span>|<span data-ttu-id="82a95-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="82a95-145">Boolean</span></span>|<span data-ttu-id="82a95-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="82a95-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82a95-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="82a95-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82a95-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="82a95-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82a95-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82a95-149">This property is read-only.</span></span> <span data-ttu-id="82a95-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="82a95-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="82a95-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="82a95-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="82a95-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="82a95-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="82a95-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="82a95-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="82a95-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="82a95-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="82a95-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="82a95-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="82a95-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="82a95-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="82a95-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="82a95-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="82a95-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="82a95-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="82a95-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82a95-163">createdDateTime</span></span>|<span data-ttu-id="82a95-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82a95-164">DateTimeOffset</span></span>|<span data-ttu-id="82a95-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="82a95-165">DateTime the object was created.</span></span> <span data-ttu-id="82a95-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-167">descrição</span><span class="sxs-lookup"><span data-stu-id="82a95-167">description</span></span>|<span data-ttu-id="82a95-168">String</span><span class="sxs-lookup"><span data-stu-id="82a95-168">String</span></span>|<span data-ttu-id="82a95-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82a95-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82a95-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-171">displayName</span><span class="sxs-lookup"><span data-stu-id="82a95-171">displayName</span></span>|<span data-ttu-id="82a95-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82a95-172">String</span></span>|<span data-ttu-id="82a95-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82a95-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82a95-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-175">versão</span><span class="sxs-lookup"><span data-stu-id="82a95-175">version</span></span>|<span data-ttu-id="82a95-176">Int32</span><span class="sxs-lookup"><span data-stu-id="82a95-176">Int32</span></span>|<span data-ttu-id="82a95-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82a95-177">Version of the device configuration.</span></span> <span data-ttu-id="82a95-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82a95-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="82a95-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="82a95-180">Int32</span><span class="sxs-lookup"><span data-stu-id="82a95-180">Int32</span></span>|<span data-ttu-id="82a95-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="82a95-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="82a95-182">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="82a95-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="82a95-183">subjectNameFormat</span></span>|[<span data-ttu-id="82a95-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="82a95-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="82a95-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="82a95-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="82a95-186">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="82a95-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="82a95-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="82a95-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="82a95-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="82a95-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="82a95-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="82a95-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="82a95-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="82a95-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="82a95-191">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="82a95-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="82a95-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="82a95-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="82a95-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="82a95-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="82a95-194">Int32</span><span class="sxs-lookup"><span data-stu-id="82a95-194">Int32</span></span>|<span data-ttu-id="82a95-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="82a95-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="82a95-196">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="82a95-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="82a95-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="82a95-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="82a95-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="82a95-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="82a95-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="82a95-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="82a95-200">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="82a95-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="82a95-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="82a95-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="82a95-202">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="82a95-202">intendedPurpose</span></span>|[<span data-ttu-id="82a95-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="82a95-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="82a95-204">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="82a95-204">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="82a95-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="82a95-205">Response</span></span>
<span data-ttu-id="82a95-206">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82a95-206">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82a95-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82a95-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="82a95-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82a95-208">Request</span></span>
<span data-ttu-id="82a95-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82a95-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="82a95-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="82a95-210">Response</span></span>
<span data-ttu-id="82a95-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82a95-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






