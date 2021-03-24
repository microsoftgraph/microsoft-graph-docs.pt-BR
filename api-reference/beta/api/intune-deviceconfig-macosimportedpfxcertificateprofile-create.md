---
title: Criar macOSImportedPFXCertificateProfile
description: Crie um novo objeto macOSImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b1a35785b9c837cfc6e6dd87e56407b281923a5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129787"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="62fab-103">Criar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="62fab-103">Create macOSImportedPFXCertificateProfile</span></span>

<span data-ttu-id="62fab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62fab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62fab-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62fab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62fab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62fab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62fab-107">Crie um novo [objeto macOSImportedPFXCertificateProfile.](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62fab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62fab-108">Prerequisites</span></span>
<span data-ttu-id="62fab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62fab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62fab-111">Permission type</span></span>|<span data-ttu-id="62fab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62fab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62fab-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62fab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62fab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62fab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62fab-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62fab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62fab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62fab-116">Not supported.</span></span>|
|<span data-ttu-id="62fab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62fab-117">Application</span></span>|<span data-ttu-id="62fab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62fab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62fab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62fab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="62fab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62fab-120">Request headers</span></span>
|<span data-ttu-id="62fab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62fab-121">Header</span></span>|<span data-ttu-id="62fab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62fab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62fab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62fab-123">Authorization</span></span>|<span data-ttu-id="62fab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62fab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62fab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62fab-125">Accept</span></span>|<span data-ttu-id="62fab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62fab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62fab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62fab-127">Request body</span></span>
<span data-ttu-id="62fab-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="62fab-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="62fab-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="62fab-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="62fab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62fab-130">Property</span></span>|<span data-ttu-id="62fab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62fab-131">Type</span></span>|<span data-ttu-id="62fab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62fab-133">id</span><span class="sxs-lookup"><span data-stu-id="62fab-133">id</span></span>|<span data-ttu-id="62fab-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62fab-134">String</span></span>|<span data-ttu-id="62fab-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62fab-135">Key of the entity.</span></span> <span data-ttu-id="62fab-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62fab-137">lastModifiedDateTime</span></span>|<span data-ttu-id="62fab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62fab-138">DateTimeOffset</span></span>|<span data-ttu-id="62fab-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="62fab-139">DateTime the object was last modified.</span></span> <span data-ttu-id="62fab-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62fab-141">roleScopeTagIds</span></span>|<span data-ttu-id="62fab-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="62fab-142">String collection</span></span>|<span data-ttu-id="62fab-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="62fab-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62fab-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62fab-145">supportsScopeTags</span></span>|<span data-ttu-id="62fab-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="62fab-146">Boolean</span></span>|<span data-ttu-id="62fab-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="62fab-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62fab-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="62fab-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62fab-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="62fab-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62fab-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62fab-150">This property is read-only.</span></span> <span data-ttu-id="62fab-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62fab-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="62fab-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62fab-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="62fab-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="62fab-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="62fab-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62fab-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="62fab-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62fab-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="62fab-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="62fab-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="62fab-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="62fab-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="62fab-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="62fab-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="62fab-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="62fab-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="62fab-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62fab-164">createdDateTime</span></span>|<span data-ttu-id="62fab-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62fab-165">DateTimeOffset</span></span>|<span data-ttu-id="62fab-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="62fab-166">DateTime the object was created.</span></span> <span data-ttu-id="62fab-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-168">descrição</span><span class="sxs-lookup"><span data-stu-id="62fab-168">description</span></span>|<span data-ttu-id="62fab-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62fab-169">String</span></span>|<span data-ttu-id="62fab-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62fab-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62fab-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-172">displayName</span><span class="sxs-lookup"><span data-stu-id="62fab-172">displayName</span></span>|<span data-ttu-id="62fab-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62fab-173">String</span></span>|<span data-ttu-id="62fab-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62fab-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62fab-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-176">versão</span><span class="sxs-lookup"><span data-stu-id="62fab-176">version</span></span>|<span data-ttu-id="62fab-177">Int32</span><span class="sxs-lookup"><span data-stu-id="62fab-177">Int32</span></span>|<span data-ttu-id="62fab-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62fab-178">Version of the device configuration.</span></span> <span data-ttu-id="62fab-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62fab-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="62fab-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="62fab-181">Int32</span><span class="sxs-lookup"><span data-stu-id="62fab-181">Int32</span></span>|<span data-ttu-id="62fab-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="62fab-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="62fab-183">Herdado [do macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62fab-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62fab-184">subjectNameFormat</span></span>|[<span data-ttu-id="62fab-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62fab-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="62fab-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="62fab-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="62fab-187">Herdado [de macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62fab-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="62fab-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="62fab-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="62fab-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="62fab-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="62fab-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="62fab-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="62fab-191">Tipo de nome alternativo do assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="62fab-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="62fab-192">Herdado [de macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62fab-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="62fab-193">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="62fab-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="62fab-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="62fab-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="62fab-195">Int32</span><span class="sxs-lookup"><span data-stu-id="62fab-195">Int32</span></span>|<span data-ttu-id="62fab-196">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="62fab-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="62fab-197">Herdado [do macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62fab-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62fab-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="62fab-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="62fab-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="62fab-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="62fab-200">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="62fab-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="62fab-201">Herdado [de macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62fab-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="62fab-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="62fab-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="62fab-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="62fab-203">intendedPurpose</span></span>|[<span data-ttu-id="62fab-204">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="62fab-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="62fab-205">Finalidade pretendido do Perfil de Certificado - que pode ser Unassigned, SmimeEncryption, SmimeSigning etc. Os valores possíveis são: `unassigned` , , , , `smimeEncryption` `smimeSigning` `vpn` `wifi` .</span><span class="sxs-lookup"><span data-stu-id="62fab-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="62fab-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="62fab-206">Response</span></span>
<span data-ttu-id="62fab-207">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62fab-207">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62fab-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62fab-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="62fab-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62fab-209">Request</span></span>
<span data-ttu-id="62fab-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62fab-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62fab-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="62fab-211">Response</span></span>
<span data-ttu-id="62fab-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62fab-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




