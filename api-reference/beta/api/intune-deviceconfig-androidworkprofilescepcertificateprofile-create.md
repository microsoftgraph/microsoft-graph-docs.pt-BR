---
title: Criar Entidadeandroidworkprofilescepcertificateprofile
description: Criar um novo objeto Entidadeandroidworkprofilescepcertificateprofile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5046a1f8ffc8c2c2850e3e2a0b900e35be6e2d07
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981871"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="fb178-103">Criar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="fb178-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="fb178-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb178-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb178-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb178-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb178-106">Criar um novo objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fb178-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb178-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb178-107">Prerequisites</span></span>
<span data-ttu-id="fb178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb178-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb178-110">Permission type</span></span>|<span data-ttu-id="fb178-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb178-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb178-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb178-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb178-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb178-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb178-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb178-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb178-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb178-115">Not supported.</span></span>|
|<span data-ttu-id="fb178-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb178-116">Application</span></span>|<span data-ttu-id="fb178-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb178-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb178-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb178-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb178-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb178-119">Request headers</span></span>
|<span data-ttu-id="fb178-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb178-120">Header</span></span>|<span data-ttu-id="fb178-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb178-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb178-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb178-122">Authorization</span></span>|<span data-ttu-id="fb178-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb178-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb178-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb178-124">Accept</span></span>|<span data-ttu-id="fb178-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb178-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb178-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb178-126">Request body</span></span>
<span data-ttu-id="fb178-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidworkprofilescepcertificateprofile.</span><span class="sxs-lookup"><span data-stu-id="fb178-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="fb178-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidworkprofilescepcertificateprofile.</span><span class="sxs-lookup"><span data-stu-id="fb178-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="fb178-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb178-129">Property</span></span>|<span data-ttu-id="fb178-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb178-130">Type</span></span>|<span data-ttu-id="fb178-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb178-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb178-132">id</span><span class="sxs-lookup"><span data-stu-id="fb178-132">id</span></span>|<span data-ttu-id="fb178-133">String</span><span class="sxs-lookup"><span data-stu-id="fb178-133">String</span></span>|<span data-ttu-id="fb178-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fb178-134">Key of the entity.</span></span> <span data-ttu-id="fb178-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb178-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fb178-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb178-137">DateTimeOffset</span></span>|<span data-ttu-id="fb178-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fb178-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fb178-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb178-140">roleScopeTagIds</span></span>|<span data-ttu-id="fb178-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="fb178-141">String collection</span></span>|<span data-ttu-id="fb178-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fb178-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fb178-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fb178-144">supportsScopeTags</span></span>|<span data-ttu-id="fb178-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb178-145">Boolean</span></span>|<span data-ttu-id="fb178-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="fb178-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fb178-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="fb178-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fb178-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fb178-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fb178-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb178-149">This property is read-only.</span></span> <span data-ttu-id="fb178-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb178-151">createdDateTime</span></span>|<span data-ttu-id="fb178-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb178-152">DateTimeOffset</span></span>|<span data-ttu-id="fb178-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fb178-153">DateTime the object was created.</span></span> <span data-ttu-id="fb178-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-155">descrição</span><span class="sxs-lookup"><span data-stu-id="fb178-155">description</span></span>|<span data-ttu-id="fb178-156">String</span><span class="sxs-lookup"><span data-stu-id="fb178-156">String</span></span>|<span data-ttu-id="fb178-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb178-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb178-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fb178-159">displayName</span></span>|<span data-ttu-id="fb178-160">String</span><span class="sxs-lookup"><span data-stu-id="fb178-160">String</span></span>|<span data-ttu-id="fb178-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb178-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb178-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-163">versão</span><span class="sxs-lookup"><span data-stu-id="fb178-163">version</span></span>|<span data-ttu-id="fb178-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fb178-164">Int32</span></span>|<span data-ttu-id="fb178-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb178-165">Version of the device configuration.</span></span> <span data-ttu-id="fb178-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb178-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="fb178-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="fb178-168">Int32</span><span class="sxs-lookup"><span data-stu-id="fb178-168">Int32</span></span>|<span data-ttu-id="fb178-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="fb178-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fb178-170">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fb178-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fb178-171">subjectNameFormat</span></span>|[<span data-ttu-id="fb178-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fb178-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="fb178-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fb178-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="fb178-174">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fb178-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="fb178-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="fb178-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="fb178-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fb178-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fb178-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fb178-177">Int32</span></span>|<span data-ttu-id="fb178-178">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fb178-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="fb178-179">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fb178-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fb178-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fb178-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fb178-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fb178-182">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fb178-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="fb178-183">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fb178-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="fb178-184">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="fb178-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fb178-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="fb178-185">extendedKeyUsages</span></span>|<span data-ttu-id="fb178-186">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="fb178-187">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="fb178-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="fb178-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fb178-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fb178-189">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fb178-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="fb178-190">scepServerUrls</span></span>|<span data-ttu-id="fb178-191">Coleção String</span><span class="sxs-lookup"><span data-stu-id="fb178-191">String collection</span></span>|<span data-ttu-id="fb178-192">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="fb178-192">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="fb178-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fb178-193">subjectNameFormatString</span></span>|<span data-ttu-id="fb178-194">String</span><span class="sxs-lookup"><span data-stu-id="fb178-194">String</span></span>|<span data-ttu-id="fb178-195">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="fb178-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="fb178-196">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="fb178-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="fb178-197">uso de</span><span class="sxs-lookup"><span data-stu-id="fb178-197">keyUsage</span></span>|[<span data-ttu-id="fb178-198">usos de</span><span class="sxs-lookup"><span data-stu-id="fb178-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="fb178-199">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="fb178-199">SCEP Key Usage.</span></span> <span data-ttu-id="fb178-200">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="fb178-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="fb178-201">keySize</span><span class="sxs-lookup"><span data-stu-id="fb178-201">keySize</span></span>|[<span data-ttu-id="fb178-202">keySize</span><span class="sxs-lookup"><span data-stu-id="fb178-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="fb178-203">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="fb178-203">SCEP Key Size.</span></span> <span data-ttu-id="fb178-204">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="fb178-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="fb178-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="fb178-205">hashAlgorithm</span></span>|[<span data-ttu-id="fb178-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="fb178-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="fb178-207">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="fb178-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="fb178-208">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="fb178-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="fb178-209">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="fb178-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="fb178-210">String</span><span class="sxs-lookup"><span data-stu-id="fb178-210">String</span></span>|<span data-ttu-id="fb178-211">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="fb178-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="fb178-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fb178-212">certificateStore</span></span>|[<span data-ttu-id="fb178-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fb178-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="fb178-214">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="fb178-214">Target store certificate.</span></span> <span data-ttu-id="fb178-215">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="fb178-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="fb178-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="fb178-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="fb178-217">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="fb178-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="fb178-218">Definições de nome alterantive da entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="fb178-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="fb178-219">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fb178-219">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fb178-220">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fb178-220">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fb178-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fb178-221">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fb178-222">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fb178-222">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="fb178-223">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="fb178-223">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="fb178-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb178-224">Response</span></span>
<span data-ttu-id="fb178-225">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb178-225">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb178-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb178-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb178-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb178-227">Request</span></span>
<span data-ttu-id="fb178-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb178-228">Here is an example of the request.</span></span>
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
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="fb178-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb178-229">Response</span></span>
<span data-ttu-id="fb178-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb178-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```




