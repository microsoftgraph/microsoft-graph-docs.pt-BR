---
title: Atualizar androidForWorkScepCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad30c1f03032efbb582b5832814090d5d5106bbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157964"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="abfca-103">Atualizar androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="abfca-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="abfca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abfca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abfca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abfca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abfca-106">Atualiza as propriedades de um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="abfca-106">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abfca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abfca-107">Prerequisites</span></span>
<span data-ttu-id="abfca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="abfca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="abfca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abfca-110">Permission type</span></span>|<span data-ttu-id="abfca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abfca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abfca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abfca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abfca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abfca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abfca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abfca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abfca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abfca-115">Not supported.</span></span>|
|<span data-ttu-id="abfca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abfca-116">Application</span></span>|<span data-ttu-id="abfca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abfca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abfca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abfca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="abfca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abfca-119">Request headers</span></span>
|<span data-ttu-id="abfca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abfca-120">Header</span></span>|<span data-ttu-id="abfca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="abfca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abfca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abfca-122">Authorization</span></span>|<span data-ttu-id="abfca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abfca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abfca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abfca-124">Accept</span></span>|<span data-ttu-id="abfca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abfca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abfca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abfca-126">Request body</span></span>
<span data-ttu-id="abfca-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="abfca-127">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="abfca-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="abfca-128">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="abfca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abfca-129">Property</span></span>|<span data-ttu-id="abfca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="abfca-130">Type</span></span>|<span data-ttu-id="abfca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abfca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abfca-132">id</span><span class="sxs-lookup"><span data-stu-id="abfca-132">id</span></span>|<span data-ttu-id="abfca-133">String</span><span class="sxs-lookup"><span data-stu-id="abfca-133">String</span></span>|<span data-ttu-id="abfca-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="abfca-134">Key of the entity.</span></span> <span data-ttu-id="abfca-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abfca-136">lastModifiedDateTime</span></span>|<span data-ttu-id="abfca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abfca-137">DateTimeOffset</span></span>|<span data-ttu-id="abfca-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="abfca-138">DateTime the object was last modified.</span></span> <span data-ttu-id="abfca-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="abfca-140">roleScopeTagIds</span></span>|<span data-ttu-id="abfca-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abfca-141">String collection</span></span>|<span data-ttu-id="abfca-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="abfca-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="abfca-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="abfca-144">supportsScopeTags</span></span>|<span data-ttu-id="abfca-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="abfca-145">Boolean</span></span>|<span data-ttu-id="abfca-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="abfca-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="abfca-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="abfca-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="abfca-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="abfca-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="abfca-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="abfca-149">This property is read-only.</span></span> <span data-ttu-id="abfca-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abfca-151">createdDateTime</span></span>|<span data-ttu-id="abfca-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abfca-152">DateTimeOffset</span></span>|<span data-ttu-id="abfca-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="abfca-153">DateTime the object was created.</span></span> <span data-ttu-id="abfca-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-155">description</span><span class="sxs-lookup"><span data-stu-id="abfca-155">description</span></span>|<span data-ttu-id="abfca-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abfca-156">String</span></span>|<span data-ttu-id="abfca-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abfca-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="abfca-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-159">displayName</span><span class="sxs-lookup"><span data-stu-id="abfca-159">displayName</span></span>|<span data-ttu-id="abfca-160">String</span><span class="sxs-lookup"><span data-stu-id="abfca-160">String</span></span>|<span data-ttu-id="abfca-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abfca-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="abfca-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-163">version</span><span class="sxs-lookup"><span data-stu-id="abfca-163">version</span></span>|<span data-ttu-id="abfca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="abfca-164">Int32</span></span>|<span data-ttu-id="abfca-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abfca-165">Version of the device configuration.</span></span> <span data-ttu-id="abfca-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abfca-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="abfca-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="abfca-168">Int32</span><span class="sxs-lookup"><span data-stu-id="abfca-168">Int32</span></span>|<span data-ttu-id="abfca-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="abfca-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="abfca-170">Valores válidos de 1 a 99 herdados de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="abfca-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="abfca-171">subjectNameFormat</span></span>|[<span data-ttu-id="abfca-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="abfca-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="abfca-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="abfca-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="abfca-174">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="abfca-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="abfca-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="abfca-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="abfca-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="abfca-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="abfca-177">Int32</span><span class="sxs-lookup"><span data-stu-id="abfca-177">Int32</span></span>|<span data-ttu-id="abfca-178">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="abfca-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="abfca-179">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="abfca-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="abfca-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="abfca-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="abfca-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="abfca-182">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="abfca-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="abfca-183">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="abfca-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="abfca-184">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="abfca-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="abfca-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="abfca-185">extendedKeyUsages</span></span>|<span data-ttu-id="abfca-186">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="abfca-187">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="abfca-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="abfca-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="abfca-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="abfca-189">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="abfca-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="abfca-190">scepServerUrls</span></span>|<span data-ttu-id="abfca-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abfca-191">String collection</span></span>|<span data-ttu-id="abfca-192">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="abfca-192">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="abfca-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="abfca-193">subjectNameFormatString</span></span>|<span data-ttu-id="abfca-194">String</span><span class="sxs-lookup"><span data-stu-id="abfca-194">String</span></span>|<span data-ttu-id="abfca-195">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="abfca-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="abfca-196">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="abfca-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="abfca-197">uso de</span><span class="sxs-lookup"><span data-stu-id="abfca-197">keyUsage</span></span>|[<span data-ttu-id="abfca-198">usos de</span><span class="sxs-lookup"><span data-stu-id="abfca-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="abfca-199">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="abfca-199">SCEP Key Usage.</span></span> <span data-ttu-id="abfca-200">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="abfca-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="abfca-201">keySize</span><span class="sxs-lookup"><span data-stu-id="abfca-201">keySize</span></span>|[<span data-ttu-id="abfca-202">keySize</span><span class="sxs-lookup"><span data-stu-id="abfca-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="abfca-203">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="abfca-203">SCEP Key Size.</span></span> <span data-ttu-id="abfca-204">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="abfca-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="abfca-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="abfca-205">hashAlgorithm</span></span>|[<span data-ttu-id="abfca-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="abfca-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="abfca-207">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="abfca-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="abfca-208">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="abfca-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="abfca-209">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="abfca-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="abfca-210">String</span><span class="sxs-lookup"><span data-stu-id="abfca-210">String</span></span>|<span data-ttu-id="abfca-211">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="abfca-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="abfca-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="abfca-212">certificateStore</span></span>|[<span data-ttu-id="abfca-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="abfca-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="abfca-214">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="abfca-214">Target store certificate.</span></span> <span data-ttu-id="abfca-215">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="abfca-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="abfca-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="abfca-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="abfca-217">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="abfca-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="abfca-218">Definições de nome alterantive da entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="abfca-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="abfca-219">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="abfca-219">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="abfca-220">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="abfca-220">subjectAlternativeNameType</span></span>|[<span data-ttu-id="abfca-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="abfca-221">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="abfca-222">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="abfca-222">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="abfca-223">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="abfca-223">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="abfca-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="abfca-224">Response</span></span>
<span data-ttu-id="abfca-225">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abfca-225">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abfca-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abfca-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="abfca-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abfca-227">Request</span></span>
<span data-ttu-id="abfca-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abfca-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1205

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="abfca-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="abfca-229">Response</span></span>
<span data-ttu-id="abfca-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abfca-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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




