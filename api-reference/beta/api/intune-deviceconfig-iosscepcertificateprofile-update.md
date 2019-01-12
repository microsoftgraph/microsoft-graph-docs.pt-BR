---
title: Atualizar iosScepCertificateProfile
description: Atualize as propriedades de um objeto iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1cb0158eff965e2076d7a081d23c7eda793722a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914522"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="f2810-103">Atualizar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f2810-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="f2810-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2810-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2810-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2810-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2810-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f2810-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2810-107">Atualize as propriedades de um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f2810-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2810-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2810-108">Prerequisites</span></span>
<span data-ttu-id="f2810-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2810-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2810-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2810-111">Permission type</span></span>|<span data-ttu-id="f2810-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2810-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2810-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2810-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2810-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2810-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2810-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2810-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2810-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2810-116">Not supported.</span></span>|
|<span data-ttu-id="f2810-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2810-117">Application</span></span>|<span data-ttu-id="f2810-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2810-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2810-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2810-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f2810-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2810-120">Request headers</span></span>
|<span data-ttu-id="f2810-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2810-121">Header</span></span>|<span data-ttu-id="f2810-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2810-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2810-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2810-123">Authorization</span></span>|<span data-ttu-id="f2810-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2810-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2810-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2810-125">Accept</span></span>|<span data-ttu-id="f2810-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2810-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2810-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2810-127">Request body</span></span>
<span data-ttu-id="f2810-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f2810-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f2810-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f2810-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="f2810-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2810-130">Property</span></span>|<span data-ttu-id="f2810-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2810-131">Type</span></span>|<span data-ttu-id="f2810-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2810-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2810-133">id</span><span class="sxs-lookup"><span data-stu-id="f2810-133">id</span></span>|<span data-ttu-id="f2810-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2810-134">String</span></span>|<span data-ttu-id="f2810-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2810-135">Key of the entity.</span></span> <span data-ttu-id="f2810-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2810-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f2810-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2810-138">DateTimeOffset</span></span>|<span data-ttu-id="f2810-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f2810-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f2810-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2810-141">roleScopeTagIds</span></span>|<span data-ttu-id="f2810-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f2810-142">String collection</span></span>|<span data-ttu-id="f2810-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2810-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f2810-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f2810-145">supportsScopeTags</span></span>|<span data-ttu-id="f2810-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f2810-146">Boolean</span></span>|<span data-ttu-id="f2810-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f2810-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f2810-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f2810-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f2810-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f2810-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f2810-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2810-150">This property is read-only.</span></span> <span data-ttu-id="f2810-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2810-152">createdDateTime</span></span>|<span data-ttu-id="f2810-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2810-153">DateTimeOffset</span></span>|<span data-ttu-id="f2810-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f2810-154">DateTime the object was created.</span></span> <span data-ttu-id="f2810-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-156">description</span><span class="sxs-lookup"><span data-stu-id="f2810-156">description</span></span>|<span data-ttu-id="f2810-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2810-157">String</span></span>|<span data-ttu-id="f2810-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2810-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2810-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f2810-160">displayName</span></span>|<span data-ttu-id="f2810-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2810-161">String</span></span>|<span data-ttu-id="f2810-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2810-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2810-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-164">version</span><span class="sxs-lookup"><span data-stu-id="f2810-164">version</span></span>|<span data-ttu-id="f2810-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f2810-165">Int32</span></span>|<span data-ttu-id="f2810-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2810-166">Version of the device configuration.</span></span> <span data-ttu-id="f2810-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2810-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f2810-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="f2810-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f2810-169">Int32</span></span>|<span data-ttu-id="f2810-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="f2810-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f2810-171">Válido valores de 1 a 99 Inherited de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f2810-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f2810-172">subjectNameFormat</span></span>|[<span data-ttu-id="f2810-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f2810-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f2810-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f2810-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="f2810-175">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f2810-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f2810-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f2810-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f2810-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f2810-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f2810-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f2810-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f2810-179">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f2810-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="f2810-180">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f2810-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f2810-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f2810-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f2810-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f2810-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f2810-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f2810-183">Int32</span></span>|<span data-ttu-id="f2810-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f2810-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f2810-185">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f2810-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f2810-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f2810-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f2810-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f2810-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f2810-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f2810-189">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f2810-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f2810-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f2810-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f2810-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f2810-191">scepServerUrls</span></span>|<span data-ttu-id="f2810-192">String collection</span><span class="sxs-lookup"><span data-stu-id="f2810-192">String collection</span></span>|<span data-ttu-id="f2810-193">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="f2810-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f2810-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f2810-194">subjectNameFormatString</span></span>|<span data-ttu-id="f2810-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2810-195">String</span></span>|<span data-ttu-id="f2810-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="f2810-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f2810-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="f2810-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f2810-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="f2810-198">keyUsage</span></span>|[<span data-ttu-id="f2810-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f2810-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f2810-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="f2810-200">SCEP Key Usage.</span></span> <span data-ttu-id="f2810-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f2810-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f2810-202">keySize</span><span class="sxs-lookup"><span data-stu-id="f2810-202">keySize</span></span>|[<span data-ttu-id="f2810-203">keySize</span><span class="sxs-lookup"><span data-stu-id="f2810-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f2810-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="f2810-204">SCEP Key Size.</span></span> <span data-ttu-id="f2810-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="f2810-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f2810-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f2810-206">extendedKeyUsages</span></span>|<span data-ttu-id="f2810-207">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f2810-208">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="f2810-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f2810-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f2810-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f2810-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f2810-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f2810-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2810-211">String</span></span>|<span data-ttu-id="f2810-212">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="f2810-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f2810-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f2810-213">certificateStore</span></span>|[<span data-ttu-id="f2810-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f2810-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f2810-215">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="f2810-215">Target store certificate.</span></span> <span data-ttu-id="f2810-216">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="f2810-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f2810-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f2810-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f2810-218">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f2810-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f2810-219">Configurações de Alterantive nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="f2810-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="f2810-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f2810-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f2810-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2810-221">Response</span></span>
<span data-ttu-id="f2810-222">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2810-222">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2810-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2810-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2810-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2810-224">Request</span></span>
<span data-ttu-id="f2810-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2810-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2810-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2810-226">Response</span></span>
<span data-ttu-id="f2810-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2810-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





