---
title: Criar iosScepCertificateProfile
description: Criar um novo objeto iosScepCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4590710906138eccd6e58d32eed38c231876de83
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42749645"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="a6e07-103">Criar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a6e07-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="a6e07-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6e07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6e07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6e07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6e07-106">Criar um novo objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a6e07-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6e07-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6e07-107">Prerequisites</span></span>
<span data-ttu-id="a6e07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e07-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6e07-110">Permission type</span></span>|<span data-ttu-id="a6e07-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6e07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6e07-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6e07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6e07-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e07-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6e07-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6e07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6e07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6e07-115">Not supported.</span></span>|
|<span data-ttu-id="a6e07-116">Application</span><span class="sxs-lookup"><span data-stu-id="a6e07-116">Application</span></span>|<span data-ttu-id="a6e07-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e07-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6e07-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6e07-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e07-119">Request headers</span></span>
|<span data-ttu-id="a6e07-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6e07-120">Header</span></span>|<span data-ttu-id="a6e07-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a6e07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6e07-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6e07-122">Authorization</span></span>|<span data-ttu-id="a6e07-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6e07-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6e07-124">Accept</span></span>|<span data-ttu-id="a6e07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6e07-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e07-126">Request body</span></span>
<span data-ttu-id="a6e07-127">No corpo da solicitação, forneça uma representação JSON do objeto iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a6e07-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="a6e07-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a6e07-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="a6e07-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6e07-129">Property</span></span>|<span data-ttu-id="a6e07-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6e07-130">Type</span></span>|<span data-ttu-id="a6e07-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6e07-132">id</span><span class="sxs-lookup"><span data-stu-id="a6e07-132">id</span></span>|<span data-ttu-id="a6e07-133">String</span><span class="sxs-lookup"><span data-stu-id="a6e07-133">String</span></span>|<span data-ttu-id="a6e07-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6e07-134">Key of the entity.</span></span> <span data-ttu-id="a6e07-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e07-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a6e07-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e07-137">DateTimeOffset</span></span>|<span data-ttu-id="a6e07-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a6e07-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a6e07-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6e07-140">roleScopeTagIds</span></span>|<span data-ttu-id="a6e07-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e07-141">String collection</span></span>|<span data-ttu-id="a6e07-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a6e07-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6e07-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6e07-144">supportsScopeTags</span></span>|<span data-ttu-id="a6e07-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6e07-145">Boolean</span></span>|<span data-ttu-id="a6e07-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a6e07-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6e07-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a6e07-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6e07-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a6e07-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6e07-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6e07-149">This property is read-only.</span></span> <span data-ttu-id="a6e07-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a6e07-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a6e07-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a6e07-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a6e07-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a6e07-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a6e07-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a6e07-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a6e07-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a6e07-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a6e07-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a6e07-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a6e07-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a6e07-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a6e07-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a6e07-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a6e07-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a6e07-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a6e07-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e07-163">createdDateTime</span></span>|<span data-ttu-id="a6e07-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e07-164">DateTimeOffset</span></span>|<span data-ttu-id="a6e07-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a6e07-165">DateTime the object was created.</span></span> <span data-ttu-id="a6e07-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-167">description</span><span class="sxs-lookup"><span data-stu-id="a6e07-167">description</span></span>|<span data-ttu-id="a6e07-168">String</span><span class="sxs-lookup"><span data-stu-id="a6e07-168">String</span></span>|<span data-ttu-id="a6e07-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a6e07-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6e07-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e07-171">displayName</span></span>|<span data-ttu-id="a6e07-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e07-172">String</span></span>|<span data-ttu-id="a6e07-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a6e07-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6e07-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-175">versão</span><span class="sxs-lookup"><span data-stu-id="a6e07-175">version</span></span>|<span data-ttu-id="a6e07-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a6e07-176">Int32</span></span>|<span data-ttu-id="a6e07-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a6e07-177">Version of the device configuration.</span></span> <span data-ttu-id="a6e07-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e07-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a6e07-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="a6e07-180">Int32</span><span class="sxs-lookup"><span data-stu-id="a6e07-180">Int32</span></span>|<span data-ttu-id="a6e07-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="a6e07-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a6e07-182">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a6e07-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a6e07-183">subjectNameFormat</span></span>|[<span data-ttu-id="a6e07-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a6e07-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="a6e07-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a6e07-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="a6e07-186">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a6e07-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="a6e07-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="a6e07-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="a6e07-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a6e07-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a6e07-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a6e07-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a6e07-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a6e07-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="a6e07-191">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a6e07-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="a6e07-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a6e07-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a6e07-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a6e07-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a6e07-194">Int32</span><span class="sxs-lookup"><span data-stu-id="a6e07-194">Int32</span></span>|<span data-ttu-id="a6e07-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a6e07-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a6e07-196">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a6e07-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a6e07-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a6e07-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a6e07-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a6e07-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a6e07-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a6e07-200">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a6e07-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="a6e07-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a6e07-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a6e07-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a6e07-202">scepServerUrls</span></span>|<span data-ttu-id="a6e07-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e07-203">String collection</span></span>|<span data-ttu-id="a6e07-204">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="a6e07-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="a6e07-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a6e07-205">subjectNameFormatString</span></span>|<span data-ttu-id="a6e07-206">String</span><span class="sxs-lookup"><span data-stu-id="a6e07-206">String</span></span>|<span data-ttu-id="a6e07-207">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a6e07-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a6e07-208">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="a6e07-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a6e07-209">uso de</span><span class="sxs-lookup"><span data-stu-id="a6e07-209">keyUsage</span></span>|[<span data-ttu-id="a6e07-210">usos de</span><span class="sxs-lookup"><span data-stu-id="a6e07-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a6e07-211">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="a6e07-211">SCEP Key Usage.</span></span> <span data-ttu-id="a6e07-212">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a6e07-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a6e07-213">keySize</span><span class="sxs-lookup"><span data-stu-id="a6e07-213">keySize</span></span>|[<span data-ttu-id="a6e07-214">keySize</span><span class="sxs-lookup"><span data-stu-id="a6e07-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a6e07-215">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="a6e07-215">SCEP Key Size.</span></span> <span data-ttu-id="a6e07-216">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="a6e07-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a6e07-217">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a6e07-217">extendedKeyUsages</span></span>|<span data-ttu-id="a6e07-218">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a6e07-219">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="a6e07-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a6e07-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a6e07-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a6e07-221">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="a6e07-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a6e07-222">String</span><span class="sxs-lookup"><span data-stu-id="a6e07-222">String</span></span>|<span data-ttu-id="a6e07-223">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="a6e07-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="a6e07-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="a6e07-224">certificateStore</span></span>|[<span data-ttu-id="a6e07-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="a6e07-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="a6e07-226">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="a6e07-226">Target store certificate.</span></span> <span data-ttu-id="a6e07-227">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="a6e07-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="a6e07-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="a6e07-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="a6e07-229">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="a6e07-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="a6e07-230">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="a6e07-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="a6e07-231">A variável Onpremisesuserprincipalname à é compatível, bem como outras documentadas aqui: s://go.microsoft.com/fwlink/?LinkId=2027630.</span><span class="sxs-lookup"><span data-stu-id="a6e07-231">The OnPremisesUserPrincipalName variable is support as well as others documented here: s://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="a6e07-232">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a6e07-232">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a6e07-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e07-233">Response</span></span>
<span data-ttu-id="a6e07-234">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6e07-234">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6e07-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6e07-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6e07-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e07-236">Request</span></span>
<span data-ttu-id="a6e07-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6e07-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a6e07-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e07-238">Response</span></span>
<span data-ttu-id="a6e07-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6e07-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




