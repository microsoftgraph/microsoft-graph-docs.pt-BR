---
title: Atualizar macOSScepCertificateProfile
description: Atualiza as propriedades de um objeto macOSScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29b34723f32476dcc8d52a02998f242ea8539da4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160932"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="8f155-103">Atualizar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8f155-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="8f155-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f155-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f155-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f155-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f155-106">Atualiza as propriedades de um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8f155-106">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f155-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f155-107">Prerequisites</span></span>
<span data-ttu-id="8f155-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f155-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f155-110">Permission type</span></span>|<span data-ttu-id="8f155-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f155-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f155-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f155-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f155-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f155-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f155-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f155-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f155-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f155-115">Not supported.</span></span>|
|<span data-ttu-id="8f155-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f155-116">Application</span></span>|<span data-ttu-id="8f155-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f155-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f155-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f155-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8f155-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f155-119">Request headers</span></span>
|<span data-ttu-id="8f155-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f155-120">Header</span></span>|<span data-ttu-id="8f155-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8f155-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f155-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f155-122">Authorization</span></span>|<span data-ttu-id="8f155-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f155-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f155-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f155-124">Accept</span></span>|<span data-ttu-id="8f155-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f155-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f155-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f155-126">Request body</span></span>
<span data-ttu-id="8f155-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8f155-127">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="8f155-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8f155-128">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="8f155-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f155-129">Property</span></span>|<span data-ttu-id="8f155-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f155-130">Type</span></span>|<span data-ttu-id="8f155-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f155-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f155-132">id</span><span class="sxs-lookup"><span data-stu-id="8f155-132">id</span></span>|<span data-ttu-id="8f155-133">String</span><span class="sxs-lookup"><span data-stu-id="8f155-133">String</span></span>|<span data-ttu-id="8f155-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8f155-134">Key of the entity.</span></span> <span data-ttu-id="8f155-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f155-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8f155-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f155-137">DateTimeOffset</span></span>|<span data-ttu-id="8f155-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8f155-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8f155-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f155-140">roleScopeTagIds</span></span>|<span data-ttu-id="8f155-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f155-141">String collection</span></span>|<span data-ttu-id="8f155-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8f155-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8f155-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8f155-144">supportsScopeTags</span></span>|<span data-ttu-id="8f155-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f155-145">Boolean</span></span>|<span data-ttu-id="8f155-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8f155-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8f155-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8f155-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8f155-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8f155-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8f155-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f155-149">This property is read-only.</span></span> <span data-ttu-id="8f155-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f155-151">createdDateTime</span></span>|<span data-ttu-id="8f155-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f155-152">DateTimeOffset</span></span>|<span data-ttu-id="8f155-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8f155-153">DateTime the object was created.</span></span> <span data-ttu-id="8f155-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-155">description</span><span class="sxs-lookup"><span data-stu-id="8f155-155">description</span></span>|<span data-ttu-id="8f155-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f155-156">String</span></span>|<span data-ttu-id="8f155-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f155-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f155-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8f155-159">displayName</span></span>|<span data-ttu-id="8f155-160">String</span><span class="sxs-lookup"><span data-stu-id="8f155-160">String</span></span>|<span data-ttu-id="8f155-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f155-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f155-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-163">version</span><span class="sxs-lookup"><span data-stu-id="8f155-163">version</span></span>|<span data-ttu-id="8f155-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8f155-164">Int32</span></span>|<span data-ttu-id="8f155-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f155-165">Version of the device configuration.</span></span> <span data-ttu-id="8f155-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f155-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8f155-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="8f155-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8f155-168">Int32</span></span>|<span data-ttu-id="8f155-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="8f155-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8f155-170">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8f155-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8f155-171">subjectNameFormat</span></span>|[<span data-ttu-id="8f155-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8f155-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="8f155-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f155-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="8f155-174">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f155-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="8f155-175">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="8f155-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="8f155-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8f155-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8f155-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8f155-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8f155-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f155-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="8f155-179">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f155-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="8f155-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8f155-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8f155-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8f155-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8f155-182">Int32</span><span class="sxs-lookup"><span data-stu-id="8f155-182">Int32</span></span>|<span data-ttu-id="8f155-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f155-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8f155-184">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8f155-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8f155-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8f155-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8f155-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8f155-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f155-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8f155-188">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f155-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="8f155-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8f155-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8f155-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="8f155-190">scepServerUrls</span></span>|<span data-ttu-id="8f155-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f155-191">String collection</span></span>|<span data-ttu-id="8f155-192">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f155-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="8f155-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8f155-193">subjectNameFormatString</span></span>|<span data-ttu-id="8f155-194">String</span><span class="sxs-lookup"><span data-stu-id="8f155-194">String</span></span>|<span data-ttu-id="8f155-195">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="8f155-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="8f155-196">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="8f155-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8f155-197">uso de</span><span class="sxs-lookup"><span data-stu-id="8f155-197">keyUsage</span></span>|[<span data-ttu-id="8f155-198">usos de</span><span class="sxs-lookup"><span data-stu-id="8f155-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="8f155-199">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f155-199">SCEP Key Usage.</span></span> <span data-ttu-id="8f155-200">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="8f155-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="8f155-201">keySize</span><span class="sxs-lookup"><span data-stu-id="8f155-201">keySize</span></span>|[<span data-ttu-id="8f155-202">keySize</span><span class="sxs-lookup"><span data-stu-id="8f155-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="8f155-203">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f155-203">SCEP Key Size.</span></span> <span data-ttu-id="8f155-204">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="8f155-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="8f155-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8f155-205">hashAlgorithm</span></span>|[<span data-ttu-id="8f155-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8f155-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="8f155-207">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f155-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="8f155-208">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="8f155-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="8f155-209">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="8f155-209">extendedKeyUsages</span></span>|<span data-ttu-id="8f155-210">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8f155-211">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="8f155-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8f155-212">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f155-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8f155-213">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="8f155-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8f155-214">String</span><span class="sxs-lookup"><span data-stu-id="8f155-214">String</span></span>|<span data-ttu-id="8f155-215">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="8f155-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="8f155-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8f155-216">certificateStore</span></span>|[<span data-ttu-id="8f155-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8f155-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="8f155-218">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="8f155-218">Target store certificate.</span></span> <span data-ttu-id="8f155-219">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="8f155-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="8f155-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="8f155-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="8f155-221">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="8f155-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="8f155-222">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="8f155-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="8f155-223">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f155-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8f155-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f155-224">Response</span></span>
<span data-ttu-id="8f155-225">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f155-225">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f155-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f155-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f155-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f155-227">Request</span></span>
<span data-ttu-id="8f155-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f155-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="8f155-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f155-229">Response</span></span>
<span data-ttu-id="8f155-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f155-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




