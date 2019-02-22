---
title: Atualizar androidWorkProfilePkcsCertificateProfile
description: Atualiza as propriedades de um objeto androidWorkProfilePkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fbba0e2ae5974d9cd0738a5079c5c1324f00cfe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154492"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="8bcd4-103">Atualizar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8bcd4-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="8bcd4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bcd4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bcd4-106">Atualiza as propriedades de um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8bcd4-106">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bcd4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bcd4-107">Prerequisites</span></span>
<span data-ttu-id="8bcd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8bcd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8bcd4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bcd4-110">Permission type</span></span>|<span data-ttu-id="8bcd4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bcd4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bcd4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bcd4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bcd4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bcd4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-115">Not supported.</span></span>|
|<span data-ttu-id="8bcd4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bcd4-116">Application</span></span>|<span data-ttu-id="8bcd4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bcd4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bcd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8bcd4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcd4-119">Request headers</span></span>
|<span data-ttu-id="8bcd4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bcd4-120">Header</span></span>|<span data-ttu-id="8bcd4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8bcd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bcd4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bcd4-122">Authorization</span></span>|<span data-ttu-id="8bcd4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bcd4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bcd4-124">Accept</span></span>|<span data-ttu-id="8bcd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bcd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bcd4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcd4-126">Request body</span></span>
<span data-ttu-id="8bcd4-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8bcd4-127">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="8bcd4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8bcd4-128">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="8bcd4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bcd4-129">Property</span></span>|<span data-ttu-id="8bcd4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bcd4-130">Type</span></span>|<span data-ttu-id="8bcd4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bcd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bcd4-132">id</span><span class="sxs-lookup"><span data-stu-id="8bcd4-132">id</span></span>|<span data-ttu-id="8bcd4-133">String</span><span class="sxs-lookup"><span data-stu-id="8bcd4-133">String</span></span>|<span data-ttu-id="8bcd4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-134">Key of the entity.</span></span> <span data-ttu-id="8bcd4-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bcd4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8bcd4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bcd4-137">DateTimeOffset</span></span>|<span data-ttu-id="8bcd4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8bcd4-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8bcd4-140">roleScopeTagIds</span></span>|<span data-ttu-id="8bcd4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bcd4-141">String collection</span></span>|<span data-ttu-id="8bcd4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8bcd4-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8bcd4-144">supportsScopeTags</span></span>|<span data-ttu-id="8bcd4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="8bcd4-145">Boolean</span></span>|<span data-ttu-id="8bcd4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8bcd4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8bcd4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8bcd4-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-149">This property is read-only.</span></span> <span data-ttu-id="8bcd4-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bcd4-151">createdDateTime</span></span>|<span data-ttu-id="8bcd4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bcd4-152">DateTimeOffset</span></span>|<span data-ttu-id="8bcd4-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-153">DateTime the object was created.</span></span> <span data-ttu-id="8bcd4-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-155">description</span><span class="sxs-lookup"><span data-stu-id="8bcd4-155">description</span></span>|<span data-ttu-id="8bcd4-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bcd4-156">String</span></span>|<span data-ttu-id="8bcd4-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8bcd4-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8bcd4-159">displayName</span></span>|<span data-ttu-id="8bcd4-160">String</span><span class="sxs-lookup"><span data-stu-id="8bcd4-160">String</span></span>|<span data-ttu-id="8bcd4-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8bcd4-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-163">version</span><span class="sxs-lookup"><span data-stu-id="8bcd4-163">version</span></span>|<span data-ttu-id="8bcd4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8bcd4-164">Int32</span></span>|<span data-ttu-id="8bcd4-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-165">Version of the device configuration.</span></span> <span data-ttu-id="8bcd4-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bcd4-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8bcd4-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="8bcd4-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8bcd4-168">Int32</span></span>|<span data-ttu-id="8bcd4-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8bcd4-170">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8bcd4-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8bcd4-171">subjectNameFormat</span></span>|[<span data-ttu-id="8bcd4-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8bcd4-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="8bcd4-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="8bcd4-174">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8bcd4-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="8bcd4-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="8bcd4-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8bcd4-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8bcd4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8bcd4-177">Int32</span></span>|<span data-ttu-id="8bcd4-178">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8bcd4-179">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8bcd4-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8bcd4-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8bcd4-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8bcd4-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8bcd4-182">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8bcd4-183">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8bcd4-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="8bcd4-184">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8bcd4-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="8bcd4-185">extendedKeyUsages</span></span>|<span data-ttu-id="8bcd4-186">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8bcd4-187">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="8bcd4-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8bcd4-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8bcd4-189">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8bcd4-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8bcd4-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="8bcd4-190">certificationAuthority</span></span>|<span data-ttu-id="8bcd4-191">String</span><span class="sxs-lookup"><span data-stu-id="8bcd4-191">String</span></span>|<span data-ttu-id="8bcd4-192">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="8bcd4-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="8bcd4-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="8bcd4-193">certificationAuthorityName</span></span>|<span data-ttu-id="8bcd4-194">String</span><span class="sxs-lookup"><span data-stu-id="8bcd4-194">String</span></span>|<span data-ttu-id="8bcd4-195">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="8bcd4-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="8bcd4-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="8bcd4-196">certificateTemplateName</span></span>|<span data-ttu-id="8bcd4-197">String</span><span class="sxs-lookup"><span data-stu-id="8bcd4-197">String</span></span>|<span data-ttu-id="8bcd4-198">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="8bcd4-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="8bcd4-199">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="8bcd4-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8bcd4-200">String</span><span class="sxs-lookup"><span data-stu-id="8bcd4-200">String</span></span>|<span data-ttu-id="8bcd4-201">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="8bcd4-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8bcd4-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8bcd4-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8bcd4-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8bcd4-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="8bcd4-205">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-205">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="8bcd4-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bcd4-206">Response</span></span>
<span data-ttu-id="8bcd4-207">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-207">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bcd4-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bcd4-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bcd4-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcd4-209">Request</span></span>
<span data-ttu-id="8bcd4-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 969

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="8bcd4-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bcd4-211">Response</span></span>
<span data-ttu-id="8bcd4-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bcd4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```




