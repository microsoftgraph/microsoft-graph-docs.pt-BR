---
title: Criar Entidadeandroidworkprofilescepcertificateprofile
description: Criar um novo objeto Entidadeandroidworkprofilescepcertificateprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ecd1806cd1797c6d5a79c34270c7b8db9a8893
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928320"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="59583-103">Criar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="59583-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="59583-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59583-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59583-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59583-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59583-106">Criar um novo objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="59583-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59583-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59583-107">Prerequisites</span></span>
<span data-ttu-id="59583-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59583-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59583-110">Permission type</span></span>|<span data-ttu-id="59583-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59583-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59583-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59583-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59583-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59583-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59583-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59583-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59583-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59583-115">Not supported.</span></span>|
|<span data-ttu-id="59583-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59583-116">Application</span></span>|<span data-ttu-id="59583-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59583-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59583-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59583-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="59583-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59583-119">Request headers</span></span>
|<span data-ttu-id="59583-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59583-120">Header</span></span>|<span data-ttu-id="59583-121">Valor</span><span class="sxs-lookup"><span data-stu-id="59583-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59583-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59583-122">Authorization</span></span>|<span data-ttu-id="59583-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59583-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59583-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59583-124">Accept</span></span>|<span data-ttu-id="59583-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59583-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59583-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59583-126">Request body</span></span>
<span data-ttu-id="59583-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidworkprofilescepcertificateprofile.</span><span class="sxs-lookup"><span data-stu-id="59583-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="59583-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidworkprofilescepcertificateprofile.</span><span class="sxs-lookup"><span data-stu-id="59583-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="59583-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59583-129">Property</span></span>|<span data-ttu-id="59583-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="59583-130">Type</span></span>|<span data-ttu-id="59583-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="59583-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59583-132">id</span><span class="sxs-lookup"><span data-stu-id="59583-132">id</span></span>|<span data-ttu-id="59583-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59583-133">String</span></span>|<span data-ttu-id="59583-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="59583-134">Key of the entity.</span></span> <span data-ttu-id="59583-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59583-136">lastModifiedDateTime</span></span>|<span data-ttu-id="59583-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59583-137">DateTimeOffset</span></span>|<span data-ttu-id="59583-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="59583-138">DateTime the object was last modified.</span></span> <span data-ttu-id="59583-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59583-140">roleScopeTagIds</span></span>|<span data-ttu-id="59583-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="59583-141">String collection</span></span>|<span data-ttu-id="59583-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="59583-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="59583-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="59583-144">supportsScopeTags</span></span>|<span data-ttu-id="59583-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="59583-145">Boolean</span></span>|<span data-ttu-id="59583-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="59583-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="59583-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="59583-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="59583-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="59583-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="59583-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59583-149">This property is read-only.</span></span> <span data-ttu-id="59583-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59583-151">createdDateTime</span></span>|<span data-ttu-id="59583-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59583-152">DateTimeOffset</span></span>|<span data-ttu-id="59583-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="59583-153">DateTime the object was created.</span></span> <span data-ttu-id="59583-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-155">description</span><span class="sxs-lookup"><span data-stu-id="59583-155">description</span></span>|<span data-ttu-id="59583-156">String</span><span class="sxs-lookup"><span data-stu-id="59583-156">String</span></span>|<span data-ttu-id="59583-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59583-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="59583-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-159">displayName</span><span class="sxs-lookup"><span data-stu-id="59583-159">displayName</span></span>|<span data-ttu-id="59583-160">String</span><span class="sxs-lookup"><span data-stu-id="59583-160">String</span></span>|<span data-ttu-id="59583-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59583-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="59583-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-163">versão</span><span class="sxs-lookup"><span data-stu-id="59583-163">version</span></span>|<span data-ttu-id="59583-164">Int32</span><span class="sxs-lookup"><span data-stu-id="59583-164">Int32</span></span>|<span data-ttu-id="59583-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59583-165">Version of the device configuration.</span></span> <span data-ttu-id="59583-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59583-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59583-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="59583-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="59583-168">Int32</span><span class="sxs-lookup"><span data-stu-id="59583-168">Int32</span></span>|<span data-ttu-id="59583-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="59583-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="59583-170">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="59583-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="59583-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="59583-171">subjectNameFormat</span></span>|[<span data-ttu-id="59583-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="59583-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="59583-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="59583-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="59583-174">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="59583-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="59583-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="59583-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="59583-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="59583-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="59583-177">Int32</span><span class="sxs-lookup"><span data-stu-id="59583-177">Int32</span></span>|<span data-ttu-id="59583-178">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="59583-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="59583-179">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="59583-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="59583-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="59583-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="59583-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="59583-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="59583-182">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="59583-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="59583-183">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="59583-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="59583-184">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="59583-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="59583-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="59583-185">extendedKeyUsages</span></span>|<span data-ttu-id="59583-186">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="59583-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="59583-187">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="59583-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="59583-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="59583-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="59583-189">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="59583-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="59583-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="59583-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="59583-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="59583-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="59583-192">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="59583-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="59583-193">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="59583-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="59583-194">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="59583-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="59583-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="59583-195">scepServerUrls</span></span>|<span data-ttu-id="59583-196">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="59583-196">String collection</span></span>|<span data-ttu-id="59583-197">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="59583-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="59583-198">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="59583-198">subjectNameFormatString</span></span>|<span data-ttu-id="59583-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59583-199">String</span></span>|<span data-ttu-id="59583-200">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="59583-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="59583-201">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="59583-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="59583-202">uso de</span><span class="sxs-lookup"><span data-stu-id="59583-202">keyUsage</span></span>|[<span data-ttu-id="59583-203">usos de</span><span class="sxs-lookup"><span data-stu-id="59583-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="59583-204">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="59583-204">SCEP Key Usage.</span></span> <span data-ttu-id="59583-205">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="59583-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="59583-206">keySize</span><span class="sxs-lookup"><span data-stu-id="59583-206">keySize</span></span>|[<span data-ttu-id="59583-207">keySize</span><span class="sxs-lookup"><span data-stu-id="59583-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="59583-208">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="59583-208">SCEP Key Size.</span></span> <span data-ttu-id="59583-209">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="59583-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="59583-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="59583-210">hashAlgorithm</span></span>|[<span data-ttu-id="59583-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="59583-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="59583-212">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="59583-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="59583-213">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="59583-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="59583-214">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="59583-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="59583-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59583-215">String</span></span>|<span data-ttu-id="59583-216">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="59583-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="59583-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="59583-217">certificateStore</span></span>|[<span data-ttu-id="59583-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="59583-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="59583-219">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="59583-219">Target store certificate.</span></span> <span data-ttu-id="59583-220">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="59583-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="59583-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="59583-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="59583-222">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="59583-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="59583-223">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="59583-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="59583-224">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="59583-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="59583-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="59583-225">Response</span></span>
<span data-ttu-id="59583-226">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59583-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59583-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59583-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="59583-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59583-228">Request</span></span>
<span data-ttu-id="59583-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59583-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="59583-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="59583-230">Response</span></span>
<span data-ttu-id="59583-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59583-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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




