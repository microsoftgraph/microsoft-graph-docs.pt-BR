---
title: Criar androidScepCertificateProfile
description: Crie um novo objeto de androidScepCertificateProfile.
ms.openlocfilehash: fbea937e508cb17570142c5c0b5ab603aba38541
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039786"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="b4236-103">Criar androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b4236-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="b4236-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4236-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4236-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4236-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4236-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4236-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4236-107">Crie um novo objeto de [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b4236-107">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4236-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4236-108">Prerequisites</span></span>
<span data-ttu-id="b4236-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4236-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4236-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4236-111">Permission type</span></span>|<span data-ttu-id="b4236-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4236-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4236-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4236-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4236-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4236-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4236-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4236-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4236-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4236-116">Not supported.</span></span>|
|<span data-ttu-id="b4236-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4236-117">Application</span></span>|<span data-ttu-id="b4236-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4236-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4236-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4236-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4236-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4236-120">Request headers</span></span>
|<span data-ttu-id="b4236-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4236-121">Header</span></span>|<span data-ttu-id="b4236-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4236-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4236-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4236-123">Authorization</span></span>|<span data-ttu-id="b4236-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4236-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4236-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4236-125">Accept</span></span>|<span data-ttu-id="b4236-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4236-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4236-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4236-127">Request body</span></span>
<span data-ttu-id="b4236-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b4236-128">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="b4236-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b4236-129">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="b4236-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4236-130">Property</span></span>|<span data-ttu-id="b4236-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4236-131">Type</span></span>|<span data-ttu-id="b4236-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4236-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4236-133">id</span><span class="sxs-lookup"><span data-stu-id="b4236-133">id</span></span>|<span data-ttu-id="b4236-134">String</span><span class="sxs-lookup"><span data-stu-id="b4236-134">String</span></span>|<span data-ttu-id="b4236-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4236-135">Key of the entity.</span></span> <span data-ttu-id="b4236-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4236-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b4236-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4236-138">DateTimeOffset</span></span>|<span data-ttu-id="b4236-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b4236-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b4236-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4236-141">roleScopeTagIds</span></span>|<span data-ttu-id="b4236-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b4236-142">String collection</span></span>|<span data-ttu-id="b4236-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4236-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b4236-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b4236-145">supportsScopeTags</span></span>|<span data-ttu-id="b4236-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4236-146">Boolean</span></span>|<span data-ttu-id="b4236-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b4236-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b4236-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b4236-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b4236-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b4236-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b4236-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4236-150">This property is read-only.</span></span> <span data-ttu-id="b4236-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4236-152">createdDateTime</span></span>|<span data-ttu-id="b4236-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4236-153">DateTimeOffset</span></span>|<span data-ttu-id="b4236-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b4236-154">DateTime the object was created.</span></span> <span data-ttu-id="b4236-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-156">description</span><span class="sxs-lookup"><span data-stu-id="b4236-156">description</span></span>|<span data-ttu-id="b4236-157">String</span><span class="sxs-lookup"><span data-stu-id="b4236-157">String</span></span>|<span data-ttu-id="b4236-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4236-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4236-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b4236-160">displayName</span></span>|<span data-ttu-id="b4236-161">String</span><span class="sxs-lookup"><span data-stu-id="b4236-161">String</span></span>|<span data-ttu-id="b4236-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4236-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4236-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-164">version</span><span class="sxs-lookup"><span data-stu-id="b4236-164">version</span></span>|<span data-ttu-id="b4236-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b4236-165">Int32</span></span>|<span data-ttu-id="b4236-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4236-166">Version of the device configuration.</span></span> <span data-ttu-id="b4236-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4236-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b4236-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b4236-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b4236-169">Int32</span></span>|<span data-ttu-id="b4236-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="b4236-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b4236-171">Válido valores de 1 a 99 Inherited de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4236-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b4236-172">subjectNameFormat</span></span>|[<span data-ttu-id="b4236-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b4236-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b4236-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4236-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="b4236-175">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4236-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b4236-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b4236-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b4236-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b4236-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b4236-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b4236-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b4236-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4236-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b4236-180">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4236-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b4236-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b4236-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b4236-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b4236-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b4236-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b4236-183">Int32</span></span>|<span data-ttu-id="b4236-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4236-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b4236-185">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4236-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b4236-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b4236-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b4236-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b4236-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4236-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b4236-189">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4236-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b4236-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b4236-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b4236-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b4236-191">extendedKeyUsages</span></span>|<span data-ttu-id="b4236-192">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b4236-193">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="b4236-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b4236-194">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b4236-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b4236-195">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4236-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4236-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="b4236-196">scepServerUrls</span></span>|<span data-ttu-id="b4236-197">String collection</span><span class="sxs-lookup"><span data-stu-id="b4236-197">String collection</span></span>|<span data-ttu-id="b4236-198">URL de servidor SCEP (s)</span><span class="sxs-lookup"><span data-stu-id="b4236-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="b4236-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b4236-199">subjectNameFormatString</span></span>|<span data-ttu-id="b4236-200">String</span><span class="sxs-lookup"><span data-stu-id="b4236-200">String</span></span>|<span data-ttu-id="b4236-201">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="b4236-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b4236-202">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="b4236-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b4236-203">keyUsage</span><span class="sxs-lookup"><span data-stu-id="b4236-203">keyUsage</span></span>|[<span data-ttu-id="b4236-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="b4236-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b4236-205">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="b4236-205">SCEP Key Usage.</span></span> <span data-ttu-id="b4236-206">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="b4236-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b4236-207">keySize</span><span class="sxs-lookup"><span data-stu-id="b4236-207">keySize</span></span>|[<span data-ttu-id="b4236-208">keySize</span><span class="sxs-lookup"><span data-stu-id="b4236-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="b4236-209">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="b4236-209">SCEP Key Size.</span></span> <span data-ttu-id="b4236-210">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="b4236-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="b4236-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b4236-211">hashAlgorithm</span></span>|[<span data-ttu-id="b4236-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="b4236-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="b4236-213">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="b4236-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="b4236-214">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="b4236-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="b4236-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b4236-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b4236-216">String</span><span class="sxs-lookup"><span data-stu-id="b4236-216">String</span></span>|<span data-ttu-id="b4236-217">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="b4236-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="b4236-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4236-218">Response</span></span>
<span data-ttu-id="b4236-219">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4236-219">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4236-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4236-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4236-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4236-221">Request</span></span>
<span data-ttu-id="b4236-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4236-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1038

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="b4236-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4236-223">Response</span></span>
<span data-ttu-id="b4236-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4236-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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





