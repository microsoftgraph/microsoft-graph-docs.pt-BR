---
title: Atualizar macOSScepCertificateProfile
description: Atualize as propriedades de um objeto macOSScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e654208e006b04c846721fe2cd3446183553902
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968019"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="84a5e-103">Atualizar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="84a5e-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="84a5e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84a5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84a5e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84a5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84a5e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84a5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84a5e-107">Atualize as propriedades de um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="84a5e-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84a5e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84a5e-108">Prerequisites</span></span>
<span data-ttu-id="84a5e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84a5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84a5e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84a5e-111">Permission type</span></span>|<span data-ttu-id="84a5e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84a5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84a5e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84a5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84a5e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a5e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84a5e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84a5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84a5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a5e-116">Not supported.</span></span>|
|<span data-ttu-id="84a5e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84a5e-117">Application</span></span>|<span data-ttu-id="84a5e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a5e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84a5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84a5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="84a5e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84a5e-120">Request headers</span></span>
|<span data-ttu-id="84a5e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84a5e-121">Header</span></span>|<span data-ttu-id="84a5e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84a5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84a5e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84a5e-123">Authorization</span></span>|<span data-ttu-id="84a5e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84a5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84a5e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84a5e-125">Accept</span></span>|<span data-ttu-id="84a5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84a5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84a5e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84a5e-127">Request body</span></span>
<span data-ttu-id="84a5e-128">No corpo da solicitação, fornece uma representação JSON para o objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="84a5e-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="84a5e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="84a5e-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="84a5e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84a5e-130">Property</span></span>|<span data-ttu-id="84a5e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84a5e-131">Type</span></span>|<span data-ttu-id="84a5e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a5e-133">id</span><span class="sxs-lookup"><span data-stu-id="84a5e-133">id</span></span>|<span data-ttu-id="84a5e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a5e-134">String</span></span>|<span data-ttu-id="84a5e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84a5e-135">Key of the entity.</span></span> <span data-ttu-id="84a5e-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84a5e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="84a5e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a5e-138">DateTimeOffset</span></span>|<span data-ttu-id="84a5e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="84a5e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="84a5e-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84a5e-141">roleScopeTagIds</span></span>|<span data-ttu-id="84a5e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="84a5e-142">String collection</span></span>|<span data-ttu-id="84a5e-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="84a5e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84a5e-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84a5e-145">supportsScopeTags</span></span>|<span data-ttu-id="84a5e-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a5e-146">Boolean</span></span>|<span data-ttu-id="84a5e-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="84a5e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84a5e-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="84a5e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84a5e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="84a5e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84a5e-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84a5e-150">This property is read-only.</span></span> <span data-ttu-id="84a5e-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84a5e-152">createdDateTime</span></span>|<span data-ttu-id="84a5e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a5e-153">DateTimeOffset</span></span>|<span data-ttu-id="84a5e-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="84a5e-154">DateTime the object was created.</span></span> <span data-ttu-id="84a5e-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-156">description</span><span class="sxs-lookup"><span data-stu-id="84a5e-156">description</span></span>|<span data-ttu-id="84a5e-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a5e-157">String</span></span>|<span data-ttu-id="84a5e-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84a5e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84a5e-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="84a5e-160">displayName</span></span>|<span data-ttu-id="84a5e-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a5e-161">String</span></span>|<span data-ttu-id="84a5e-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84a5e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84a5e-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-164">version</span><span class="sxs-lookup"><span data-stu-id="84a5e-164">version</span></span>|<span data-ttu-id="84a5e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84a5e-165">Int32</span></span>|<span data-ttu-id="84a5e-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84a5e-166">Version of the device configuration.</span></span> <span data-ttu-id="84a5e-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a5e-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="84a5e-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="84a5e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="84a5e-169">Int32</span></span>|<span data-ttu-id="84a5e-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="84a5e-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="84a5e-171">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="84a5e-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="84a5e-172">subjectNameFormat</span></span>|[<span data-ttu-id="84a5e-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="84a5e-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="84a5e-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="84a5e-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="84a5e-175">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84a5e-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="84a5e-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="84a5e-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="84a5e-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="84a5e-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="84a5e-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="84a5e-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="84a5e-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="84a5e-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="84a5e-180">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84a5e-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="84a5e-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="84a5e-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="84a5e-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="84a5e-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="84a5e-183">Int32</span><span class="sxs-lookup"><span data-stu-id="84a5e-183">Int32</span></span>|<span data-ttu-id="84a5e-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="84a5e-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="84a5e-185">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="84a5e-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="84a5e-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="84a5e-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="84a5e-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="84a5e-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="84a5e-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="84a5e-189">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84a5e-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="84a5e-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="84a5e-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="84a5e-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="84a5e-191">scepServerUrls</span></span>|<span data-ttu-id="84a5e-192">String collection</span><span class="sxs-lookup"><span data-stu-id="84a5e-192">String collection</span></span>|<span data-ttu-id="84a5e-193">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="84a5e-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="84a5e-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="84a5e-194">subjectNameFormatString</span></span>|<span data-ttu-id="84a5e-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a5e-195">String</span></span>|<span data-ttu-id="84a5e-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="84a5e-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="84a5e-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="84a5e-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="84a5e-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="84a5e-198">keyUsage</span></span>|[<span data-ttu-id="84a5e-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="84a5e-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="84a5e-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="84a5e-200">SCEP Key Usage.</span></span> <span data-ttu-id="84a5e-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="84a5e-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="84a5e-202">keySize</span><span class="sxs-lookup"><span data-stu-id="84a5e-202">keySize</span></span>|[<span data-ttu-id="84a5e-203">keySize</span><span class="sxs-lookup"><span data-stu-id="84a5e-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="84a5e-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="84a5e-204">SCEP Key Size.</span></span> <span data-ttu-id="84a5e-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="84a5e-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="84a5e-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="84a5e-206">hashAlgorithm</span></span>|[<span data-ttu-id="84a5e-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="84a5e-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="84a5e-208">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="84a5e-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="84a5e-209">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="84a5e-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="84a5e-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="84a5e-210">extendedKeyUsages</span></span>|<span data-ttu-id="84a5e-211">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="84a5e-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="84a5e-212">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="84a5e-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="84a5e-213">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="84a5e-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="84a5e-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="84a5e-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="84a5e-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a5e-215">String</span></span>|<span data-ttu-id="84a5e-216">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="84a5e-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="84a5e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a5e-217">Response</span></span>
<span data-ttu-id="84a5e-218">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84a5e-218">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84a5e-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84a5e-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="84a5e-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84a5e-220">Request</span></span>
<span data-ttu-id="84a5e-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84a5e-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 963

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
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="84a5e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a5e-222">Response</span></span>
<span data-ttu-id="84a5e-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84a5e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





