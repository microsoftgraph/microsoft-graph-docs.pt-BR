---
title: Atualizar iosScepCertificateProfile
description: Atualize as propriedades de um objeto iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5f8ee6b856e2b8351059cd47de7bf8e9d2dddfd5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887196"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="4918b-103">Atualizar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4918b-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="4918b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4918b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4918b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4918b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4918b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4918b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4918b-107">Atualize as propriedades de um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4918b-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4918b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4918b-108">Prerequisites</span></span>
<span data-ttu-id="4918b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4918b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4918b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4918b-111">Permission type</span></span>|<span data-ttu-id="4918b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4918b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4918b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4918b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4918b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4918b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4918b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4918b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4918b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4918b-116">Not supported.</span></span>|
|<span data-ttu-id="4918b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4918b-117">Application</span></span>|<span data-ttu-id="4918b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4918b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4918b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4918b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4918b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4918b-120">Request headers</span></span>
|<span data-ttu-id="4918b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4918b-121">Header</span></span>|<span data-ttu-id="4918b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4918b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4918b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4918b-123">Authorization</span></span>|<span data-ttu-id="4918b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4918b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4918b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4918b-125">Accept</span></span>|<span data-ttu-id="4918b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4918b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4918b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4918b-127">Request body</span></span>
<span data-ttu-id="4918b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4918b-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="4918b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4918b-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="4918b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4918b-130">Property</span></span>|<span data-ttu-id="4918b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4918b-131">Type</span></span>|<span data-ttu-id="4918b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4918b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4918b-133">id</span><span class="sxs-lookup"><span data-stu-id="4918b-133">id</span></span>|<span data-ttu-id="4918b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4918b-134">String</span></span>|<span data-ttu-id="4918b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4918b-135">Key of the entity.</span></span> <span data-ttu-id="4918b-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4918b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4918b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4918b-138">DateTimeOffset</span></span>|<span data-ttu-id="4918b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4918b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4918b-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4918b-141">roleScopeTagIds</span></span>|<span data-ttu-id="4918b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4918b-142">String collection</span></span>|<span data-ttu-id="4918b-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="4918b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4918b-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4918b-145">supportsScopeTags</span></span>|<span data-ttu-id="4918b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="4918b-146">Boolean</span></span>|<span data-ttu-id="4918b-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4918b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4918b-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4918b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4918b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="4918b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4918b-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4918b-150">This property is read-only.</span></span> <span data-ttu-id="4918b-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4918b-152">createdDateTime</span></span>|<span data-ttu-id="4918b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4918b-153">DateTimeOffset</span></span>|<span data-ttu-id="4918b-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4918b-154">DateTime the object was created.</span></span> <span data-ttu-id="4918b-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-156">description</span><span class="sxs-lookup"><span data-stu-id="4918b-156">description</span></span>|<span data-ttu-id="4918b-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4918b-157">String</span></span>|<span data-ttu-id="4918b-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4918b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4918b-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4918b-160">displayName</span></span>|<span data-ttu-id="4918b-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4918b-161">String</span></span>|<span data-ttu-id="4918b-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4918b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4918b-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-164">version</span><span class="sxs-lookup"><span data-stu-id="4918b-164">version</span></span>|<span data-ttu-id="4918b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4918b-165">Int32</span></span>|<span data-ttu-id="4918b-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4918b-166">Version of the device configuration.</span></span> <span data-ttu-id="4918b-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4918b-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="4918b-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="4918b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="4918b-169">Int32</span></span>|<span data-ttu-id="4918b-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="4918b-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4918b-171">Válido valores de 1 a 99 Inherited de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4918b-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4918b-172">subjectNameFormat</span></span>|[<span data-ttu-id="4918b-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4918b-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="4918b-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4918b-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="4918b-175">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4918b-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="4918b-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="4918b-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="4918b-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4918b-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4918b-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4918b-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="4918b-179">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4918b-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="4918b-180">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4918b-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="4918b-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="4918b-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="4918b-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4918b-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4918b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="4918b-183">Int32</span></span>|<span data-ttu-id="4918b-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4918b-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="4918b-185">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4918b-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4918b-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4918b-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4918b-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="4918b-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4918b-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="4918b-189">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4918b-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="4918b-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="4918b-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4918b-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="4918b-191">scepServerUrls</span></span>|<span data-ttu-id="4918b-192">String collection</span><span class="sxs-lookup"><span data-stu-id="4918b-192">String collection</span></span>|<span data-ttu-id="4918b-193">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="4918b-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="4918b-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4918b-194">subjectNameFormatString</span></span>|<span data-ttu-id="4918b-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4918b-195">String</span></span>|<span data-ttu-id="4918b-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="4918b-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="4918b-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="4918b-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="4918b-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="4918b-198">keyUsage</span></span>|[<span data-ttu-id="4918b-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="4918b-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="4918b-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="4918b-200">SCEP Key Usage.</span></span> <span data-ttu-id="4918b-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="4918b-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="4918b-202">keySize</span><span class="sxs-lookup"><span data-stu-id="4918b-202">keySize</span></span>|[<span data-ttu-id="4918b-203">keySize</span><span class="sxs-lookup"><span data-stu-id="4918b-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="4918b-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="4918b-204">SCEP Key Size.</span></span> <span data-ttu-id="4918b-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="4918b-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="4918b-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="4918b-206">extendedKeyUsages</span></span>|<span data-ttu-id="4918b-207">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="4918b-208">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="4918b-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="4918b-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4918b-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4918b-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4918b-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4918b-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4918b-211">String</span></span>|<span data-ttu-id="4918b-212">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="4918b-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="4918b-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4918b-213">certificateStore</span></span>|[<span data-ttu-id="4918b-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4918b-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="4918b-215">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="4918b-215">Target store certificate.</span></span> <span data-ttu-id="4918b-216">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="4918b-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="4918b-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="4918b-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="4918b-218">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="4918b-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="4918b-219">Configurações de Alterantive nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="4918b-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="4918b-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4918b-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4918b-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="4918b-221">Response</span></span>
<span data-ttu-id="4918b-222">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4918b-222">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4918b-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4918b-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="4918b-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4918b-224">Request</span></span>
<span data-ttu-id="4918b-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4918b-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

{
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

### <a name="response"></a><span data-ttu-id="4918b-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="4918b-226">Response</span></span>
<span data-ttu-id="4918b-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4918b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





