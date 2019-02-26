---
title: Atualizar androidScepCertificateProfile
description: Atualiza as propriedades de um objeto androidScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 182710b083ac79604cb238226084f7bee02dd5c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151503"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="bc0fd-103">Atualizar androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bc0fd-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="bc0fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc0fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc0fd-106">Atualiza as propriedades de um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bc0fd-106">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc0fd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc0fd-107">Prerequisites</span></span>
<span data-ttu-id="bc0fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc0fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc0fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc0fd-110">Permission type</span></span>|<span data-ttu-id="bc0fd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc0fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc0fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc0fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc0fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-115">Not supported.</span></span>|
|<span data-ttu-id="bc0fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc0fd-116">Application</span></span>|<span data-ttu-id="bc0fd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc0fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc0fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bc0fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc0fd-119">Request headers</span></span>
|<span data-ttu-id="bc0fd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc0fd-120">Header</span></span>|<span data-ttu-id="bc0fd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bc0fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc0fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc0fd-122">Authorization</span></span>|<span data-ttu-id="bc0fd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc0fd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc0fd-124">Accept</span></span>|<span data-ttu-id="bc0fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc0fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc0fd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc0fd-126">Request body</span></span>
<span data-ttu-id="bc0fd-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bc0fd-127">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="bc0fd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="bc0fd-128">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="bc0fd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc0fd-129">Property</span></span>|<span data-ttu-id="bc0fd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0fd-130">Type</span></span>|<span data-ttu-id="bc0fd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc0fd-132">id</span><span class="sxs-lookup"><span data-stu-id="bc0fd-132">id</span></span>|<span data-ttu-id="bc0fd-133">String</span><span class="sxs-lookup"><span data-stu-id="bc0fd-133">String</span></span>|<span data-ttu-id="bc0fd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-134">Key of the entity.</span></span> <span data-ttu-id="bc0fd-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc0fd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bc0fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc0fd-137">DateTimeOffset</span></span>|<span data-ttu-id="bc0fd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bc0fd-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc0fd-140">roleScopeTagIds</span></span>|<span data-ttu-id="bc0fd-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc0fd-141">String collection</span></span>|<span data-ttu-id="bc0fd-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bc0fd-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bc0fd-144">supportsScopeTags</span></span>|<span data-ttu-id="bc0fd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc0fd-145">Boolean</span></span>|<span data-ttu-id="bc0fd-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bc0fd-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bc0fd-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bc0fd-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-149">This property is read-only.</span></span> <span data-ttu-id="bc0fd-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc0fd-151">createdDateTime</span></span>|<span data-ttu-id="bc0fd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc0fd-152">DateTimeOffset</span></span>|<span data-ttu-id="bc0fd-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-153">DateTime the object was created.</span></span> <span data-ttu-id="bc0fd-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-155">description</span><span class="sxs-lookup"><span data-stu-id="bc0fd-155">description</span></span>|<span data-ttu-id="bc0fd-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc0fd-156">String</span></span>|<span data-ttu-id="bc0fd-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc0fd-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bc0fd-159">displayName</span></span>|<span data-ttu-id="bc0fd-160">String</span><span class="sxs-lookup"><span data-stu-id="bc0fd-160">String</span></span>|<span data-ttu-id="bc0fd-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc0fd-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-163">version</span><span class="sxs-lookup"><span data-stu-id="bc0fd-163">version</span></span>|<span data-ttu-id="bc0fd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bc0fd-164">Int32</span></span>|<span data-ttu-id="bc0fd-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-165">Version of the device configuration.</span></span> <span data-ttu-id="bc0fd-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc0fd-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bc0fd-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="bc0fd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bc0fd-168">Int32</span></span>|<span data-ttu-id="bc0fd-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bc0fd-170">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc0fd-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bc0fd-171">subjectNameFormat</span></span>|[<span data-ttu-id="bc0fd-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bc0fd-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="bc0fd-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="bc0fd-174">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bc0fd-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="bc0fd-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="bc0fd-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bc0fd-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bc0fd-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bc0fd-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bc0fd-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="bc0fd-179">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bc0fd-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="bc0fd-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bc0fd-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bc0fd-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bc0fd-182">Int32</span><span class="sxs-lookup"><span data-stu-id="bc0fd-182">Int32</span></span>|<span data-ttu-id="bc0fd-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="bc0fd-184">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc0fd-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bc0fd-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bc0fd-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bc0fd-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bc0fd-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="bc0fd-188">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bc0fd-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="bc0fd-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bc0fd-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bc0fd-190">extendedKeyUsages</span></span>|<span data-ttu-id="bc0fd-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bc0fd-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="bc0fd-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bc0fd-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bc0fd-194">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fd-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc0fd-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="bc0fd-195">scepServerUrls</span></span>|<span data-ttu-id="bc0fd-196">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc0fd-196">String collection</span></span>|<span data-ttu-id="bc0fd-197">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="bc0fd-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="bc0fd-198">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bc0fd-198">subjectNameFormatString</span></span>|<span data-ttu-id="bc0fd-199">String</span><span class="sxs-lookup"><span data-stu-id="bc0fd-199">String</span></span>|<span data-ttu-id="bc0fd-200">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="bc0fd-201">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="bc0fd-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="bc0fd-202">uso de</span><span class="sxs-lookup"><span data-stu-id="bc0fd-202">keyUsage</span></span>|[<span data-ttu-id="bc0fd-203">usos de</span><span class="sxs-lookup"><span data-stu-id="bc0fd-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="bc0fd-204">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-204">SCEP Key Usage.</span></span> <span data-ttu-id="bc0fd-205">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="bc0fd-206">keySize</span><span class="sxs-lookup"><span data-stu-id="bc0fd-206">keySize</span></span>|[<span data-ttu-id="bc0fd-207">keySize</span><span class="sxs-lookup"><span data-stu-id="bc0fd-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="bc0fd-208">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-208">SCEP Key Size.</span></span> <span data-ttu-id="bc0fd-209">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="bc0fd-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="bc0fd-210">hashAlgorithm</span></span>|[<span data-ttu-id="bc0fd-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="bc0fd-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="bc0fd-212">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="bc0fd-213">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="bc0fd-214">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="bc0fd-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bc0fd-215">String</span><span class="sxs-lookup"><span data-stu-id="bc0fd-215">String</span></span>|<span data-ttu-id="bc0fd-216">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="bc0fd-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc0fd-217">Response</span></span>
<span data-ttu-id="bc0fd-218">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-218">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc0fd-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc0fd-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc0fd-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc0fd-220">Request</span></span>
<span data-ttu-id="bc0fd-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="bc0fd-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc0fd-222">Response</span></span>
<span data-ttu-id="bc0fd-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc0fd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




