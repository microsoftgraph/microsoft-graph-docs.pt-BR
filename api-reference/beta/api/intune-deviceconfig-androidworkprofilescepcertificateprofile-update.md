---
title: Atualizar Entidadeandroidworkprofilescepcertificateprofile
description: Atualiza as propriedades de um objeto Entidadeandroidworkprofilescepcertificateprofile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: caf0b434a2ffb17dbe66fd48a59a4c5c715ef141
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32472985"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="19316-103">Atualizar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="19316-103">Update androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="19316-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19316-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19316-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19316-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19316-106">Atualiza as propriedades de um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="19316-106">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19316-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19316-107">Prerequisites</span></span>
<span data-ttu-id="19316-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19316-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19316-110">Permission type</span></span>|<span data-ttu-id="19316-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19316-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19316-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19316-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19316-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19316-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19316-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19316-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19316-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19316-115">Not supported.</span></span>|
|<span data-ttu-id="19316-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19316-116">Application</span></span>|<span data-ttu-id="19316-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19316-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19316-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19316-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="19316-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19316-119">Request headers</span></span>
|<span data-ttu-id="19316-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19316-120">Header</span></span>|<span data-ttu-id="19316-121">Valor</span><span class="sxs-lookup"><span data-stu-id="19316-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19316-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="19316-122">Authorization</span></span>|<span data-ttu-id="19316-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19316-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19316-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19316-124">Accept</span></span>|<span data-ttu-id="19316-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19316-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19316-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19316-126">Request body</span></span>
<span data-ttu-id="19316-127">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="19316-127">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="19316-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="19316-128">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="19316-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19316-129">Property</span></span>|<span data-ttu-id="19316-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="19316-130">Type</span></span>|<span data-ttu-id="19316-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="19316-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19316-132">id</span><span class="sxs-lookup"><span data-stu-id="19316-132">id</span></span>|<span data-ttu-id="19316-133">String</span><span class="sxs-lookup"><span data-stu-id="19316-133">String</span></span>|<span data-ttu-id="19316-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="19316-134">Key of the entity.</span></span> <span data-ttu-id="19316-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19316-136">lastModifiedDateTime</span></span>|<span data-ttu-id="19316-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19316-137">DateTimeOffset</span></span>|<span data-ttu-id="19316-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="19316-138">DateTime the object was last modified.</span></span> <span data-ttu-id="19316-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19316-140">roleScopeTagIds</span></span>|<span data-ttu-id="19316-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="19316-141">String collection</span></span>|<span data-ttu-id="19316-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="19316-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="19316-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="19316-144">supportsScopeTags</span></span>|<span data-ttu-id="19316-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="19316-145">Boolean</span></span>|<span data-ttu-id="19316-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="19316-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="19316-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="19316-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="19316-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="19316-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="19316-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="19316-149">This property is read-only.</span></span> <span data-ttu-id="19316-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19316-151">createdDateTime</span></span>|<span data-ttu-id="19316-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19316-152">DateTimeOffset</span></span>|<span data-ttu-id="19316-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="19316-153">DateTime the object was created.</span></span> <span data-ttu-id="19316-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-155">description</span><span class="sxs-lookup"><span data-stu-id="19316-155">description</span></span>|<span data-ttu-id="19316-156">String</span><span class="sxs-lookup"><span data-stu-id="19316-156">String</span></span>|<span data-ttu-id="19316-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19316-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19316-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-159">displayName</span><span class="sxs-lookup"><span data-stu-id="19316-159">displayName</span></span>|<span data-ttu-id="19316-160">String</span><span class="sxs-lookup"><span data-stu-id="19316-160">String</span></span>|<span data-ttu-id="19316-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19316-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19316-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-163">versão</span><span class="sxs-lookup"><span data-stu-id="19316-163">version</span></span>|<span data-ttu-id="19316-164">Int32</span><span class="sxs-lookup"><span data-stu-id="19316-164">Int32</span></span>|<span data-ttu-id="19316-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19316-165">Version of the device configuration.</span></span> <span data-ttu-id="19316-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19316-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19316-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="19316-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="19316-168">Int32</span><span class="sxs-lookup"><span data-stu-id="19316-168">Int32</span></span>|<span data-ttu-id="19316-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="19316-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="19316-170">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="19316-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="19316-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="19316-171">subjectNameFormat</span></span>|[<span data-ttu-id="19316-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="19316-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="19316-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="19316-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="19316-174">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="19316-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="19316-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="19316-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="19316-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="19316-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="19316-177">Int32</span><span class="sxs-lookup"><span data-stu-id="19316-177">Int32</span></span>|<span data-ttu-id="19316-178">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="19316-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="19316-179">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="19316-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="19316-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="19316-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="19316-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="19316-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="19316-182">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="19316-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="19316-183">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="19316-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="19316-184">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="19316-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="19316-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="19316-185">extendedKeyUsages</span></span>|<span data-ttu-id="19316-186">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="19316-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="19316-187">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="19316-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="19316-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="19316-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="19316-189">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="19316-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="19316-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="19316-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="19316-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="19316-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="19316-192">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="19316-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="19316-193">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="19316-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="19316-194">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="19316-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="19316-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="19316-195">scepServerUrls</span></span>|<span data-ttu-id="19316-196">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="19316-196">String collection</span></span>|<span data-ttu-id="19316-197">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="19316-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="19316-198">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="19316-198">subjectNameFormatString</span></span>|<span data-ttu-id="19316-199">String</span><span class="sxs-lookup"><span data-stu-id="19316-199">String</span></span>|<span data-ttu-id="19316-200">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="19316-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="19316-201">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="19316-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="19316-202">uso de</span><span class="sxs-lookup"><span data-stu-id="19316-202">keyUsage</span></span>|[<span data-ttu-id="19316-203">usos de</span><span class="sxs-lookup"><span data-stu-id="19316-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="19316-204">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="19316-204">SCEP Key Usage.</span></span> <span data-ttu-id="19316-205">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="19316-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="19316-206">keySize</span><span class="sxs-lookup"><span data-stu-id="19316-206">keySize</span></span>|[<span data-ttu-id="19316-207">keySize</span><span class="sxs-lookup"><span data-stu-id="19316-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="19316-208">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="19316-208">SCEP Key Size.</span></span> <span data-ttu-id="19316-209">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="19316-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="19316-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="19316-210">hashAlgorithm</span></span>|[<span data-ttu-id="19316-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="19316-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="19316-212">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="19316-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="19316-213">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="19316-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="19316-214">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="19316-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="19316-215">String</span><span class="sxs-lookup"><span data-stu-id="19316-215">String</span></span>|<span data-ttu-id="19316-216">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="19316-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="19316-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="19316-217">certificateStore</span></span>|[<span data-ttu-id="19316-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="19316-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="19316-219">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="19316-219">Target store certificate.</span></span> <span data-ttu-id="19316-220">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="19316-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="19316-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="19316-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="19316-222">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="19316-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="19316-223">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="19316-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="19316-224">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="19316-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="19316-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="19316-225">Response</span></span>
<span data-ttu-id="19316-226">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19316-226">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19316-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19316-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="19316-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19316-228">Request</span></span>
<span data-ttu-id="19316-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19316-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
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
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="19316-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="19316-230">Response</span></span>
<span data-ttu-id="19316-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19316-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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





