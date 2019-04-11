---
title: Criar androidPkcsCertificateProfile
description: Criar um novo objeto androidPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 207ee5b51d66658605e413464da37268822a44e6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773585"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="a0c29-103">Criar androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a0c29-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="a0c29-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0c29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0c29-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0c29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0c29-106">Criar um novo objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c29-106">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0c29-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0c29-107">Prerequisites</span></span>
<span data-ttu-id="a0c29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0c29-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0c29-110">Permission type</span></span>|<span data-ttu-id="a0c29-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0c29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0c29-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0c29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0c29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0c29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0c29-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0c29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0c29-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0c29-115">Not supported.</span></span>|
|<span data-ttu-id="a0c29-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0c29-116">Application</span></span>|<span data-ttu-id="a0c29-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0c29-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0c29-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0c29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0c29-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0c29-119">Request headers</span></span>
|<span data-ttu-id="a0c29-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0c29-120">Header</span></span>|<span data-ttu-id="a0c29-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0c29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0c29-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0c29-122">Authorization</span></span>|<span data-ttu-id="a0c29-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0c29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0c29-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0c29-124">Accept</span></span>|<span data-ttu-id="a0c29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0c29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0c29-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0c29-126">Request body</span></span>
<span data-ttu-id="a0c29-127">No corpo da solicitação, forneça uma representação JSON do objeto androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a0c29-127">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="a0c29-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a0c29-128">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="a0c29-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0c29-129">Property</span></span>|<span data-ttu-id="a0c29-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0c29-130">Type</span></span>|<span data-ttu-id="a0c29-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0c29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0c29-132">id</span><span class="sxs-lookup"><span data-stu-id="a0c29-132">id</span></span>|<span data-ttu-id="a0c29-133">String</span><span class="sxs-lookup"><span data-stu-id="a0c29-133">String</span></span>|<span data-ttu-id="a0c29-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0c29-134">Key of the entity.</span></span> <span data-ttu-id="a0c29-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c29-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a0c29-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c29-137">DateTimeOffset</span></span>|<span data-ttu-id="a0c29-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0c29-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a0c29-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0c29-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0c29-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a0c29-141">String collection</span></span>|<span data-ttu-id="a0c29-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a0c29-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0c29-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0c29-144">supportsScopeTags</span></span>|<span data-ttu-id="a0c29-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a0c29-145">Boolean</span></span>|<span data-ttu-id="a0c29-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a0c29-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0c29-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a0c29-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0c29-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0c29-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0c29-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0c29-149">This property is read-only.</span></span> <span data-ttu-id="a0c29-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c29-151">createdDateTime</span></span>|<span data-ttu-id="a0c29-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c29-152">DateTimeOffset</span></span>|<span data-ttu-id="a0c29-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a0c29-153">DateTime the object was created.</span></span> <span data-ttu-id="a0c29-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-155">description</span><span class="sxs-lookup"><span data-stu-id="a0c29-155">description</span></span>|<span data-ttu-id="a0c29-156">String</span><span class="sxs-lookup"><span data-stu-id="a0c29-156">String</span></span>|<span data-ttu-id="a0c29-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0c29-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0c29-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a0c29-159">displayName</span></span>|<span data-ttu-id="a0c29-160">String</span><span class="sxs-lookup"><span data-stu-id="a0c29-160">String</span></span>|<span data-ttu-id="a0c29-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0c29-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0c29-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-163">versão</span><span class="sxs-lookup"><span data-stu-id="a0c29-163">version</span></span>|<span data-ttu-id="a0c29-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a0c29-164">Int32</span></span>|<span data-ttu-id="a0c29-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0c29-165">Version of the device configuration.</span></span> <span data-ttu-id="a0c29-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0c29-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a0c29-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="a0c29-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a0c29-168">Int32</span></span>|<span data-ttu-id="a0c29-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="a0c29-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a0c29-170">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0c29-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a0c29-171">subjectNameFormat</span></span>|[<span data-ttu-id="a0c29-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a0c29-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a0c29-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0c29-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="a0c29-174">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0c29-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a0c29-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a0c29-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a0c29-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a0c29-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a0c29-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a0c29-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a0c29-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0c29-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a0c29-179">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0c29-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a0c29-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a0c29-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a0c29-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a0c29-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a0c29-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a0c29-182">Int32</span></span>|<span data-ttu-id="a0c29-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0c29-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a0c29-184">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0c29-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a0c29-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a0c29-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a0c29-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a0c29-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a0c29-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a0c29-188">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0c29-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a0c29-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a0c29-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a0c29-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a0c29-190">extendedKeyUsages</span></span>|<span data-ttu-id="a0c29-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a0c29-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="a0c29-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a0c29-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a0c29-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a0c29-194">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0c29-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0c29-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="a0c29-195">certificationAuthority</span></span>|<span data-ttu-id="a0c29-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0c29-196">String</span></span>|<span data-ttu-id="a0c29-197">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="a0c29-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="a0c29-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="a0c29-198">certificationAuthorityName</span></span>|<span data-ttu-id="a0c29-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0c29-199">String</span></span>|<span data-ttu-id="a0c29-200">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="a0c29-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="a0c29-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="a0c29-201">certificateTemplateName</span></span>|<span data-ttu-id="a0c29-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0c29-202">String</span></span>|<span data-ttu-id="a0c29-203">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="a0c29-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="a0c29-204">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="a0c29-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a0c29-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0c29-205">String</span></span>|<span data-ttu-id="a0c29-206">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="a0c29-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a0c29-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0c29-207">Response</span></span>
<span data-ttu-id="a0c29-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0c29-208">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0c29-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0c29-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0c29-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0c29-210">Request</span></span>
<span data-ttu-id="a0c29-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0c29-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0c29-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0c29-212">Response</span></span>
<span data-ttu-id="a0c29-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0c29-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





