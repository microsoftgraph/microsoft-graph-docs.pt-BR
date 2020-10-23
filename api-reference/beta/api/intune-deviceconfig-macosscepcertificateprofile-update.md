---
title: Atualizar macOSScepCertificateProfile
description: Atualiza as propriedades de um objeto macOSScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 291e60716cde30cf653aa27a7eaa5eb3aa447bb8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723599"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="e0010-103">Atualizar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e0010-103">Update macOSScepCertificateProfile</span></span>

<span data-ttu-id="e0010-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0010-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0010-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0010-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0010-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0010-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0010-107">Atualiza as propriedades de um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e0010-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0010-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0010-108">Prerequisites</span></span>
<span data-ttu-id="e0010-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0010-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0010-111">Permission type</span></span>|<span data-ttu-id="e0010-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0010-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0010-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0010-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0010-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0010-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0010-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0010-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0010-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0010-116">Not supported.</span></span>|
|<span data-ttu-id="e0010-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0010-117">Application</span></span>|<span data-ttu-id="e0010-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0010-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0010-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0010-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0010-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0010-120">Request headers</span></span>
|<span data-ttu-id="e0010-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0010-121">Header</span></span>|<span data-ttu-id="e0010-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e0010-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0010-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0010-123">Authorization</span></span>|<span data-ttu-id="e0010-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0010-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0010-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0010-125">Accept</span></span>|<span data-ttu-id="e0010-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0010-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0010-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0010-127">Request body</span></span>
<span data-ttu-id="e0010-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e0010-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="e0010-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e0010-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="e0010-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0010-130">Property</span></span>|<span data-ttu-id="e0010-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0010-131">Type</span></span>|<span data-ttu-id="e0010-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0010-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0010-133">id</span><span class="sxs-lookup"><span data-stu-id="e0010-133">id</span></span>|<span data-ttu-id="e0010-134">String</span><span class="sxs-lookup"><span data-stu-id="e0010-134">String</span></span>|<span data-ttu-id="e0010-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0010-135">Key of the entity.</span></span> <span data-ttu-id="e0010-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0010-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e0010-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0010-138">DateTimeOffset</span></span>|<span data-ttu-id="e0010-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e0010-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e0010-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0010-141">roleScopeTagIds</span></span>|<span data-ttu-id="e0010-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0010-142">String collection</span></span>|<span data-ttu-id="e0010-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e0010-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0010-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e0010-145">supportsScopeTags</span></span>|<span data-ttu-id="e0010-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0010-146">Boolean</span></span>|<span data-ttu-id="e0010-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e0010-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0010-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e0010-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0010-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0010-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0010-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0010-150">This property is read-only.</span></span> <span data-ttu-id="e0010-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0010-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e0010-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0010-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e0010-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="e0010-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e0010-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0010-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e0010-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0010-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e0010-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="e0010-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e0010-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0010-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e0010-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0010-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e0010-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="e0010-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e0010-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0010-164">createdDateTime</span></span>|<span data-ttu-id="e0010-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0010-165">DateTimeOffset</span></span>|<span data-ttu-id="e0010-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e0010-166">DateTime the object was created.</span></span> <span data-ttu-id="e0010-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-168">description</span><span class="sxs-lookup"><span data-stu-id="e0010-168">description</span></span>|<span data-ttu-id="e0010-169">String</span><span class="sxs-lookup"><span data-stu-id="e0010-169">String</span></span>|<span data-ttu-id="e0010-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0010-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0010-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e0010-172">displayName</span></span>|<span data-ttu-id="e0010-173">String</span><span class="sxs-lookup"><span data-stu-id="e0010-173">String</span></span>|<span data-ttu-id="e0010-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0010-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0010-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-176">versão</span><span class="sxs-lookup"><span data-stu-id="e0010-176">version</span></span>|<span data-ttu-id="e0010-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e0010-177">Int32</span></span>|<span data-ttu-id="e0010-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0010-178">Version of the device configuration.</span></span> <span data-ttu-id="e0010-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0010-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="e0010-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="e0010-181">Int32</span><span class="sxs-lookup"><span data-stu-id="e0010-181">Int32</span></span>|<span data-ttu-id="e0010-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="e0010-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e0010-183">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e0010-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0010-184">subjectNameFormat</span></span>|[<span data-ttu-id="e0010-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0010-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="e0010-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e0010-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="e0010-187">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e0010-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="e0010-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="e0010-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="e0010-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e0010-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e0010-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e0010-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e0010-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e0010-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="e0010-192">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e0010-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="e0010-193">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="e0010-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="e0010-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e0010-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e0010-195">Int32</span><span class="sxs-lookup"><span data-stu-id="e0010-195">Int32</span></span>|<span data-ttu-id="e0010-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e0010-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="e0010-197">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e0010-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e0010-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e0010-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e0010-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e0010-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e0010-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e0010-201">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e0010-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="e0010-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e0010-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e0010-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="e0010-203">scepServerUrls</span></span>|<span data-ttu-id="e0010-204">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0010-204">String collection</span></span>|<span data-ttu-id="e0010-205">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="e0010-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="e0010-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e0010-206">subjectNameFormatString</span></span>|<span data-ttu-id="e0010-207">String</span><span class="sxs-lookup"><span data-stu-id="e0010-207">String</span></span>|<span data-ttu-id="e0010-208">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="e0010-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="e0010-209">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="e0010-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="e0010-210">uso de</span><span class="sxs-lookup"><span data-stu-id="e0010-210">keyUsage</span></span>|[<span data-ttu-id="e0010-211">usos de</span><span class="sxs-lookup"><span data-stu-id="e0010-211">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e0010-212">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="e0010-212">SCEP Key Usage.</span></span> <span data-ttu-id="e0010-213">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="e0010-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e0010-214">keySize</span><span class="sxs-lookup"><span data-stu-id="e0010-214">keySize</span></span>|[<span data-ttu-id="e0010-215">keySize</span><span class="sxs-lookup"><span data-stu-id="e0010-215">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="e0010-216">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="e0010-216">SCEP Key Size.</span></span> <span data-ttu-id="e0010-217">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="e0010-217">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="e0010-218">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e0010-218">hashAlgorithm</span></span>|[<span data-ttu-id="e0010-219">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e0010-219">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="e0010-220">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="e0010-220">SCEP Hash Algorithm.</span></span> <span data-ttu-id="e0010-221">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="e0010-221">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="e0010-222">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="e0010-222">extendedKeyUsages</span></span>|<span data-ttu-id="e0010-223">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-223">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e0010-224">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="e0010-224">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e0010-225">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e0010-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e0010-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="e0010-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e0010-227">String</span><span class="sxs-lookup"><span data-stu-id="e0010-227">String</span></span>|<span data-ttu-id="e0010-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="e0010-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="e0010-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="e0010-229">certificateStore</span></span>|[<span data-ttu-id="e0010-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="e0010-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="e0010-231">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="e0010-231">Target store certificate.</span></span> <span data-ttu-id="e0010-232">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="e0010-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="e0010-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="e0010-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="e0010-234">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="e0010-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="e0010-235">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="e0010-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="e0010-236">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e0010-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e0010-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0010-237">Response</span></span>
<span data-ttu-id="e0010-238">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0010-238">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0010-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0010-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0010-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0010-240">Request</span></span>
<span data-ttu-id="e0010-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0010-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1962

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e0010-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0010-242">Response</span></span>
<span data-ttu-id="e0010-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0010-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2134

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```





