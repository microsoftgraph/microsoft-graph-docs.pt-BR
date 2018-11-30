---
title: Criar androidForWorkScepCertificateProfile
description: Crie um novo objeto de androidForWorkScepCertificateProfile.
ms.openlocfilehash: 8d780cb50ef7fc272bb34f4112f8adfe9b596ad0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034561"
---
# <a name="create-androidforworkscepcertificateprofile"></a><span data-ttu-id="fe439-103">Criar androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="fe439-103">Create androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="fe439-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe439-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe439-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe439-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe439-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fe439-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe439-107">Crie um novo objeto de [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fe439-107">Create a new [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe439-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe439-108">Prerequisites</span></span>
<span data-ttu-id="fe439-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe439-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe439-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe439-111">Permission type</span></span>|<span data-ttu-id="fe439-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe439-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe439-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe439-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe439-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe439-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe439-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe439-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe439-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe439-116">Not supported.</span></span>|
|<span data-ttu-id="fe439-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe439-117">Application</span></span>|<span data-ttu-id="fe439-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe439-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe439-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe439-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fe439-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe439-120">Request headers</span></span>
|<span data-ttu-id="fe439-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe439-121">Header</span></span>|<span data-ttu-id="fe439-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fe439-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe439-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe439-123">Authorization</span></span>|<span data-ttu-id="fe439-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe439-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe439-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe439-125">Accept</span></span>|<span data-ttu-id="fe439-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe439-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe439-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe439-127">Request body</span></span>
<span data-ttu-id="fe439-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="fe439-128">In the request body, supply a JSON representation for the androidForWorkScepCertificateProfile object.</span></span>

<span data-ttu-id="fe439-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="fe439-129">The following table shows the properties that are required when you create the androidForWorkScepCertificateProfile.</span></span>

|<span data-ttu-id="fe439-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe439-130">Property</span></span>|<span data-ttu-id="fe439-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe439-131">Type</span></span>|<span data-ttu-id="fe439-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe439-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe439-133">id</span><span class="sxs-lookup"><span data-stu-id="fe439-133">id</span></span>|<span data-ttu-id="fe439-134">String</span><span class="sxs-lookup"><span data-stu-id="fe439-134">String</span></span>|<span data-ttu-id="fe439-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe439-135">Key of the entity.</span></span> <span data-ttu-id="fe439-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe439-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fe439-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe439-138">DateTimeOffset</span></span>|<span data-ttu-id="fe439-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fe439-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fe439-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe439-141">roleScopeTagIds</span></span>|<span data-ttu-id="fe439-142">String collection</span><span class="sxs-lookup"><span data-stu-id="fe439-142">String collection</span></span>|<span data-ttu-id="fe439-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe439-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe439-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fe439-145">supportsScopeTags</span></span>|<span data-ttu-id="fe439-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="fe439-146">Boolean</span></span>|<span data-ttu-id="fe439-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="fe439-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe439-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="fe439-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe439-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="fe439-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe439-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fe439-150">This property is read-only.</span></span> <span data-ttu-id="fe439-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe439-152">createdDateTime</span></span>|<span data-ttu-id="fe439-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe439-153">DateTimeOffset</span></span>|<span data-ttu-id="fe439-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fe439-154">DateTime the object was created.</span></span> <span data-ttu-id="fe439-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-156">description</span><span class="sxs-lookup"><span data-stu-id="fe439-156">description</span></span>|<span data-ttu-id="fe439-157">String</span><span class="sxs-lookup"><span data-stu-id="fe439-157">String</span></span>|<span data-ttu-id="fe439-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe439-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe439-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fe439-160">displayName</span></span>|<span data-ttu-id="fe439-161">String</span><span class="sxs-lookup"><span data-stu-id="fe439-161">String</span></span>|<span data-ttu-id="fe439-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe439-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe439-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-164">version</span><span class="sxs-lookup"><span data-stu-id="fe439-164">version</span></span>|<span data-ttu-id="fe439-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fe439-165">Int32</span></span>|<span data-ttu-id="fe439-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe439-166">Version of the device configuration.</span></span> <span data-ttu-id="fe439-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe439-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="fe439-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="fe439-169">Int32</span><span class="sxs-lookup"><span data-stu-id="fe439-169">Int32</span></span>|<span data-ttu-id="fe439-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="fe439-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fe439-171">Válido valores de 1 a 99 Inherited de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fe439-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fe439-172">subjectNameFormat</span></span>|[<span data-ttu-id="fe439-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fe439-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="fe439-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fe439-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="fe439-175">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fe439-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="fe439-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="fe439-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="fe439-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fe439-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fe439-178">Int32</span><span class="sxs-lookup"><span data-stu-id="fe439-178">Int32</span></span>|<span data-ttu-id="fe439-179">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fe439-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="fe439-180">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fe439-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fe439-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fe439-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fe439-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fe439-183">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fe439-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="fe439-184">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fe439-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="fe439-185">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="fe439-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fe439-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="fe439-186">extendedKeyUsages</span></span>|<span data-ttu-id="fe439-187">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="fe439-188">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="fe439-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="fe439-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe439-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fe439-190">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fe439-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="fe439-191">scepServerUrls</span></span>|<span data-ttu-id="fe439-192">String collection</span><span class="sxs-lookup"><span data-stu-id="fe439-192">String collection</span></span>|<span data-ttu-id="fe439-193">URL de servidor SCEP (s)</span><span class="sxs-lookup"><span data-stu-id="fe439-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="fe439-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fe439-194">subjectNameFormatString</span></span>|<span data-ttu-id="fe439-195">String</span><span class="sxs-lookup"><span data-stu-id="fe439-195">String</span></span>|<span data-ttu-id="fe439-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="fe439-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="fe439-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="fe439-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="fe439-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="fe439-198">keyUsage</span></span>|[<span data-ttu-id="fe439-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="fe439-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="fe439-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="fe439-200">SCEP Key Usage.</span></span> <span data-ttu-id="fe439-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="fe439-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="fe439-202">keySize</span><span class="sxs-lookup"><span data-stu-id="fe439-202">keySize</span></span>|[<span data-ttu-id="fe439-203">keySize</span><span class="sxs-lookup"><span data-stu-id="fe439-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="fe439-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="fe439-204">SCEP Key Size.</span></span> <span data-ttu-id="fe439-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="fe439-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="fe439-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="fe439-206">hashAlgorithm</span></span>|[<span data-ttu-id="fe439-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="fe439-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="fe439-208">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="fe439-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="fe439-209">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="fe439-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="fe439-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fe439-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="fe439-211">String</span><span class="sxs-lookup"><span data-stu-id="fe439-211">String</span></span>|<span data-ttu-id="fe439-212">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="fe439-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="fe439-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fe439-213">certificateStore</span></span>|[<span data-ttu-id="fe439-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fe439-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="fe439-215">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="fe439-215">Target store certificate.</span></span> <span data-ttu-id="fe439-216">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="fe439-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="fe439-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="fe439-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="fe439-218">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="fe439-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="fe439-219">Configurações de Alterantive nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="fe439-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="fe439-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe439-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe439-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fe439-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fe439-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fe439-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fe439-223">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fe439-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="fe439-224">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="fe439-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="fe439-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe439-225">Response</span></span>
<span data-ttu-id="fe439-226">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe439-226">If successful, this method returns a `201 Created` response code and a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe439-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe439-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe439-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe439-228">Request</span></span>
<span data-ttu-id="fe439-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe439-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1269

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="fe439-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe439-230">Response</span></span>
<span data-ttu-id="fe439-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe439-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





