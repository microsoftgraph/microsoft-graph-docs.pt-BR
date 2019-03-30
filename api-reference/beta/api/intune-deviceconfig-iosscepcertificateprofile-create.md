---
title: Criar iosScepCertificateProfile
description: Criar um novo objeto iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bd52508ef7ffd5581edc988356edbce2eba2d4e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988046"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="50c69-103">Criar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="50c69-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="50c69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50c69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50c69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50c69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50c69-106">Criar um novo objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="50c69-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50c69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50c69-107">Prerequisites</span></span>
<span data-ttu-id="50c69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50c69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50c69-110">Permission type</span></span>|<span data-ttu-id="50c69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50c69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50c69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50c69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50c69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50c69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50c69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50c69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50c69-115">Not supported.</span></span>|
|<span data-ttu-id="50c69-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50c69-116">Application</span></span>|<span data-ttu-id="50c69-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50c69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50c69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50c69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50c69-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50c69-119">Request headers</span></span>
|<span data-ttu-id="50c69-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50c69-120">Header</span></span>|<span data-ttu-id="50c69-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50c69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50c69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50c69-122">Authorization</span></span>|<span data-ttu-id="50c69-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50c69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50c69-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50c69-124">Accept</span></span>|<span data-ttu-id="50c69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50c69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50c69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50c69-126">Request body</span></span>
<span data-ttu-id="50c69-127">No corpo da solicitação, forneça uma representação JSON do objeto iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="50c69-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="50c69-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="50c69-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="50c69-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50c69-129">Property</span></span>|<span data-ttu-id="50c69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50c69-130">Type</span></span>|<span data-ttu-id="50c69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50c69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50c69-132">id</span><span class="sxs-lookup"><span data-stu-id="50c69-132">id</span></span>|<span data-ttu-id="50c69-133">String</span><span class="sxs-lookup"><span data-stu-id="50c69-133">String</span></span>|<span data-ttu-id="50c69-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50c69-134">Key of the entity.</span></span> <span data-ttu-id="50c69-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50c69-136">lastModifiedDateTime</span></span>|<span data-ttu-id="50c69-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50c69-137">DateTimeOffset</span></span>|<span data-ttu-id="50c69-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="50c69-138">DateTime the object was last modified.</span></span> <span data-ttu-id="50c69-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50c69-140">roleScopeTagIds</span></span>|<span data-ttu-id="50c69-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="50c69-141">String collection</span></span>|<span data-ttu-id="50c69-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="50c69-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50c69-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="50c69-144">supportsScopeTags</span></span>|<span data-ttu-id="50c69-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="50c69-145">Boolean</span></span>|<span data-ttu-id="50c69-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="50c69-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50c69-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="50c69-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50c69-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="50c69-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50c69-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50c69-149">This property is read-only.</span></span> <span data-ttu-id="50c69-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50c69-151">createdDateTime</span></span>|<span data-ttu-id="50c69-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50c69-152">DateTimeOffset</span></span>|<span data-ttu-id="50c69-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="50c69-153">DateTime the object was created.</span></span> <span data-ttu-id="50c69-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-155">description</span><span class="sxs-lookup"><span data-stu-id="50c69-155">description</span></span>|<span data-ttu-id="50c69-156">String</span><span class="sxs-lookup"><span data-stu-id="50c69-156">String</span></span>|<span data-ttu-id="50c69-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50c69-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50c69-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-159">displayName</span><span class="sxs-lookup"><span data-stu-id="50c69-159">displayName</span></span>|<span data-ttu-id="50c69-160">String</span><span class="sxs-lookup"><span data-stu-id="50c69-160">String</span></span>|<span data-ttu-id="50c69-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50c69-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50c69-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-163">versão</span><span class="sxs-lookup"><span data-stu-id="50c69-163">version</span></span>|<span data-ttu-id="50c69-164">Int32</span><span class="sxs-lookup"><span data-stu-id="50c69-164">Int32</span></span>|<span data-ttu-id="50c69-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50c69-165">Version of the device configuration.</span></span> <span data-ttu-id="50c69-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50c69-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="50c69-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="50c69-168">Int32</span><span class="sxs-lookup"><span data-stu-id="50c69-168">Int32</span></span>|<span data-ttu-id="50c69-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="50c69-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="50c69-170">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50c69-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="50c69-171">subjectNameFormat</span></span>|[<span data-ttu-id="50c69-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="50c69-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="50c69-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50c69-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="50c69-174">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50c69-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="50c69-175">Os valores possíveis são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="50c69-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="50c69-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="50c69-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="50c69-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="50c69-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="50c69-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50c69-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="50c69-179">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50c69-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="50c69-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="50c69-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="50c69-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="50c69-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="50c69-182">Int32</span><span class="sxs-lookup"><span data-stu-id="50c69-182">Int32</span></span>|<span data-ttu-id="50c69-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50c69-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="50c69-184">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50c69-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="50c69-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="50c69-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="50c69-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="50c69-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="50c69-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="50c69-188">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50c69-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="50c69-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="50c69-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="50c69-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="50c69-190">scepServerUrls</span></span>|<span data-ttu-id="50c69-191">Coleção String</span><span class="sxs-lookup"><span data-stu-id="50c69-191">String collection</span></span>|<span data-ttu-id="50c69-192">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="50c69-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="50c69-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="50c69-193">subjectNameFormatString</span></span>|<span data-ttu-id="50c69-194">String</span><span class="sxs-lookup"><span data-stu-id="50c69-194">String</span></span>|<span data-ttu-id="50c69-195">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="50c69-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="50c69-196">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="50c69-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="50c69-197">uso de</span><span class="sxs-lookup"><span data-stu-id="50c69-197">keyUsage</span></span>|[<span data-ttu-id="50c69-198">usos de</span><span class="sxs-lookup"><span data-stu-id="50c69-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="50c69-199">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="50c69-199">SCEP Key Usage.</span></span> <span data-ttu-id="50c69-200">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="50c69-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="50c69-201">keySize</span><span class="sxs-lookup"><span data-stu-id="50c69-201">keySize</span></span>|[<span data-ttu-id="50c69-202">keySize</span><span class="sxs-lookup"><span data-stu-id="50c69-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="50c69-203">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="50c69-203">SCEP Key Size.</span></span> <span data-ttu-id="50c69-204">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="50c69-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="50c69-205">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="50c69-205">extendedKeyUsages</span></span>|<span data-ttu-id="50c69-206">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="50c69-207">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="50c69-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="50c69-208">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="50c69-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="50c69-209">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="50c69-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="50c69-210">String</span><span class="sxs-lookup"><span data-stu-id="50c69-210">String</span></span>|<span data-ttu-id="50c69-211">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="50c69-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="50c69-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="50c69-212">certificateStore</span></span>|[<span data-ttu-id="50c69-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="50c69-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="50c69-214">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="50c69-214">Target store certificate.</span></span> <span data-ttu-id="50c69-215">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="50c69-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="50c69-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="50c69-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="50c69-217">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="50c69-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="50c69-218">Definições de nome alterantive da entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="50c69-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="50c69-219">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="50c69-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="50c69-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="50c69-220">Response</span></span>
<span data-ttu-id="50c69-221">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50c69-221">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50c69-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50c69-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="50c69-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50c69-223">Request</span></span>
<span data-ttu-id="50c69-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50c69-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="50c69-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="50c69-225">Response</span></span>
<span data-ttu-id="50c69-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50c69-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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




