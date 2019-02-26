---
title: Atualizar windowsPhone81SCEPCertificateProfile
description: Atualiza as propriedades de um objeto windowsPhone81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e87b876c70a9dcd76425fd3d124178beffff1c74
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160225"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="d844e-103">Atualizar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d844e-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="d844e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d844e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d844e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d844e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d844e-106">Atualiza as propriedades de um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d844e-106">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d844e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d844e-107">Prerequisites</span></span>
<span data-ttu-id="d844e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d844e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d844e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d844e-110">Permission type</span></span>|<span data-ttu-id="d844e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d844e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d844e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d844e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d844e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d844e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d844e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d844e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d844e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d844e-115">Not supported.</span></span>|
|<span data-ttu-id="d844e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d844e-116">Application</span></span>|<span data-ttu-id="d844e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d844e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d844e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d844e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d844e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d844e-119">Request headers</span></span>
|<span data-ttu-id="d844e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d844e-120">Header</span></span>|<span data-ttu-id="d844e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d844e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d844e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d844e-122">Authorization</span></span>|<span data-ttu-id="d844e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d844e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d844e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d844e-124">Accept</span></span>|<span data-ttu-id="d844e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d844e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d844e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d844e-126">Request body</span></span>
<span data-ttu-id="d844e-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d844e-127">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d844e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d844e-128">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="d844e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d844e-129">Property</span></span>|<span data-ttu-id="d844e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d844e-130">Type</span></span>|<span data-ttu-id="d844e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d844e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d844e-132">id</span><span class="sxs-lookup"><span data-stu-id="d844e-132">id</span></span>|<span data-ttu-id="d844e-133">String</span><span class="sxs-lookup"><span data-stu-id="d844e-133">String</span></span>|<span data-ttu-id="d844e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d844e-134">Key of the entity.</span></span> <span data-ttu-id="d844e-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d844e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d844e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d844e-137">DateTimeOffset</span></span>|<span data-ttu-id="d844e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d844e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d844e-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d844e-140">roleScopeTagIds</span></span>|<span data-ttu-id="d844e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d844e-141">String collection</span></span>|<span data-ttu-id="d844e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d844e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d844e-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d844e-144">supportsScopeTags</span></span>|<span data-ttu-id="d844e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d844e-145">Boolean</span></span>|<span data-ttu-id="d844e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d844e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d844e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d844e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d844e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d844e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d844e-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d844e-149">This property is read-only.</span></span> <span data-ttu-id="d844e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d844e-151">createdDateTime</span></span>|<span data-ttu-id="d844e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d844e-152">DateTimeOffset</span></span>|<span data-ttu-id="d844e-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d844e-153">DateTime the object was created.</span></span> <span data-ttu-id="d844e-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-155">description</span><span class="sxs-lookup"><span data-stu-id="d844e-155">description</span></span>|<span data-ttu-id="d844e-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d844e-156">String</span></span>|<span data-ttu-id="d844e-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d844e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d844e-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d844e-159">displayName</span></span>|<span data-ttu-id="d844e-160">String</span><span class="sxs-lookup"><span data-stu-id="d844e-160">String</span></span>|<span data-ttu-id="d844e-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d844e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d844e-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-163">version</span><span class="sxs-lookup"><span data-stu-id="d844e-163">version</span></span>|<span data-ttu-id="d844e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d844e-164">Int32</span></span>|<span data-ttu-id="d844e-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d844e-165">Version of the device configuration.</span></span> <span data-ttu-id="d844e-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d844e-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d844e-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="d844e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d844e-168">Int32</span></span>|<span data-ttu-id="d844e-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="d844e-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d844e-170">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d844e-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d844e-171">keyStorageProvider</span></span>|[<span data-ttu-id="d844e-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d844e-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d844e-173">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="d844e-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="d844e-174">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d844e-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="d844e-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="d844e-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="d844e-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d844e-176">subjectNameFormat</span></span>|[<span data-ttu-id="d844e-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d844e-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d844e-178">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d844e-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="d844e-179">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d844e-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="d844e-180">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d844e-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d844e-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d844e-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d844e-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d844e-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d844e-183">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d844e-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d844e-184">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d844e-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="d844e-185">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d844e-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d844e-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d844e-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d844e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="d844e-187">Int32</span></span>|<span data-ttu-id="d844e-188">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="d844e-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="d844e-189">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d844e-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d844e-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d844e-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d844e-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d844e-192">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d844e-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d844e-193">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d844e-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="d844e-194">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d844e-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d844e-195">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d844e-195">extendedKeyUsages</span></span>|<span data-ttu-id="d844e-196">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d844e-197">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="d844e-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d844e-198">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d844e-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d844e-199">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d844e-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d844e-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="d844e-200">scepServerUrls</span></span>|<span data-ttu-id="d844e-201">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d844e-201">String collection</span></span>|<span data-ttu-id="d844e-202">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="d844e-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="d844e-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d844e-203">subjectNameFormatString</span></span>|<span data-ttu-id="d844e-204">String</span><span class="sxs-lookup"><span data-stu-id="d844e-204">String</span></span>|<span data-ttu-id="d844e-205">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="d844e-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d844e-206">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="d844e-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d844e-207">uso de</span><span class="sxs-lookup"><span data-stu-id="d844e-207">keyUsage</span></span>|[<span data-ttu-id="d844e-208">usos de</span><span class="sxs-lookup"><span data-stu-id="d844e-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d844e-209">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="d844e-209">SCEP Key Usage.</span></span> <span data-ttu-id="d844e-210">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="d844e-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d844e-211">keySize</span><span class="sxs-lookup"><span data-stu-id="d844e-211">keySize</span></span>|[<span data-ttu-id="d844e-212">keySize</span><span class="sxs-lookup"><span data-stu-id="d844e-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="d844e-213">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="d844e-213">SCEP Key Size.</span></span> <span data-ttu-id="d844e-214">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="d844e-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="d844e-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d844e-215">hashAlgorithm</span></span>|[<span data-ttu-id="d844e-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d844e-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="d844e-217">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="d844e-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="d844e-218">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="d844e-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="d844e-219">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="d844e-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d844e-220">String</span><span class="sxs-lookup"><span data-stu-id="d844e-220">String</span></span>|<span data-ttu-id="d844e-221">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="d844e-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="d844e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="d844e-222">Response</span></span>
<span data-ttu-id="d844e-223">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d844e-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d844e-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d844e-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="d844e-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d844e-225">Request</span></span>
<span data-ttu-id="d844e-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d844e-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="d844e-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="d844e-227">Response</span></span>
<span data-ttu-id="d844e-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d844e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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




