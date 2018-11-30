---
title: Atualizar windows10PkcsCertificateProfile
description: Atualize as propriedades de um objeto windows10PkcsCertificateProfile.
ms.openlocfilehash: 710b4b2abac6a4e4818e3a9f7024e3ced669e541
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036107"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="b91f5-103">Atualizar windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b91f5-103">Update windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="b91f5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b91f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b91f5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b91f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b91f5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b91f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b91f5-107">Atualize as propriedades de um objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b91f5-107">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b91f5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b91f5-108">Prerequisites</span></span>
<span data-ttu-id="b91f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b91f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b91f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b91f5-111">Permission type</span></span>|<span data-ttu-id="b91f5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b91f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b91f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b91f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b91f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b91f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b91f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b91f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b91f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b91f5-116">Not supported.</span></span>|
|<span data-ttu-id="b91f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b91f5-117">Application</span></span>|<span data-ttu-id="b91f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b91f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b91f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b91f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b91f5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b91f5-120">Request headers</span></span>
|<span data-ttu-id="b91f5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b91f5-121">Header</span></span>|<span data-ttu-id="b91f5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b91f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b91f5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b91f5-123">Authorization</span></span>|<span data-ttu-id="b91f5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b91f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b91f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b91f5-125">Accept</span></span>|<span data-ttu-id="b91f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b91f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b91f5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b91f5-127">Request body</span></span>
<span data-ttu-id="b91f5-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b91f5-128">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="b91f5-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b91f5-129">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="b91f5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b91f5-130">Property</span></span>|<span data-ttu-id="b91f5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b91f5-131">Type</span></span>|<span data-ttu-id="b91f5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b91f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b91f5-133">id</span><span class="sxs-lookup"><span data-stu-id="b91f5-133">id</span></span>|<span data-ttu-id="b91f5-134">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-134">String</span></span>|<span data-ttu-id="b91f5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b91f5-135">Key of the entity.</span></span> <span data-ttu-id="b91f5-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b91f5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b91f5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b91f5-138">DateTimeOffset</span></span>|<span data-ttu-id="b91f5-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b91f5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b91f5-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b91f5-141">roleScopeTagIds</span></span>|<span data-ttu-id="b91f5-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b91f5-142">String collection</span></span>|<span data-ttu-id="b91f5-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b91f5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b91f5-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b91f5-145">supportsScopeTags</span></span>|<span data-ttu-id="b91f5-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b91f5-146">Boolean</span></span>|<span data-ttu-id="b91f5-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b91f5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b91f5-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b91f5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b91f5-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b91f5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b91f5-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b91f5-150">This property is read-only.</span></span> <span data-ttu-id="b91f5-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b91f5-152">createdDateTime</span></span>|<span data-ttu-id="b91f5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b91f5-153">DateTimeOffset</span></span>|<span data-ttu-id="b91f5-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b91f5-154">DateTime the object was created.</span></span> <span data-ttu-id="b91f5-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-156">description</span><span class="sxs-lookup"><span data-stu-id="b91f5-156">description</span></span>|<span data-ttu-id="b91f5-157">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-157">String</span></span>|<span data-ttu-id="b91f5-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b91f5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b91f5-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b91f5-160">displayName</span></span>|<span data-ttu-id="b91f5-161">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-161">String</span></span>|<span data-ttu-id="b91f5-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b91f5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b91f5-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-164">version</span><span class="sxs-lookup"><span data-stu-id="b91f5-164">version</span></span>|<span data-ttu-id="b91f5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b91f5-165">Int32</span></span>|<span data-ttu-id="b91f5-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b91f5-166">Version of the device configuration.</span></span> <span data-ttu-id="b91f5-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91f5-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b91f5-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b91f5-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b91f5-169">Int32</span></span>|<span data-ttu-id="b91f5-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="b91f5-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b91f5-171">Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b91f5-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="b91f5-172">keyStorageProvider</span></span>|[<span data-ttu-id="b91f5-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="b91f5-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="b91f5-174">Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b91f5-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b91f5-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="b91f5-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="b91f5-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b91f5-176">subjectNameFormat</span></span>|[<span data-ttu-id="b91f5-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b91f5-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b91f5-178">Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b91f5-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b91f5-179">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b91f5-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b91f5-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b91f5-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b91f5-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b91f5-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b91f5-182">Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b91f5-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b91f5-183">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b91f5-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b91f5-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b91f5-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b91f5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b91f5-185">Int32</span></span>|<span data-ttu-id="b91f5-186">Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b91f5-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b91f5-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b91f5-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b91f5-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b91f5-189">Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b91f5-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b91f5-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b91f5-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b91f5-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="b91f5-191">certificationAuthority</span></span>|<span data-ttu-id="b91f5-192">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-192">String</span></span>|<span data-ttu-id="b91f5-193">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="b91f5-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="b91f5-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="b91f5-194">certificationAuthorityName</span></span>|<span data-ttu-id="b91f5-195">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-195">String</span></span>|<span data-ttu-id="b91f5-196">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="b91f5-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="b91f5-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="b91f5-197">certificateTemplateName</span></span>|<span data-ttu-id="b91f5-198">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-198">String</span></span>|<span data-ttu-id="b91f5-199">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="b91f5-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="b91f5-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b91f5-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b91f5-201">String</span><span class="sxs-lookup"><span data-stu-id="b91f5-201">String</span></span>|<span data-ttu-id="b91f5-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="b91f5-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b91f5-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b91f5-203">extendedKeyUsages</span></span>|<span data-ttu-id="b91f5-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b91f5-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b91f5-205">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="b91f5-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b91f5-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b91f5-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b91f5-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="b91f5-207">Response</span></span>
<span data-ttu-id="b91f5-208">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b91f5-208">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b91f5-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b91f5-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="b91f5-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b91f5-210">Request</span></span>
<span data-ttu-id="b91f5-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b91f5-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1005

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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b91f5-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="b91f5-212">Response</span></span>
<span data-ttu-id="b91f5-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b91f5-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1183

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```





