---
title: Criar windowsPhone81SCEPCertificateProfile
description: Criar um novo objeto windowsPhone81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0f08c4802a77390945d4e25b94f66dc5228d97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512688"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="45640-103">Criar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="45640-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="45640-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45640-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45640-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45640-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45640-106">Criar um novo objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45640-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45640-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45640-107">Prerequisites</span></span>
<span data-ttu-id="45640-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45640-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45640-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45640-110">Permission type</span></span>|<span data-ttu-id="45640-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45640-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45640-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45640-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45640-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45640-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45640-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45640-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45640-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45640-115">Not supported.</span></span>|
|<span data-ttu-id="45640-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45640-116">Application</span></span>|<span data-ttu-id="45640-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45640-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45640-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45640-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45640-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45640-119">Request headers</span></span>
|<span data-ttu-id="45640-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45640-120">Header</span></span>|<span data-ttu-id="45640-121">Valor</span><span class="sxs-lookup"><span data-stu-id="45640-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45640-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="45640-122">Authorization</span></span>|<span data-ttu-id="45640-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45640-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45640-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45640-124">Accept</span></span>|<span data-ttu-id="45640-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45640-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45640-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45640-126">Request body</span></span>
<span data-ttu-id="45640-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="45640-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="45640-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="45640-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="45640-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45640-129">Property</span></span>|<span data-ttu-id="45640-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="45640-130">Type</span></span>|<span data-ttu-id="45640-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="45640-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45640-132">id</span><span class="sxs-lookup"><span data-stu-id="45640-132">id</span></span>|<span data-ttu-id="45640-133">String</span><span class="sxs-lookup"><span data-stu-id="45640-133">String</span></span>|<span data-ttu-id="45640-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45640-134">Key of the entity.</span></span> <span data-ttu-id="45640-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45640-136">lastModifiedDateTime</span></span>|<span data-ttu-id="45640-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45640-137">DateTimeOffset</span></span>|<span data-ttu-id="45640-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45640-138">DateTime the object was last modified.</span></span> <span data-ttu-id="45640-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45640-140">roleScopeTagIds</span></span>|<span data-ttu-id="45640-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45640-141">String collection</span></span>|<span data-ttu-id="45640-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="45640-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45640-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45640-144">supportsScopeTags</span></span>|<span data-ttu-id="45640-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="45640-145">Boolean</span></span>|<span data-ttu-id="45640-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="45640-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45640-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="45640-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45640-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="45640-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45640-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45640-149">This property is read-only.</span></span> <span data-ttu-id="45640-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45640-151">createdDateTime</span></span>|<span data-ttu-id="45640-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45640-152">DateTimeOffset</span></span>|<span data-ttu-id="45640-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45640-153">DateTime the object was created.</span></span> <span data-ttu-id="45640-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-155">description</span><span class="sxs-lookup"><span data-stu-id="45640-155">description</span></span>|<span data-ttu-id="45640-156">String</span><span class="sxs-lookup"><span data-stu-id="45640-156">String</span></span>|<span data-ttu-id="45640-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45640-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45640-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-159">displayName</span><span class="sxs-lookup"><span data-stu-id="45640-159">displayName</span></span>|<span data-ttu-id="45640-160">String</span><span class="sxs-lookup"><span data-stu-id="45640-160">String</span></span>|<span data-ttu-id="45640-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45640-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45640-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-163">versão</span><span class="sxs-lookup"><span data-stu-id="45640-163">version</span></span>|<span data-ttu-id="45640-164">Int32</span><span class="sxs-lookup"><span data-stu-id="45640-164">Int32</span></span>|<span data-ttu-id="45640-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45640-165">Version of the device configuration.</span></span> <span data-ttu-id="45640-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45640-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45640-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="45640-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="45640-168">Int32</span><span class="sxs-lookup"><span data-stu-id="45640-168">Int32</span></span>|<span data-ttu-id="45640-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="45640-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="45640-170">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45640-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="45640-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="45640-171">keyStorageProvider</span></span>|[<span data-ttu-id="45640-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="45640-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="45640-173">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="45640-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="45640-174">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45640-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="45640-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="45640-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="45640-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="45640-176">subjectNameFormat</span></span>|[<span data-ttu-id="45640-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="45640-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="45640-178">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="45640-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="45640-179">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45640-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="45640-180">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="45640-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="45640-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="45640-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="45640-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="45640-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="45640-183">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="45640-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="45640-184">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45640-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="45640-185">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="45640-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="45640-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="45640-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="45640-187">Int32</span><span class="sxs-lookup"><span data-stu-id="45640-187">Int32</span></span>|<span data-ttu-id="45640-188">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="45640-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="45640-189">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45640-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="45640-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45640-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="45640-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45640-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="45640-192">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="45640-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="45640-193">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45640-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="45640-194">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="45640-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="45640-195">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="45640-195">extendedKeyUsages</span></span>|<span data-ttu-id="45640-196">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="45640-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="45640-197">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="45640-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="45640-198">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45640-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="45640-199">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45640-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="45640-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="45640-200">scepServerUrls</span></span>|<span data-ttu-id="45640-201">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45640-201">String collection</span></span>|<span data-ttu-id="45640-202">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="45640-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="45640-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="45640-203">subjectNameFormatString</span></span>|<span data-ttu-id="45640-204">String</span><span class="sxs-lookup"><span data-stu-id="45640-204">String</span></span>|<span data-ttu-id="45640-205">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="45640-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="45640-206">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="45640-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="45640-207">uso de</span><span class="sxs-lookup"><span data-stu-id="45640-207">keyUsage</span></span>|[<span data-ttu-id="45640-208">usos de</span><span class="sxs-lookup"><span data-stu-id="45640-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="45640-209">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="45640-209">SCEP Key Usage.</span></span> <span data-ttu-id="45640-210">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="45640-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="45640-211">keySize</span><span class="sxs-lookup"><span data-stu-id="45640-211">keySize</span></span>|[<span data-ttu-id="45640-212">keySize</span><span class="sxs-lookup"><span data-stu-id="45640-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="45640-213">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="45640-213">SCEP Key Size.</span></span> <span data-ttu-id="45640-214">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="45640-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="45640-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="45640-215">hashAlgorithm</span></span>|[<span data-ttu-id="45640-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="45640-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="45640-217">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="45640-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="45640-218">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="45640-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="45640-219">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="45640-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="45640-220">String</span><span class="sxs-lookup"><span data-stu-id="45640-220">String</span></span>|<span data-ttu-id="45640-221">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="45640-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="45640-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="45640-222">Response</span></span>
<span data-ttu-id="45640-223">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45640-223">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45640-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45640-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="45640-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45640-225">Request</span></span>
<span data-ttu-id="45640-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45640-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45640-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="45640-227">Response</span></span>
<span data-ttu-id="45640-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45640-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





