---
title: Atualizar macOSScepCertificateProfile
description: Atualiza as propriedades de um objeto macOSScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db025f950f6ecc6e9a0776654ae4ef15f94e4a2a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948139"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="16d7a-103">Atualizar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="16d7a-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="16d7a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16d7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16d7a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16d7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16d7a-106">Atualiza as propriedades de um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16d7a-106">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16d7a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16d7a-107">Prerequisites</span></span>
<span data-ttu-id="16d7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16d7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16d7a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16d7a-110">Permission type</span></span>|<span data-ttu-id="16d7a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16d7a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16d7a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16d7a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16d7a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16d7a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16d7a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16d7a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16d7a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16d7a-115">Not supported.</span></span>|
|<span data-ttu-id="16d7a-116">Application</span><span class="sxs-lookup"><span data-stu-id="16d7a-116">Application</span></span>|<span data-ttu-id="16d7a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16d7a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16d7a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16d7a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="16d7a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16d7a-119">Request headers</span></span>
|<span data-ttu-id="16d7a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16d7a-120">Header</span></span>|<span data-ttu-id="16d7a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16d7a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16d7a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16d7a-122">Authorization</span></span>|<span data-ttu-id="16d7a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16d7a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16d7a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16d7a-124">Accept</span></span>|<span data-ttu-id="16d7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16d7a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16d7a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16d7a-126">Request body</span></span>
<span data-ttu-id="16d7a-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16d7a-127">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="16d7a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="16d7a-128">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="16d7a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16d7a-129">Property</span></span>|<span data-ttu-id="16d7a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16d7a-130">Type</span></span>|<span data-ttu-id="16d7a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16d7a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d7a-132">id</span><span class="sxs-lookup"><span data-stu-id="16d7a-132">id</span></span>|<span data-ttu-id="16d7a-133">String</span><span class="sxs-lookup"><span data-stu-id="16d7a-133">String</span></span>|<span data-ttu-id="16d7a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16d7a-134">Key of the entity.</span></span> <span data-ttu-id="16d7a-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16d7a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="16d7a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16d7a-137">DateTimeOffset</span></span>|<span data-ttu-id="16d7a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="16d7a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="16d7a-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16d7a-140">roleScopeTagIds</span></span>|<span data-ttu-id="16d7a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="16d7a-141">String collection</span></span>|<span data-ttu-id="16d7a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="16d7a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16d7a-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="16d7a-144">supportsScopeTags</span></span>|<span data-ttu-id="16d7a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="16d7a-145">Boolean</span></span>|<span data-ttu-id="16d7a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="16d7a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16d7a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="16d7a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16d7a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d7a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16d7a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16d7a-149">This property is read-only.</span></span> <span data-ttu-id="16d7a-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="16d7a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="16d7a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="16d7a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="16d7a-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="16d7a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="16d7a-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="16d7a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="16d7a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="16d7a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="16d7a-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="16d7a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="16d7a-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="16d7a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="16d7a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="16d7a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="16d7a-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="16d7a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="16d7a-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16d7a-163">createdDateTime</span></span>|<span data-ttu-id="16d7a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16d7a-164">DateTimeOffset</span></span>|<span data-ttu-id="16d7a-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="16d7a-165">DateTime the object was created.</span></span> <span data-ttu-id="16d7a-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-167">description</span><span class="sxs-lookup"><span data-stu-id="16d7a-167">description</span></span>|<span data-ttu-id="16d7a-168">String</span><span class="sxs-lookup"><span data-stu-id="16d7a-168">String</span></span>|<span data-ttu-id="16d7a-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16d7a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16d7a-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="16d7a-171">displayName</span></span>|<span data-ttu-id="16d7a-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16d7a-172">String</span></span>|<span data-ttu-id="16d7a-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16d7a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16d7a-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-175">versão</span><span class="sxs-lookup"><span data-stu-id="16d7a-175">version</span></span>|<span data-ttu-id="16d7a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="16d7a-176">Int32</span></span>|<span data-ttu-id="16d7a-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16d7a-177">Version of the device configuration.</span></span> <span data-ttu-id="16d7a-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16d7a-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="16d7a-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="16d7a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="16d7a-180">Int32</span></span>|<span data-ttu-id="16d7a-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="16d7a-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="16d7a-182">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="16d7a-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="16d7a-183">subjectNameFormat</span></span>|[<span data-ttu-id="16d7a-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="16d7a-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="16d7a-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16d7a-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="16d7a-186">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="16d7a-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="16d7a-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="16d7a-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="16d7a-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="16d7a-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="16d7a-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="16d7a-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16d7a-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="16d7a-191">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="16d7a-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="16d7a-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="16d7a-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="16d7a-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="16d7a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="16d7a-194">Int32</span></span>|<span data-ttu-id="16d7a-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16d7a-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="16d7a-196">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="16d7a-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="16d7a-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="16d7a-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="16d7a-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="16d7a-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16d7a-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="16d7a-200">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="16d7a-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="16d7a-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="16d7a-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="16d7a-202">scepServerUrls</span></span>|<span data-ttu-id="16d7a-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="16d7a-203">String collection</span></span>|<span data-ttu-id="16d7a-204">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="16d7a-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="16d7a-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="16d7a-205">subjectNameFormatString</span></span>|<span data-ttu-id="16d7a-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="16d7a-206">String</span></span>|<span data-ttu-id="16d7a-207">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="16d7a-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="16d7a-208">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="16d7a-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="16d7a-209">uso de</span><span class="sxs-lookup"><span data-stu-id="16d7a-209">keyUsage</span></span>|[<span data-ttu-id="16d7a-210">usos de</span><span class="sxs-lookup"><span data-stu-id="16d7a-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="16d7a-211">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="16d7a-211">SCEP Key Usage.</span></span> <span data-ttu-id="16d7a-212">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="16d7a-213">keySize</span><span class="sxs-lookup"><span data-stu-id="16d7a-213">keySize</span></span>|[<span data-ttu-id="16d7a-214">keySize</span><span class="sxs-lookup"><span data-stu-id="16d7a-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="16d7a-215">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="16d7a-215">SCEP Key Size.</span></span> <span data-ttu-id="16d7a-216">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="16d7a-217">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="16d7a-217">hashAlgorithm</span></span>|[<span data-ttu-id="16d7a-218">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="16d7a-218">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="16d7a-219">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="16d7a-219">SCEP Hash Algorithm.</span></span> <span data-ttu-id="16d7a-220">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-220">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="16d7a-221">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="16d7a-221">extendedKeyUsages</span></span>|<span data-ttu-id="16d7a-222">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="16d7a-223">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="16d7a-223">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="16d7a-224">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="16d7a-224">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="16d7a-225">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="16d7a-225">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="16d7a-226">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="16d7a-226">String</span></span>|<span data-ttu-id="16d7a-227">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="16d7a-227">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="16d7a-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="16d7a-228">certificateStore</span></span>|[<span data-ttu-id="16d7a-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="16d7a-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="16d7a-230">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="16d7a-230">Target store certificate.</span></span> <span data-ttu-id="16d7a-231">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="16d7a-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="16d7a-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="16d7a-233">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="16d7a-234">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="16d7a-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="16d7a-235">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="16d7a-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="16d7a-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="16d7a-236">Response</span></span>
<span data-ttu-id="16d7a-237">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16d7a-237">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16d7a-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16d7a-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="16d7a-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16d7a-239">Request</span></span>
<span data-ttu-id="16d7a-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16d7a-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16d7a-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="16d7a-241">Response</span></span>
<span data-ttu-id="16d7a-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16d7a-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





