---
title: Criar windowsPhone81SCEPCertificateProfile
description: Criar um novo objeto windowsPhone81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69222d314245f9d25eedcc712bb05441ae7d9a72
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971525"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="95726-103">Criar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="95726-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="95726-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95726-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95726-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95726-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95726-106">Criar um novo objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="95726-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95726-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95726-107">Prerequisites</span></span>
<span data-ttu-id="95726-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95726-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95726-110">Permission type</span></span>|<span data-ttu-id="95726-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95726-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95726-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95726-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95726-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95726-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95726-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95726-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95726-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95726-115">Not supported.</span></span>|
|<span data-ttu-id="95726-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95726-116">Application</span></span>|<span data-ttu-id="95726-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95726-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95726-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95726-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95726-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95726-119">Request headers</span></span>
|<span data-ttu-id="95726-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95726-120">Header</span></span>|<span data-ttu-id="95726-121">Valor</span><span class="sxs-lookup"><span data-stu-id="95726-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95726-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95726-122">Authorization</span></span>|<span data-ttu-id="95726-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95726-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95726-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95726-124">Accept</span></span>|<span data-ttu-id="95726-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95726-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95726-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95726-126">Request body</span></span>
<span data-ttu-id="95726-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="95726-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="95726-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="95726-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="95726-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95726-129">Property</span></span>|<span data-ttu-id="95726-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="95726-130">Type</span></span>|<span data-ttu-id="95726-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="95726-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95726-132">id</span><span class="sxs-lookup"><span data-stu-id="95726-132">id</span></span>|<span data-ttu-id="95726-133">String</span><span class="sxs-lookup"><span data-stu-id="95726-133">String</span></span>|<span data-ttu-id="95726-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95726-134">Key of the entity.</span></span> <span data-ttu-id="95726-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95726-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95726-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95726-137">DateTimeOffset</span></span>|<span data-ttu-id="95726-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="95726-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95726-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95726-140">roleScopeTagIds</span></span>|<span data-ttu-id="95726-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="95726-141">String collection</span></span>|<span data-ttu-id="95726-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="95726-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95726-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95726-144">supportsScopeTags</span></span>|<span data-ttu-id="95726-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95726-145">Boolean</span></span>|<span data-ttu-id="95726-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="95726-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95726-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="95726-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95726-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="95726-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95726-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95726-149">This property is read-only.</span></span> <span data-ttu-id="95726-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95726-151">createdDateTime</span></span>|<span data-ttu-id="95726-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95726-152">DateTimeOffset</span></span>|<span data-ttu-id="95726-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="95726-153">DateTime the object was created.</span></span> <span data-ttu-id="95726-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-155">descrição</span><span class="sxs-lookup"><span data-stu-id="95726-155">description</span></span>|<span data-ttu-id="95726-156">String</span><span class="sxs-lookup"><span data-stu-id="95726-156">String</span></span>|<span data-ttu-id="95726-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95726-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95726-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-159">displayName</span><span class="sxs-lookup"><span data-stu-id="95726-159">displayName</span></span>|<span data-ttu-id="95726-160">String</span><span class="sxs-lookup"><span data-stu-id="95726-160">String</span></span>|<span data-ttu-id="95726-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95726-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95726-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-163">versão</span><span class="sxs-lookup"><span data-stu-id="95726-163">version</span></span>|<span data-ttu-id="95726-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95726-164">Int32</span></span>|<span data-ttu-id="95726-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95726-165">Version of the device configuration.</span></span> <span data-ttu-id="95726-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95726-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95726-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="95726-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="95726-168">Int32</span><span class="sxs-lookup"><span data-stu-id="95726-168">Int32</span></span>|<span data-ttu-id="95726-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="95726-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="95726-170">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="95726-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="95726-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="95726-171">keyStorageProvider</span></span>|[<span data-ttu-id="95726-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="95726-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="95726-173">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="95726-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="95726-174">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="95726-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="95726-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="95726-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="95726-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="95726-176">subjectNameFormat</span></span>|[<span data-ttu-id="95726-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="95726-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="95726-178">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="95726-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="95726-179">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="95726-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="95726-180">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="95726-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="95726-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95726-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="95726-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95726-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="95726-183">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="95726-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="95726-184">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="95726-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="95726-185">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="95726-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="95726-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="95726-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="95726-187">Int32</span><span class="sxs-lookup"><span data-stu-id="95726-187">Int32</span></span>|<span data-ttu-id="95726-188">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="95726-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="95726-189">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="95726-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="95726-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="95726-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="95726-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="95726-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="95726-192">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="95726-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="95726-193">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="95726-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="95726-194">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="95726-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="95726-195">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="95726-195">extendedKeyUsages</span></span>|<span data-ttu-id="95726-196">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="95726-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="95726-197">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="95726-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="95726-198">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="95726-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="95726-199">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="95726-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="95726-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="95726-200">scepServerUrls</span></span>|<span data-ttu-id="95726-201">Coleção String</span><span class="sxs-lookup"><span data-stu-id="95726-201">String collection</span></span>|<span data-ttu-id="95726-202">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="95726-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="95726-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="95726-203">subjectNameFormatString</span></span>|<span data-ttu-id="95726-204">String</span><span class="sxs-lookup"><span data-stu-id="95726-204">String</span></span>|<span data-ttu-id="95726-205">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="95726-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="95726-206">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="95726-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="95726-207">uso de</span><span class="sxs-lookup"><span data-stu-id="95726-207">keyUsage</span></span>|[<span data-ttu-id="95726-208">usos de</span><span class="sxs-lookup"><span data-stu-id="95726-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="95726-209">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="95726-209">SCEP Key Usage.</span></span> <span data-ttu-id="95726-210">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="95726-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="95726-211">keySize</span><span class="sxs-lookup"><span data-stu-id="95726-211">keySize</span></span>|[<span data-ttu-id="95726-212">keySize</span><span class="sxs-lookup"><span data-stu-id="95726-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="95726-213">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="95726-213">SCEP Key Size.</span></span> <span data-ttu-id="95726-214">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="95726-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="95726-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="95726-215">hashAlgorithm</span></span>|[<span data-ttu-id="95726-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="95726-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="95726-217">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="95726-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="95726-218">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="95726-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="95726-219">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="95726-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="95726-220">String</span><span class="sxs-lookup"><span data-stu-id="95726-220">String</span></span>|<span data-ttu-id="95726-221">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="95726-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="95726-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="95726-222">Response</span></span>
<span data-ttu-id="95726-223">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95726-223">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95726-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95726-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="95726-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95726-225">Request</span></span>
<span data-ttu-id="95726-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95726-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="95726-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="95726-227">Response</span></span>
<span data-ttu-id="95726-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95726-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




