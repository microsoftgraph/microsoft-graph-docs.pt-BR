---
title: Atualizar androidForWorkScepCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d881c970d1c0b559c51802d4553f56c003673bf0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774425"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="35bbc-103">Atualizar androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="35bbc-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="35bbc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35bbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35bbc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35bbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35bbc-106">Atualiza as propriedades de um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="35bbc-106">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35bbc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35bbc-107">Prerequisites</span></span>
<span data-ttu-id="35bbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35bbc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35bbc-110">Permission type</span></span>|<span data-ttu-id="35bbc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35bbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35bbc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35bbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35bbc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35bbc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35bbc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35bbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35bbc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35bbc-115">Not supported.</span></span>|
|<span data-ttu-id="35bbc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35bbc-116">Application</span></span>|<span data-ttu-id="35bbc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35bbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35bbc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35bbc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="35bbc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35bbc-119">Request headers</span></span>
|<span data-ttu-id="35bbc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35bbc-120">Header</span></span>|<span data-ttu-id="35bbc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="35bbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35bbc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="35bbc-122">Authorization</span></span>|<span data-ttu-id="35bbc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35bbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35bbc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35bbc-124">Accept</span></span>|<span data-ttu-id="35bbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35bbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35bbc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35bbc-126">Request body</span></span>
<span data-ttu-id="35bbc-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="35bbc-127">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="35bbc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="35bbc-128">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="35bbc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35bbc-129">Property</span></span>|<span data-ttu-id="35bbc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="35bbc-130">Type</span></span>|<span data-ttu-id="35bbc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="35bbc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35bbc-132">id</span><span class="sxs-lookup"><span data-stu-id="35bbc-132">id</span></span>|<span data-ttu-id="35bbc-133">String</span><span class="sxs-lookup"><span data-stu-id="35bbc-133">String</span></span>|<span data-ttu-id="35bbc-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35bbc-134">Key of the entity.</span></span> <span data-ttu-id="35bbc-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35bbc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="35bbc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35bbc-137">DateTimeOffset</span></span>|<span data-ttu-id="35bbc-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="35bbc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="35bbc-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35bbc-140">roleScopeTagIds</span></span>|<span data-ttu-id="35bbc-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="35bbc-141">String collection</span></span>|<span data-ttu-id="35bbc-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="35bbc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35bbc-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35bbc-144">supportsScopeTags</span></span>|<span data-ttu-id="35bbc-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="35bbc-145">Boolean</span></span>|<span data-ttu-id="35bbc-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="35bbc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35bbc-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="35bbc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35bbc-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="35bbc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35bbc-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35bbc-149">This property is read-only.</span></span> <span data-ttu-id="35bbc-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35bbc-151">createdDateTime</span></span>|<span data-ttu-id="35bbc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35bbc-152">DateTimeOffset</span></span>|<span data-ttu-id="35bbc-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="35bbc-153">DateTime the object was created.</span></span> <span data-ttu-id="35bbc-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-155">description</span><span class="sxs-lookup"><span data-stu-id="35bbc-155">description</span></span>|<span data-ttu-id="35bbc-156">String</span><span class="sxs-lookup"><span data-stu-id="35bbc-156">String</span></span>|<span data-ttu-id="35bbc-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35bbc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35bbc-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="35bbc-159">displayName</span></span>|<span data-ttu-id="35bbc-160">String</span><span class="sxs-lookup"><span data-stu-id="35bbc-160">String</span></span>|<span data-ttu-id="35bbc-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35bbc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35bbc-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-163">versão</span><span class="sxs-lookup"><span data-stu-id="35bbc-163">version</span></span>|<span data-ttu-id="35bbc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="35bbc-164">Int32</span></span>|<span data-ttu-id="35bbc-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35bbc-165">Version of the device configuration.</span></span> <span data-ttu-id="35bbc-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35bbc-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="35bbc-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="35bbc-168">Int32</span><span class="sxs-lookup"><span data-stu-id="35bbc-168">Int32</span></span>|<span data-ttu-id="35bbc-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="35bbc-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="35bbc-170">Valores válidos de 1 a 99 herdados de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="35bbc-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="35bbc-171">subjectNameFormat</span></span>|[<span data-ttu-id="35bbc-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="35bbc-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="35bbc-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="35bbc-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="35bbc-174">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="35bbc-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="35bbc-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="35bbc-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="35bbc-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="35bbc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="35bbc-177">Int32</span></span>|<span data-ttu-id="35bbc-178">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="35bbc-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="35bbc-179">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="35bbc-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="35bbc-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="35bbc-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="35bbc-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="35bbc-182">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="35bbc-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="35bbc-183">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="35bbc-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="35bbc-184">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="35bbc-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="35bbc-185">extendedKeyUsages</span></span>|<span data-ttu-id="35bbc-186">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="35bbc-187">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="35bbc-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="35bbc-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35bbc-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="35bbc-189">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="35bbc-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="35bbc-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="35bbc-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="35bbc-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="35bbc-192">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="35bbc-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="35bbc-193">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="35bbc-193">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="35bbc-194">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="35bbc-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="35bbc-195">scepServerUrls</span></span>|<span data-ttu-id="35bbc-196">Coleção String</span><span class="sxs-lookup"><span data-stu-id="35bbc-196">String collection</span></span>|<span data-ttu-id="35bbc-197">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="35bbc-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="35bbc-198">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="35bbc-198">subjectNameFormatString</span></span>|<span data-ttu-id="35bbc-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35bbc-199">String</span></span>|<span data-ttu-id="35bbc-200">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="35bbc-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="35bbc-201">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="35bbc-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="35bbc-202">uso de</span><span class="sxs-lookup"><span data-stu-id="35bbc-202">keyUsage</span></span>|[<span data-ttu-id="35bbc-203">usos de</span><span class="sxs-lookup"><span data-stu-id="35bbc-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="35bbc-204">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="35bbc-204">SCEP Key Usage.</span></span> <span data-ttu-id="35bbc-205">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="35bbc-206">keySize</span><span class="sxs-lookup"><span data-stu-id="35bbc-206">keySize</span></span>|[<span data-ttu-id="35bbc-207">keySize</span><span class="sxs-lookup"><span data-stu-id="35bbc-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="35bbc-208">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="35bbc-208">SCEP Key Size.</span></span> <span data-ttu-id="35bbc-209">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="35bbc-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="35bbc-210">hashAlgorithm</span></span>|[<span data-ttu-id="35bbc-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="35bbc-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="35bbc-212">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="35bbc-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="35bbc-213">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="35bbc-214">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="35bbc-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="35bbc-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35bbc-215">String</span></span>|<span data-ttu-id="35bbc-216">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="35bbc-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="35bbc-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="35bbc-217">certificateStore</span></span>|[<span data-ttu-id="35bbc-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="35bbc-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="35bbc-219">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="35bbc-219">Target store certificate.</span></span> <span data-ttu-id="35bbc-220">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="35bbc-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="35bbc-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="35bbc-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="35bbc-222">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="35bbc-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="35bbc-223">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="35bbc-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="35bbc-224">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35bbc-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="35bbc-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="35bbc-225">Response</span></span>
<span data-ttu-id="35bbc-226">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35bbc-226">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35bbc-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35bbc-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="35bbc-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35bbc-228">Request</span></span>
<span data-ttu-id="35bbc-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35bbc-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35bbc-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="35bbc-230">Response</span></span>
<span data-ttu-id="35bbc-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35bbc-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





