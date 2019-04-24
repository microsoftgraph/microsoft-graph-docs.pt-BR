---
title: Atualizar macOSScepCertificateProfile
description: Atualiza as propriedades de um objeto macOSScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2da7148fb9cdba31dd055a2edd66d00542f4586a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518419"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="f7282-103">Atualizar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f7282-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="f7282-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7282-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7282-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7282-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7282-106">Atualiza as propriedades de um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f7282-106">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7282-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7282-107">Prerequisites</span></span>
<span data-ttu-id="f7282-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7282-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7282-110">Permission type</span></span>|<span data-ttu-id="f7282-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7282-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7282-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7282-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7282-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7282-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7282-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7282-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7282-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7282-115">Not supported.</span></span>|
|<span data-ttu-id="f7282-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7282-116">Application</span></span>|<span data-ttu-id="f7282-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7282-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7282-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7282-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7282-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7282-119">Request headers</span></span>
|<span data-ttu-id="f7282-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7282-120">Header</span></span>|<span data-ttu-id="f7282-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f7282-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7282-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7282-122">Authorization</span></span>|<span data-ttu-id="f7282-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7282-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7282-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7282-124">Accept</span></span>|<span data-ttu-id="f7282-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7282-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7282-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7282-126">Request body</span></span>
<span data-ttu-id="f7282-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f7282-127">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f7282-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f7282-128">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="f7282-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7282-129">Property</span></span>|<span data-ttu-id="f7282-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7282-130">Type</span></span>|<span data-ttu-id="f7282-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7282-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7282-132">id</span><span class="sxs-lookup"><span data-stu-id="f7282-132">id</span></span>|<span data-ttu-id="f7282-133">String</span><span class="sxs-lookup"><span data-stu-id="f7282-133">String</span></span>|<span data-ttu-id="f7282-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7282-134">Key of the entity.</span></span> <span data-ttu-id="f7282-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7282-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f7282-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7282-137">DateTimeOffset</span></span>|<span data-ttu-id="f7282-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f7282-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f7282-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7282-140">roleScopeTagIds</span></span>|<span data-ttu-id="f7282-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7282-141">String collection</span></span>|<span data-ttu-id="f7282-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f7282-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f7282-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f7282-144">supportsScopeTags</span></span>|<span data-ttu-id="f7282-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7282-145">Boolean</span></span>|<span data-ttu-id="f7282-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f7282-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f7282-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f7282-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f7282-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f7282-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f7282-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7282-149">This property is read-only.</span></span> <span data-ttu-id="f7282-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7282-151">createdDateTime</span></span>|<span data-ttu-id="f7282-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7282-152">DateTimeOffset</span></span>|<span data-ttu-id="f7282-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f7282-153">DateTime the object was created.</span></span> <span data-ttu-id="f7282-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-155">description</span><span class="sxs-lookup"><span data-stu-id="f7282-155">description</span></span>|<span data-ttu-id="f7282-156">String</span><span class="sxs-lookup"><span data-stu-id="f7282-156">String</span></span>|<span data-ttu-id="f7282-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7282-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f7282-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f7282-159">displayName</span></span>|<span data-ttu-id="f7282-160">String</span><span class="sxs-lookup"><span data-stu-id="f7282-160">String</span></span>|<span data-ttu-id="f7282-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7282-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f7282-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-163">versão</span><span class="sxs-lookup"><span data-stu-id="f7282-163">version</span></span>|<span data-ttu-id="f7282-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f7282-164">Int32</span></span>|<span data-ttu-id="f7282-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7282-165">Version of the device configuration.</span></span> <span data-ttu-id="f7282-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7282-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f7282-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="f7282-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f7282-168">Int32</span></span>|<span data-ttu-id="f7282-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="f7282-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f7282-170">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f7282-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f7282-171">subjectNameFormat</span></span>|[<span data-ttu-id="f7282-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f7282-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f7282-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f7282-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="f7282-174">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7282-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f7282-175">Os valores possíveis são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f7282-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f7282-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f7282-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f7282-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f7282-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f7282-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f7282-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f7282-179">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7282-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f7282-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f7282-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f7282-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f7282-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f7282-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f7282-182">Int32</span></span>|<span data-ttu-id="f7282-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f7282-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f7282-184">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f7282-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f7282-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f7282-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f7282-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f7282-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f7282-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f7282-188">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7282-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f7282-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f7282-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f7282-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f7282-190">scepServerUrls</span></span>|<span data-ttu-id="f7282-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7282-191">String collection</span></span>|<span data-ttu-id="f7282-192">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="f7282-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f7282-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f7282-193">subjectNameFormatString</span></span>|<span data-ttu-id="f7282-194">String</span><span class="sxs-lookup"><span data-stu-id="f7282-194">String</span></span>|<span data-ttu-id="f7282-195">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="f7282-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f7282-196">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="f7282-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f7282-197">uso de</span><span class="sxs-lookup"><span data-stu-id="f7282-197">keyUsage</span></span>|[<span data-ttu-id="f7282-198">usos de</span><span class="sxs-lookup"><span data-stu-id="f7282-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f7282-199">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f7282-199">SCEP Key Usage.</span></span> <span data-ttu-id="f7282-200">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f7282-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f7282-201">keySize</span><span class="sxs-lookup"><span data-stu-id="f7282-201">keySize</span></span>|[<span data-ttu-id="f7282-202">keySize</span><span class="sxs-lookup"><span data-stu-id="f7282-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f7282-203">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="f7282-203">SCEP Key Size.</span></span> <span data-ttu-id="f7282-204">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="f7282-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f7282-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f7282-205">hashAlgorithm</span></span>|[<span data-ttu-id="f7282-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f7282-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f7282-207">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f7282-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f7282-208">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f7282-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f7282-209">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f7282-209">extendedKeyUsages</span></span>|<span data-ttu-id="f7282-210">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f7282-211">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="f7282-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f7282-212">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f7282-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f7282-213">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="f7282-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f7282-214">String</span><span class="sxs-lookup"><span data-stu-id="f7282-214">String</span></span>|<span data-ttu-id="f7282-215">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="f7282-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f7282-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f7282-216">certificateStore</span></span>|[<span data-ttu-id="f7282-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f7282-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f7282-218">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="f7282-218">Target store certificate.</span></span> <span data-ttu-id="f7282-219">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="f7282-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f7282-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f7282-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f7282-221">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f7282-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f7282-222">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="f7282-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f7282-223">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f7282-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f7282-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7282-224">Response</span></span>
<span data-ttu-id="f7282-225">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7282-225">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7282-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7282-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7282-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7282-227">Request</span></span>
<span data-ttu-id="f7282-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7282-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7282-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7282-229">Response</span></span>
<span data-ttu-id="f7282-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7282-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





