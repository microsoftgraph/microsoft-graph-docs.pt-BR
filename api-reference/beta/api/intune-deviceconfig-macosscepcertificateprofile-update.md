---
title: Atualizar macOSScepCertificateProfile
description: Atualize as propriedades de um objeto macOSScepCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 547a4468015a68bcbdb8bbfe13839f98edd6d9d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412202"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="23061-103">Atualizar macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="23061-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="23061-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="23061-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23061-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="23061-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23061-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="23061-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23061-107">Atualize as propriedades de um objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="23061-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23061-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23061-108">Prerequisites</span></span>
<span data-ttu-id="23061-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="23061-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23061-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23061-111">Permission type</span></span>|<span data-ttu-id="23061-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23061-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23061-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23061-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23061-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23061-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23061-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23061-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23061-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23061-116">Not supported.</span></span>|
|<span data-ttu-id="23061-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23061-117">Application</span></span>|<span data-ttu-id="23061-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23061-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23061-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23061-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="23061-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23061-120">Request headers</span></span>
|<span data-ttu-id="23061-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23061-121">Header</span></span>|<span data-ttu-id="23061-122">Valor</span><span class="sxs-lookup"><span data-stu-id="23061-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23061-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23061-123">Authorization</span></span>|<span data-ttu-id="23061-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23061-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23061-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23061-125">Accept</span></span>|<span data-ttu-id="23061-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23061-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23061-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23061-127">Request body</span></span>
<span data-ttu-id="23061-128">No corpo da solicitação, fornece uma representação JSON para o objeto [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="23061-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="23061-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="23061-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="23061-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23061-130">Property</span></span>|<span data-ttu-id="23061-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="23061-131">Type</span></span>|<span data-ttu-id="23061-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="23061-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23061-133">id</span><span class="sxs-lookup"><span data-stu-id="23061-133">id</span></span>|<span data-ttu-id="23061-134">String</span><span class="sxs-lookup"><span data-stu-id="23061-134">String</span></span>|<span data-ttu-id="23061-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23061-135">Key of the entity.</span></span> <span data-ttu-id="23061-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23061-137">lastModifiedDateTime</span></span>|<span data-ttu-id="23061-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23061-138">DateTimeOffset</span></span>|<span data-ttu-id="23061-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="23061-139">DateTime the object was last modified.</span></span> <span data-ttu-id="23061-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23061-141">roleScopeTagIds</span></span>|<span data-ttu-id="23061-142">String collection</span><span class="sxs-lookup"><span data-stu-id="23061-142">String collection</span></span>|<span data-ttu-id="23061-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="23061-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23061-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23061-145">supportsScopeTags</span></span>|<span data-ttu-id="23061-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="23061-146">Boolean</span></span>|<span data-ttu-id="23061-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="23061-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23061-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="23061-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23061-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="23061-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23061-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23061-150">This property is read-only.</span></span> <span data-ttu-id="23061-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23061-152">createdDateTime</span></span>|<span data-ttu-id="23061-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23061-153">DateTimeOffset</span></span>|<span data-ttu-id="23061-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="23061-154">DateTime the object was created.</span></span> <span data-ttu-id="23061-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-156">description</span><span class="sxs-lookup"><span data-stu-id="23061-156">description</span></span>|<span data-ttu-id="23061-157">String</span><span class="sxs-lookup"><span data-stu-id="23061-157">String</span></span>|<span data-ttu-id="23061-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23061-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23061-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-160">displayName</span><span class="sxs-lookup"><span data-stu-id="23061-160">displayName</span></span>|<span data-ttu-id="23061-161">String</span><span class="sxs-lookup"><span data-stu-id="23061-161">String</span></span>|<span data-ttu-id="23061-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23061-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23061-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-164">version</span><span class="sxs-lookup"><span data-stu-id="23061-164">version</span></span>|<span data-ttu-id="23061-165">Int32</span><span class="sxs-lookup"><span data-stu-id="23061-165">Int32</span></span>|<span data-ttu-id="23061-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23061-166">Version of the device configuration.</span></span> <span data-ttu-id="23061-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23061-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23061-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="23061-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="23061-169">Int32</span><span class="sxs-lookup"><span data-stu-id="23061-169">Int32</span></span>|<span data-ttu-id="23061-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="23061-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="23061-171">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="23061-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="23061-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="23061-172">subjectNameFormat</span></span>|[<span data-ttu-id="23061-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="23061-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="23061-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="23061-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="23061-175">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="23061-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="23061-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="23061-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="23061-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="23061-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="23061-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="23061-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="23061-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="23061-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="23061-180">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="23061-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="23061-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="23061-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="23061-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="23061-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="23061-183">Int32</span><span class="sxs-lookup"><span data-stu-id="23061-183">Int32</span></span>|<span data-ttu-id="23061-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="23061-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="23061-185">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="23061-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="23061-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="23061-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="23061-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="23061-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="23061-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="23061-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="23061-189">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="23061-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="23061-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="23061-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="23061-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="23061-191">scepServerUrls</span></span>|<span data-ttu-id="23061-192">String collection</span><span class="sxs-lookup"><span data-stu-id="23061-192">String collection</span></span>|<span data-ttu-id="23061-193">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="23061-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="23061-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="23061-194">subjectNameFormatString</span></span>|<span data-ttu-id="23061-195">String</span><span class="sxs-lookup"><span data-stu-id="23061-195">String</span></span>|<span data-ttu-id="23061-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="23061-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="23061-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="23061-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="23061-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="23061-198">keyUsage</span></span>|[<span data-ttu-id="23061-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="23061-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="23061-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="23061-200">SCEP Key Usage.</span></span> <span data-ttu-id="23061-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="23061-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="23061-202">keySize</span><span class="sxs-lookup"><span data-stu-id="23061-202">keySize</span></span>|[<span data-ttu-id="23061-203">keySize</span><span class="sxs-lookup"><span data-stu-id="23061-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="23061-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="23061-204">SCEP Key Size.</span></span> <span data-ttu-id="23061-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="23061-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="23061-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="23061-206">hashAlgorithm</span></span>|[<span data-ttu-id="23061-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="23061-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="23061-208">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="23061-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="23061-209">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="23061-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="23061-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="23061-210">extendedKeyUsages</span></span>|<span data-ttu-id="23061-211">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="23061-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="23061-212">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="23061-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="23061-213">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="23061-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="23061-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="23061-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="23061-215">String</span><span class="sxs-lookup"><span data-stu-id="23061-215">String</span></span>|<span data-ttu-id="23061-216">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="23061-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="23061-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="23061-217">certificateStore</span></span>|[<span data-ttu-id="23061-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="23061-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="23061-219">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="23061-219">Target store certificate.</span></span> <span data-ttu-id="23061-220">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="23061-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="23061-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="23061-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="23061-222">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="23061-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="23061-223">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="23061-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="23061-224">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="23061-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="23061-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="23061-225">Response</span></span>
<span data-ttu-id="23061-226">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23061-226">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23061-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23061-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="23061-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23061-228">Request</span></span>
<span data-ttu-id="23061-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23061-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="23061-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="23061-230">Response</span></span>
<span data-ttu-id="23061-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23061-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

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




