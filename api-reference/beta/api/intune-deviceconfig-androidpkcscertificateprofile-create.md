---
title: Criar androidPkcsCertificateProfile
description: Criar um novo objeto androidPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab7c714f5f334e6ce90710dc2e9d149d9cf22185
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33929214"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="4a111-103">Criar androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4a111-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="4a111-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a111-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a111-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a111-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a111-106">Criar um novo objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4a111-106">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a111-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a111-107">Prerequisites</span></span>
<span data-ttu-id="4a111-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a111-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a111-110">Permission type</span></span>|<span data-ttu-id="4a111-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a111-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a111-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a111-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a111-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a111-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a111-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a111-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a111-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a111-115">Not supported.</span></span>|
|<span data-ttu-id="4a111-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a111-116">Application</span></span>|<span data-ttu-id="4a111-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a111-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a111-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a111-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4a111-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a111-119">Request headers</span></span>
|<span data-ttu-id="4a111-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a111-120">Header</span></span>|<span data-ttu-id="4a111-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4a111-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a111-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a111-122">Authorization</span></span>|<span data-ttu-id="4a111-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a111-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a111-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a111-124">Accept</span></span>|<span data-ttu-id="4a111-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a111-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a111-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a111-126">Request body</span></span>
<span data-ttu-id="4a111-127">No corpo da solicitação, forneça uma representação JSON do objeto androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="4a111-127">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="4a111-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="4a111-128">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="4a111-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a111-129">Property</span></span>|<span data-ttu-id="4a111-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a111-130">Type</span></span>|<span data-ttu-id="4a111-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a111-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a111-132">id</span><span class="sxs-lookup"><span data-stu-id="4a111-132">id</span></span>|<span data-ttu-id="4a111-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a111-133">String</span></span>|<span data-ttu-id="4a111-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a111-134">Key of the entity.</span></span> <span data-ttu-id="4a111-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a111-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4a111-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a111-137">DateTimeOffset</span></span>|<span data-ttu-id="4a111-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4a111-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4a111-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a111-140">roleScopeTagIds</span></span>|<span data-ttu-id="4a111-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a111-141">String collection</span></span>|<span data-ttu-id="4a111-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4a111-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4a111-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4a111-144">supportsScopeTags</span></span>|<span data-ttu-id="4a111-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a111-145">Boolean</span></span>|<span data-ttu-id="4a111-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4a111-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4a111-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4a111-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4a111-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4a111-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4a111-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a111-149">This property is read-only.</span></span> <span data-ttu-id="4a111-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a111-151">createdDateTime</span></span>|<span data-ttu-id="4a111-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a111-152">DateTimeOffset</span></span>|<span data-ttu-id="4a111-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4a111-153">DateTime the object was created.</span></span> <span data-ttu-id="4a111-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-155">description</span><span class="sxs-lookup"><span data-stu-id="4a111-155">description</span></span>|<span data-ttu-id="4a111-156">String</span><span class="sxs-lookup"><span data-stu-id="4a111-156">String</span></span>|<span data-ttu-id="4a111-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a111-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a111-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4a111-159">displayName</span></span>|<span data-ttu-id="4a111-160">String</span><span class="sxs-lookup"><span data-stu-id="4a111-160">String</span></span>|<span data-ttu-id="4a111-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a111-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a111-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-163">versão</span><span class="sxs-lookup"><span data-stu-id="4a111-163">version</span></span>|<span data-ttu-id="4a111-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4a111-164">Int32</span></span>|<span data-ttu-id="4a111-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a111-165">Version of the device configuration.</span></span> <span data-ttu-id="4a111-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a111-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="4a111-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="4a111-168">Int32</span><span class="sxs-lookup"><span data-stu-id="4a111-168">Int32</span></span>|<span data-ttu-id="4a111-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="4a111-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4a111-170">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4a111-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4a111-171">subjectNameFormat</span></span>|[<span data-ttu-id="4a111-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4a111-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="4a111-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4a111-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="4a111-174">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a111-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="4a111-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="4a111-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="4a111-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4a111-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4a111-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4a111-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="4a111-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4a111-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="4a111-179">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a111-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="4a111-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="4a111-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="4a111-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4a111-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4a111-182">Int32</span><span class="sxs-lookup"><span data-stu-id="4a111-182">Int32</span></span>|<span data-ttu-id="4a111-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4a111-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="4a111-184">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4a111-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4a111-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4a111-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4a111-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="4a111-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4a111-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="4a111-188">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a111-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="4a111-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="4a111-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4a111-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="4a111-190">extendedKeyUsages</span></span>|<span data-ttu-id="4a111-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="4a111-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="4a111-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="4a111-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4a111-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4a111-194">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4a111-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4a111-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="4a111-195">certificationAuthority</span></span>|<span data-ttu-id="4a111-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a111-196">String</span></span>|<span data-ttu-id="4a111-197">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="4a111-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="4a111-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="4a111-198">certificationAuthorityName</span></span>|<span data-ttu-id="4a111-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a111-199">String</span></span>|<span data-ttu-id="4a111-200">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="4a111-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="4a111-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="4a111-201">certificateTemplateName</span></span>|<span data-ttu-id="4a111-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a111-202">String</span></span>|<span data-ttu-id="4a111-203">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="4a111-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="4a111-204">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="4a111-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4a111-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a111-205">String</span></span>|<span data-ttu-id="4a111-206">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="4a111-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="4a111-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a111-207">Response</span></span>
<span data-ttu-id="4a111-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a111-208">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a111-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a111-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a111-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a111-210">Request</span></span>
<span data-ttu-id="4a111-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a111-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4a111-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a111-212">Response</span></span>
<span data-ttu-id="4a111-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a111-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




