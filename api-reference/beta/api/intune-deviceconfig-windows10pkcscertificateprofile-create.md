---
title: Criar windows10PkcsCertificateProfile
description: Crie um novo objeto de windows10PkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: baa12b444c52dd78b8d92944b9296a1a25e38f6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416430"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="0d2f2-103">Criar windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0d2f2-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="0d2f2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d2f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d2f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d2f2-107">Crie um novo objeto de [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0d2f2-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d2f2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d2f2-108">Prerequisites</span></span>
<span data-ttu-id="0d2f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d2f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d2f2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d2f2-111">Permission type</span></span>|<span data-ttu-id="0d2f2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d2f2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d2f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d2f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d2f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-116">Not supported.</span></span>|
|<span data-ttu-id="0d2f2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d2f2-117">Application</span></span>|<span data-ttu-id="0d2f2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d2f2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d2f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0d2f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d2f2-120">Request headers</span></span>
|<span data-ttu-id="0d2f2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d2f2-121">Header</span></span>|<span data-ttu-id="0d2f2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d2f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d2f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d2f2-123">Authorization</span></span>|<span data-ttu-id="0d2f2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d2f2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d2f2-125">Accept</span></span>|<span data-ttu-id="0d2f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d2f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d2f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d2f2-127">Request body</span></span>
<span data-ttu-id="0d2f2-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="0d2f2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="0d2f2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d2f2-130">Property</span></span>|<span data-ttu-id="0d2f2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d2f2-131">Type</span></span>|<span data-ttu-id="0d2f2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d2f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d2f2-133">id</span><span class="sxs-lookup"><span data-stu-id="0d2f2-133">id</span></span>|<span data-ttu-id="0d2f2-134">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-134">String</span></span>|<span data-ttu-id="0d2f2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-135">Key of the entity.</span></span> <span data-ttu-id="0d2f2-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d2f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0d2f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d2f2-138">DateTimeOffset</span></span>|<span data-ttu-id="0d2f2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0d2f2-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d2f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="0d2f2-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0d2f2-142">String collection</span></span>|<span data-ttu-id="0d2f2-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0d2f2-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0d2f2-145">supportsScopeTags</span></span>|<span data-ttu-id="0d2f2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d2f2-146">Boolean</span></span>|<span data-ttu-id="0d2f2-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0d2f2-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0d2f2-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0d2f2-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-150">This property is read-only.</span></span> <span data-ttu-id="0d2f2-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d2f2-152">createdDateTime</span></span>|<span data-ttu-id="0d2f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d2f2-153">DateTimeOffset</span></span>|<span data-ttu-id="0d2f2-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-154">DateTime the object was created.</span></span> <span data-ttu-id="0d2f2-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-156">description</span><span class="sxs-lookup"><span data-stu-id="0d2f2-156">description</span></span>|<span data-ttu-id="0d2f2-157">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-157">String</span></span>|<span data-ttu-id="0d2f2-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d2f2-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0d2f2-160">displayName</span></span>|<span data-ttu-id="0d2f2-161">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-161">String</span></span>|<span data-ttu-id="0d2f2-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d2f2-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-164">version</span><span class="sxs-lookup"><span data-stu-id="0d2f2-164">version</span></span>|<span data-ttu-id="0d2f2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0d2f2-165">Int32</span></span>|<span data-ttu-id="0d2f2-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-166">Version of the device configuration.</span></span> <span data-ttu-id="0d2f2-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d2f2-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0d2f2-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="0d2f2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0d2f2-169">Int32</span></span>|<span data-ttu-id="0d2f2-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0d2f2-171">Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0d2f2-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="0d2f2-172">keyStorageProvider</span></span>|[<span data-ttu-id="0d2f2-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="0d2f2-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="0d2f2-174">Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d2f2-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="0d2f2-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="0d2f2-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0d2f2-176">subjectNameFormat</span></span>|[<span data-ttu-id="0d2f2-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0d2f2-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="0d2f2-178">Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d2f2-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="0d2f2-179">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="0d2f2-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0d2f2-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0d2f2-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0d2f2-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0d2f2-182">Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d2f2-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="0d2f2-183">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0d2f2-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0d2f2-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0d2f2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0d2f2-185">Int32</span></span>|<span data-ttu-id="0d2f2-186">Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0d2f2-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0d2f2-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0d2f2-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0d2f2-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0d2f2-189">Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d2f2-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="0d2f2-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0d2f2-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="0d2f2-191">certificationAuthority</span></span>|<span data-ttu-id="0d2f2-192">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-192">String</span></span>|<span data-ttu-id="0d2f2-193">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="0d2f2-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="0d2f2-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="0d2f2-194">certificationAuthorityName</span></span>|<span data-ttu-id="0d2f2-195">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-195">String</span></span>|<span data-ttu-id="0d2f2-196">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="0d2f2-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="0d2f2-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="0d2f2-197">certificateTemplateName</span></span>|<span data-ttu-id="0d2f2-198">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-198">String</span></span>|<span data-ttu-id="0d2f2-199">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="0d2f2-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="0d2f2-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0d2f2-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0d2f2-201">String</span><span class="sxs-lookup"><span data-stu-id="0d2f2-201">String</span></span>|<span data-ttu-id="0d2f2-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="0d2f2-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0d2f2-203">extendedKeyUsages</span></span>|<span data-ttu-id="0d2f2-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="0d2f2-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0d2f2-205">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0d2f2-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0d2f2-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d2f2-207">Response</span></span>
<span data-ttu-id="0d2f2-208">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-208">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d2f2-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d2f2-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d2f2-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d2f2-210">Request</span></span>
<span data-ttu-id="0d2f2-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1011

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="0d2f2-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d2f2-212">Response</span></span>
<span data-ttu-id="0d2f2-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d2f2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




