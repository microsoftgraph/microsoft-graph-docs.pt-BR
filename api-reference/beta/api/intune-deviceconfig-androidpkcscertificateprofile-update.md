---
title: Atualizar androidPkcsCertificateProfile
description: Atualiza as propriedades de um objeto androidPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4142893ca96f953a8269fa54be07a9b35f5a9ff8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779192"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="3741a-103">Atualizar androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3741a-103">Update androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="3741a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3741a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3741a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3741a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3741a-106">Atualiza as propriedades de um objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3741a-106">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3741a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3741a-107">Prerequisites</span></span>
<span data-ttu-id="3741a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3741a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3741a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3741a-110">Permission type</span></span>|<span data-ttu-id="3741a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3741a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3741a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3741a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3741a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3741a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3741a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3741a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3741a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3741a-115">Not supported.</span></span>|
|<span data-ttu-id="3741a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3741a-116">Application</span></span>|<span data-ttu-id="3741a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3741a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3741a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3741a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3741a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3741a-119">Request headers</span></span>
|<span data-ttu-id="3741a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3741a-120">Header</span></span>|<span data-ttu-id="3741a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3741a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3741a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3741a-122">Authorization</span></span>|<span data-ttu-id="3741a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3741a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3741a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3741a-124">Accept</span></span>|<span data-ttu-id="3741a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3741a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3741a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3741a-126">Request body</span></span>
<span data-ttu-id="3741a-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3741a-127">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="3741a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-128">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="3741a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3741a-129">Property</span></span>|<span data-ttu-id="3741a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3741a-130">Type</span></span>|<span data-ttu-id="3741a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3741a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3741a-132">id</span><span class="sxs-lookup"><span data-stu-id="3741a-132">id</span></span>|<span data-ttu-id="3741a-133">String</span><span class="sxs-lookup"><span data-stu-id="3741a-133">String</span></span>|<span data-ttu-id="3741a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3741a-134">Key of the entity.</span></span> <span data-ttu-id="3741a-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3741a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3741a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3741a-137">DateTimeOffset</span></span>|<span data-ttu-id="3741a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3741a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3741a-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3741a-140">roleScopeTagIds</span></span>|<span data-ttu-id="3741a-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="3741a-141">String collection</span></span>|<span data-ttu-id="3741a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3741a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3741a-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3741a-144">supportsScopeTags</span></span>|<span data-ttu-id="3741a-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3741a-145">Boolean</span></span>|<span data-ttu-id="3741a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3741a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3741a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3741a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3741a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3741a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3741a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3741a-149">This property is read-only.</span></span> <span data-ttu-id="3741a-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3741a-151">createdDateTime</span></span>|<span data-ttu-id="3741a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3741a-152">DateTimeOffset</span></span>|<span data-ttu-id="3741a-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3741a-153">DateTime the object was created.</span></span> <span data-ttu-id="3741a-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-155">description</span><span class="sxs-lookup"><span data-stu-id="3741a-155">description</span></span>|<span data-ttu-id="3741a-156">String</span><span class="sxs-lookup"><span data-stu-id="3741a-156">String</span></span>|<span data-ttu-id="3741a-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3741a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3741a-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3741a-159">displayName</span></span>|<span data-ttu-id="3741a-160">String</span><span class="sxs-lookup"><span data-stu-id="3741a-160">String</span></span>|<span data-ttu-id="3741a-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3741a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3741a-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-163">versão</span><span class="sxs-lookup"><span data-stu-id="3741a-163">version</span></span>|<span data-ttu-id="3741a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3741a-164">Int32</span></span>|<span data-ttu-id="3741a-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3741a-165">Version of the device configuration.</span></span> <span data-ttu-id="3741a-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3741a-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="3741a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3741a-168">Int32</span></span>|<span data-ttu-id="3741a-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="3741a-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3741a-170">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3741a-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3741a-171">subjectNameFormat</span></span>|[<span data-ttu-id="3741a-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3741a-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3741a-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3741a-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="3741a-174">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3741a-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3741a-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3741a-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3741a-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3741a-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3741a-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3741a-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3741a-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3741a-179">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3741a-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3741a-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3741a-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3741a-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3741a-182">Int32</span><span class="sxs-lookup"><span data-stu-id="3741a-182">Int32</span></span>|<span data-ttu-id="3741a-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3741a-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3741a-184">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3741a-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3741a-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3741a-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3741a-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3741a-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3741a-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3741a-188">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3741a-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3741a-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3741a-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3741a-190">extendedKeyUsages</span></span>|<span data-ttu-id="3741a-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3741a-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="3741a-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3741a-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3741a-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3741a-194">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3741a-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="3741a-195">certificationAuthority</span></span>|<span data-ttu-id="3741a-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3741a-196">String</span></span>|<span data-ttu-id="3741a-197">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="3741a-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="3741a-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="3741a-198">certificationAuthorityName</span></span>|<span data-ttu-id="3741a-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3741a-199">String</span></span>|<span data-ttu-id="3741a-200">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="3741a-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="3741a-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="3741a-201">certificateTemplateName</span></span>|<span data-ttu-id="3741a-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3741a-202">String</span></span>|<span data-ttu-id="3741a-203">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="3741a-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="3741a-204">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="3741a-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3741a-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3741a-205">String</span></span>|<span data-ttu-id="3741a-206">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="3741a-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3741a-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="3741a-207">Response</span></span>
<span data-ttu-id="3741a-208">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3741a-208">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3741a-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3741a-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="3741a-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3741a-210">Request</span></span>
<span data-ttu-id="3741a-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3741a-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 958

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="3741a-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="3741a-212">Response</span></span>
<span data-ttu-id="3741a-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3741a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





