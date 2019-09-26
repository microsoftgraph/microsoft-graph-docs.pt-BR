---
title: Atualizar iosScepCertificateProfile
description: Atualiza as propriedades de um objeto iosScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 992807556ee2b34adbfd1f8c9c1e089febbba308
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179296"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="49aaa-103">Atualizar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="49aaa-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="49aaa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49aaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49aaa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49aaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49aaa-106">Atualiza as propriedades de um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="49aaa-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49aaa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49aaa-107">Prerequisites</span></span>
<span data-ttu-id="49aaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49aaa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49aaa-110">Permission type</span></span>|<span data-ttu-id="49aaa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49aaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49aaa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49aaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49aaa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49aaa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49aaa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49aaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49aaa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49aaa-115">Not supported.</span></span>|
|<span data-ttu-id="49aaa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49aaa-116">Application</span></span>|<span data-ttu-id="49aaa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49aaa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49aaa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49aaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="49aaa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49aaa-119">Request headers</span></span>
|<span data-ttu-id="49aaa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49aaa-120">Header</span></span>|<span data-ttu-id="49aaa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49aaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49aaa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49aaa-122">Authorization</span></span>|<span data-ttu-id="49aaa-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49aaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49aaa-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49aaa-124">Accept</span></span>|<span data-ttu-id="49aaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49aaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49aaa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49aaa-126">Request body</span></span>
<span data-ttu-id="49aaa-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="49aaa-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="49aaa-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="49aaa-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="49aaa-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49aaa-129">Property</span></span>|<span data-ttu-id="49aaa-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49aaa-130">Type</span></span>|<span data-ttu-id="49aaa-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49aaa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49aaa-132">id</span><span class="sxs-lookup"><span data-stu-id="49aaa-132">id</span></span>|<span data-ttu-id="49aaa-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49aaa-133">String</span></span>|<span data-ttu-id="49aaa-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="49aaa-134">Key of the entity.</span></span> <span data-ttu-id="49aaa-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49aaa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="49aaa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49aaa-137">DateTimeOffset</span></span>|<span data-ttu-id="49aaa-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="49aaa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="49aaa-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49aaa-140">roleScopeTagIds</span></span>|<span data-ttu-id="49aaa-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49aaa-141">String collection</span></span>|<span data-ttu-id="49aaa-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="49aaa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49aaa-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="49aaa-144">supportsScopeTags</span></span>|<span data-ttu-id="49aaa-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="49aaa-145">Boolean</span></span>|<span data-ttu-id="49aaa-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="49aaa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49aaa-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="49aaa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49aaa-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="49aaa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49aaa-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49aaa-149">This property is read-only.</span></span> <span data-ttu-id="49aaa-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="49aaa-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="49aaa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="49aaa-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="49aaa-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="49aaa-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="49aaa-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="49aaa-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="49aaa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="49aaa-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="49aaa-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="49aaa-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="49aaa-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="49aaa-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="49aaa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="49aaa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="49aaa-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="49aaa-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="49aaa-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49aaa-163">createdDateTime</span></span>|<span data-ttu-id="49aaa-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49aaa-164">DateTimeOffset</span></span>|<span data-ttu-id="49aaa-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="49aaa-165">DateTime the object was created.</span></span> <span data-ttu-id="49aaa-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-167">descrição</span><span class="sxs-lookup"><span data-stu-id="49aaa-167">description</span></span>|<span data-ttu-id="49aaa-168">String</span><span class="sxs-lookup"><span data-stu-id="49aaa-168">String</span></span>|<span data-ttu-id="49aaa-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49aaa-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49aaa-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-171">displayName</span><span class="sxs-lookup"><span data-stu-id="49aaa-171">displayName</span></span>|<span data-ttu-id="49aaa-172">String</span><span class="sxs-lookup"><span data-stu-id="49aaa-172">String</span></span>|<span data-ttu-id="49aaa-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49aaa-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49aaa-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-175">versão</span><span class="sxs-lookup"><span data-stu-id="49aaa-175">version</span></span>|<span data-ttu-id="49aaa-176">Int32</span><span class="sxs-lookup"><span data-stu-id="49aaa-176">Int32</span></span>|<span data-ttu-id="49aaa-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49aaa-177">Version of the device configuration.</span></span> <span data-ttu-id="49aaa-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49aaa-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="49aaa-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="49aaa-180">Int32</span><span class="sxs-lookup"><span data-stu-id="49aaa-180">Int32</span></span>|<span data-ttu-id="49aaa-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="49aaa-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="49aaa-182">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="49aaa-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="49aaa-183">subjectNameFormat</span></span>|[<span data-ttu-id="49aaa-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="49aaa-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="49aaa-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="49aaa-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="49aaa-186">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="49aaa-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="49aaa-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="49aaa-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="49aaa-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="49aaa-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="49aaa-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="49aaa-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="49aaa-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="49aaa-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="49aaa-191">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="49aaa-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="49aaa-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="49aaa-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="49aaa-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="49aaa-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="49aaa-194">Int32</span><span class="sxs-lookup"><span data-stu-id="49aaa-194">Int32</span></span>|<span data-ttu-id="49aaa-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="49aaa-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="49aaa-196">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="49aaa-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="49aaa-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="49aaa-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="49aaa-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="49aaa-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="49aaa-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="49aaa-200">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="49aaa-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="49aaa-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="49aaa-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="49aaa-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="49aaa-202">scepServerUrls</span></span>|<span data-ttu-id="49aaa-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49aaa-203">String collection</span></span>|<span data-ttu-id="49aaa-204">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="49aaa-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="49aaa-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="49aaa-205">subjectNameFormatString</span></span>|<span data-ttu-id="49aaa-206">String</span><span class="sxs-lookup"><span data-stu-id="49aaa-206">String</span></span>|<span data-ttu-id="49aaa-207">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="49aaa-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="49aaa-208">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="49aaa-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="49aaa-209">uso de</span><span class="sxs-lookup"><span data-stu-id="49aaa-209">keyUsage</span></span>|[<span data-ttu-id="49aaa-210">usos de</span><span class="sxs-lookup"><span data-stu-id="49aaa-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="49aaa-211">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="49aaa-211">SCEP Key Usage.</span></span> <span data-ttu-id="49aaa-212">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="49aaa-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="49aaa-213">keySize</span><span class="sxs-lookup"><span data-stu-id="49aaa-213">keySize</span></span>|[<span data-ttu-id="49aaa-214">keySize</span><span class="sxs-lookup"><span data-stu-id="49aaa-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="49aaa-215">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="49aaa-215">SCEP Key Size.</span></span> <span data-ttu-id="49aaa-216">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="49aaa-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="49aaa-217">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="49aaa-217">extendedKeyUsages</span></span>|<span data-ttu-id="49aaa-218">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="49aaa-219">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="49aaa-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="49aaa-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="49aaa-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="49aaa-221">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="49aaa-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="49aaa-222">String</span><span class="sxs-lookup"><span data-stu-id="49aaa-222">String</span></span>|<span data-ttu-id="49aaa-223">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="49aaa-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="49aaa-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="49aaa-224">certificateStore</span></span>|[<span data-ttu-id="49aaa-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="49aaa-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="49aaa-226">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="49aaa-226">Target store certificate.</span></span> <span data-ttu-id="49aaa-227">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="49aaa-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="49aaa-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="49aaa-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="49aaa-229">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="49aaa-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="49aaa-230">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="49aaa-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="49aaa-231">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="49aaa-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="49aaa-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="49aaa-232">Response</span></span>
<span data-ttu-id="49aaa-233">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49aaa-233">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49aaa-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49aaa-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="49aaa-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49aaa-235">Request</span></span>
<span data-ttu-id="49aaa-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49aaa-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="49aaa-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="49aaa-237">Response</span></span>
<span data-ttu-id="49aaa-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49aaa-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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




