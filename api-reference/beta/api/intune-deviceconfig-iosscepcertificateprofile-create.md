---
title: Criar iosScepCertificateProfile
description: Crie um novo objeto de iosScepCertificateProfile.
ms.openlocfilehash: 64f0db48d1c1a96883942513d4b822850d2269e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034534"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="16287-103">Criar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="16287-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="16287-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16287-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16287-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16287-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16287-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16287-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16287-107">Crie um novo objeto de [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16287-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16287-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16287-108">Prerequisites</span></span>
<span data-ttu-id="16287-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16287-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16287-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16287-111">Permission type</span></span>|<span data-ttu-id="16287-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16287-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16287-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16287-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16287-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16287-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16287-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16287-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16287-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16287-116">Not supported.</span></span>|
|<span data-ttu-id="16287-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16287-117">Application</span></span>|<span data-ttu-id="16287-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16287-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16287-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16287-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="16287-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16287-120">Request headers</span></span>
|<span data-ttu-id="16287-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16287-121">Header</span></span>|<span data-ttu-id="16287-122">Valor</span><span class="sxs-lookup"><span data-stu-id="16287-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16287-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16287-123">Authorization</span></span>|<span data-ttu-id="16287-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16287-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16287-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16287-125">Accept</span></span>|<span data-ttu-id="16287-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16287-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16287-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16287-127">Request body</span></span>
<span data-ttu-id="16287-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="16287-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="16287-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="16287-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="16287-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16287-130">Property</span></span>|<span data-ttu-id="16287-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16287-131">Type</span></span>|<span data-ttu-id="16287-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16287-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16287-133">id</span><span class="sxs-lookup"><span data-stu-id="16287-133">id</span></span>|<span data-ttu-id="16287-134">String</span><span class="sxs-lookup"><span data-stu-id="16287-134">String</span></span>|<span data-ttu-id="16287-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16287-135">Key of the entity.</span></span> <span data-ttu-id="16287-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16287-137">lastModifiedDateTime</span></span>|<span data-ttu-id="16287-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16287-138">DateTimeOffset</span></span>|<span data-ttu-id="16287-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="16287-139">DateTime the object was last modified.</span></span> <span data-ttu-id="16287-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16287-141">roleScopeTagIds</span></span>|<span data-ttu-id="16287-142">String collection</span><span class="sxs-lookup"><span data-stu-id="16287-142">String collection</span></span>|<span data-ttu-id="16287-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="16287-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16287-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="16287-145">supportsScopeTags</span></span>|<span data-ttu-id="16287-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="16287-146">Boolean</span></span>|<span data-ttu-id="16287-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="16287-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16287-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="16287-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16287-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="16287-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16287-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16287-150">This property is read-only.</span></span> <span data-ttu-id="16287-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16287-152">createdDateTime</span></span>|<span data-ttu-id="16287-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16287-153">DateTimeOffset</span></span>|<span data-ttu-id="16287-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="16287-154">DateTime the object was created.</span></span> <span data-ttu-id="16287-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-156">description</span><span class="sxs-lookup"><span data-stu-id="16287-156">description</span></span>|<span data-ttu-id="16287-157">String</span><span class="sxs-lookup"><span data-stu-id="16287-157">String</span></span>|<span data-ttu-id="16287-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16287-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16287-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-160">displayName</span><span class="sxs-lookup"><span data-stu-id="16287-160">displayName</span></span>|<span data-ttu-id="16287-161">String</span><span class="sxs-lookup"><span data-stu-id="16287-161">String</span></span>|<span data-ttu-id="16287-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16287-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16287-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-164">version</span><span class="sxs-lookup"><span data-stu-id="16287-164">version</span></span>|<span data-ttu-id="16287-165">Int32</span><span class="sxs-lookup"><span data-stu-id="16287-165">Int32</span></span>|<span data-ttu-id="16287-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16287-166">Version of the device configuration.</span></span> <span data-ttu-id="16287-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16287-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16287-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="16287-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="16287-169">Int32</span><span class="sxs-lookup"><span data-stu-id="16287-169">Int32</span></span>|<span data-ttu-id="16287-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="16287-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="16287-171">Válido valores de 1 a 99 Inherited de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16287-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="16287-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="16287-172">subjectNameFormat</span></span>|[<span data-ttu-id="16287-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="16287-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="16287-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16287-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="16287-175">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="16287-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="16287-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="16287-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="16287-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="16287-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="16287-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="16287-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="16287-179">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16287-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="16287-180">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="16287-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="16287-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="16287-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="16287-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="16287-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="16287-183">Int32</span><span class="sxs-lookup"><span data-stu-id="16287-183">Int32</span></span>|<span data-ttu-id="16287-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16287-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="16287-185">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16287-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="16287-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="16287-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="16287-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="16287-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="16287-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="16287-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="16287-189">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="16287-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="16287-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="16287-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="16287-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="16287-191">scepServerUrls</span></span>|<span data-ttu-id="16287-192">String collection</span><span class="sxs-lookup"><span data-stu-id="16287-192">String collection</span></span>|<span data-ttu-id="16287-193">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="16287-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="16287-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="16287-194">subjectNameFormatString</span></span>|<span data-ttu-id="16287-195">String</span><span class="sxs-lookup"><span data-stu-id="16287-195">String</span></span>|<span data-ttu-id="16287-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="16287-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="16287-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="16287-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="16287-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="16287-198">keyUsage</span></span>|[<span data-ttu-id="16287-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="16287-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="16287-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="16287-200">SCEP Key Usage.</span></span> <span data-ttu-id="16287-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="16287-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="16287-202">keySize</span><span class="sxs-lookup"><span data-stu-id="16287-202">keySize</span></span>|[<span data-ttu-id="16287-203">keySize</span><span class="sxs-lookup"><span data-stu-id="16287-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="16287-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="16287-204">SCEP Key Size.</span></span> <span data-ttu-id="16287-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="16287-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="16287-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="16287-206">extendedKeyUsages</span></span>|<span data-ttu-id="16287-207">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="16287-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="16287-208">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="16287-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="16287-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="16287-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="16287-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="16287-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="16287-211">String</span><span class="sxs-lookup"><span data-stu-id="16287-211">String</span></span>|<span data-ttu-id="16287-212">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="16287-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="16287-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="16287-213">certificateStore</span></span>|[<span data-ttu-id="16287-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="16287-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="16287-215">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="16287-215">Target store certificate.</span></span> <span data-ttu-id="16287-216">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="16287-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="16287-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="16287-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="16287-218">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="16287-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="16287-219">Configurações de Alterantive nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="16287-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="16287-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="16287-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="16287-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="16287-221">Response</span></span>
<span data-ttu-id="16287-222">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16287-222">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16287-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16287-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="16287-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16287-224">Request</span></span>
<span data-ttu-id="16287-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16287-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="16287-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="16287-226">Response</span></span>
<span data-ttu-id="16287-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16287-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





