---
title: Criar windows10XSCEPCertificateProfile
description: Crie um novo objeto windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7306505efd37a879f700eee14b5535ed2bc36fe7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151981"
---
# <a name="create-windows10xscepcertificateprofile"></a><span data-ttu-id="45a1d-103">Criar windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="45a1d-103">Create windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="45a1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45a1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45a1d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45a1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45a1d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45a1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a1d-107">Crie um novo [objeto windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-107">Create a new [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45a1d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45a1d-108">Prerequisites</span></span>
<span data-ttu-id="45a1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45a1d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45a1d-111">Permission type</span></span>|<span data-ttu-id="45a1d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45a1d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a1d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45a1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45a1d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a1d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45a1d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45a1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a1d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a1d-116">Not supported.</span></span>|
|<span data-ttu-id="45a1d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45a1d-117">Application</span></span>|<span data-ttu-id="45a1d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a1d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a1d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="45a1d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a1d-120">Request headers</span></span>
|<span data-ttu-id="45a1d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45a1d-121">Header</span></span>|<span data-ttu-id="45a1d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45a1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45a1d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a1d-123">Authorization</span></span>|<span data-ttu-id="45a1d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45a1d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45a1d-125">Accept</span></span>|<span data-ttu-id="45a1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45a1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a1d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45a1d-127">Request body</span></span>
<span data-ttu-id="45a1d-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10XSCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="45a1d-128">In the request body, supply a JSON representation for the windows10XSCEPCertificateProfile object.</span></span>

<span data-ttu-id="45a1d-129">A tabela a seguir mostra as propriedades necessárias ao criar o windows10XSCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="45a1d-129">The following table shows the properties that are required when you create the windows10XSCEPCertificateProfile.</span></span>

|<span data-ttu-id="45a1d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45a1d-130">Property</span></span>|<span data-ttu-id="45a1d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a1d-131">Type</span></span>|<span data-ttu-id="45a1d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a1d-133">id</span><span class="sxs-lookup"><span data-stu-id="45a1d-133">id</span></span>|<span data-ttu-id="45a1d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a1d-134">String</span></span>|<span data-ttu-id="45a1d-135">Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-136">versão</span><span class="sxs-lookup"><span data-stu-id="45a1d-136">version</span></span>|<span data-ttu-id="45a1d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="45a1d-137">Int32</span></span>|<span data-ttu-id="45a1d-138">Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="45a1d-139">displayName</span></span>|<span data-ttu-id="45a1d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a1d-140">String</span></span>|<span data-ttu-id="45a1d-141">Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-142">descrição</span><span class="sxs-lookup"><span data-stu-id="45a1d-142">description</span></span>|<span data-ttu-id="45a1d-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a1d-143">String</span></span>|<span data-ttu-id="45a1d-144">Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="45a1d-145">creationDateTime</span></span>|<span data-ttu-id="45a1d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a1d-146">DateTimeOffset</span></span>|<span data-ttu-id="45a1d-147">Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45a1d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="45a1d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a1d-149">DateTimeOffset</span></span>|<span data-ttu-id="45a1d-150">O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45a1d-151">roleScopeTagIds</span></span>|<span data-ttu-id="45a1d-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a1d-152">String collection</span></span>|<span data-ttu-id="45a1d-153">Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="45a1d-154">certificateStore</span><span class="sxs-lookup"><span data-stu-id="45a1d-154">certificateStore</span></span>|[<span data-ttu-id="45a1d-155">certificateStore</span><span class="sxs-lookup"><span data-stu-id="45a1d-155">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="45a1d-156">Certificado de armazenamento de destino.</span><span class="sxs-lookup"><span data-stu-id="45a1d-156">Target store certificate.</span></span> <span data-ttu-id="45a1d-157">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="45a1d-157">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="45a1d-158">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45a1d-158">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="45a1d-159">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45a1d-159">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="45a1d-160">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="45a1d-160">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="45a1d-161">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="45a1d-161">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="45a1d-162">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="45a1d-162">certificateValidityPeriodValue</span></span>|<span data-ttu-id="45a1d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="45a1d-163">Int32</span></span>|<span data-ttu-id="45a1d-164">Valor do Período de Validade do Certificado</span><span class="sxs-lookup"><span data-stu-id="45a1d-164">Value for the Certificate Validity Period</span></span>|
|<span data-ttu-id="45a1d-165">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="45a1d-165">extendedKeyUsages</span></span>|<span data-ttu-id="45a1d-166">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="45a1d-167">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="45a1d-167">Extended Key Usage (EKU) settings.</span></span>|
|<span data-ttu-id="45a1d-168">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="45a1d-168">hashAlgorithm</span></span>|<span data-ttu-id="45a1d-169">[Coleção hashAlgorithms](../resources/intune-shared-hashalgorithms.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) collection</span></span>|<span data-ttu-id="45a1d-170">Algoritmo de hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="45a1d-170">SCEP Hash Algorithm.</span></span> <span data-ttu-id="45a1d-171">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="45a1d-171">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="45a1d-172">keySize</span><span class="sxs-lookup"><span data-stu-id="45a1d-172">keySize</span></span>|[<span data-ttu-id="45a1d-173">keySize</span><span class="sxs-lookup"><span data-stu-id="45a1d-173">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="45a1d-174">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="45a1d-174">SCEP Key Size.</span></span> <span data-ttu-id="45a1d-175">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="45a1d-175">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="45a1d-176">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="45a1d-176">keyStorageProvider</span></span>|[<span data-ttu-id="45a1d-177">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="45a1d-177">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="45a1d-178">KSP (Provedor de Armazenamento de Chaves).</span><span class="sxs-lookup"><span data-stu-id="45a1d-178">Key Storage Provider (KSP).</span></span> <span data-ttu-id="45a1d-179">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="45a1d-179">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="45a1d-180">keyUsage</span><span class="sxs-lookup"><span data-stu-id="45a1d-180">keyUsage</span></span>|[<span data-ttu-id="45a1d-181">keyUsages</span><span class="sxs-lookup"><span data-stu-id="45a1d-181">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="45a1d-182">Uso da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="45a1d-182">SCEP Key Usage.</span></span> <span data-ttu-id="45a1d-183">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="45a1d-183">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="45a1d-184">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="45a1d-184">renewalThresholdPercentage</span></span>|<span data-ttu-id="45a1d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="45a1d-185">Int32</span></span>|<span data-ttu-id="45a1d-186">Porcentagem de limite de renovação de certificado</span><span class="sxs-lookup"><span data-stu-id="45a1d-186">Certificate renewal threshold percentage</span></span>|
|<span data-ttu-id="45a1d-187">rootCertificateId</span><span class="sxs-lookup"><span data-stu-id="45a1d-187">rootCertificateId</span></span>|<span data-ttu-id="45a1d-188">Guid</span><span class="sxs-lookup"><span data-stu-id="45a1d-188">Guid</span></span>|<span data-ttu-id="45a1d-189">ID de certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="45a1d-189">Trusted Root Certificate ID</span></span>|
|<span data-ttu-id="45a1d-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="45a1d-190">scepServerUrls</span></span>|<span data-ttu-id="45a1d-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a1d-191">String collection</span></span>|<span data-ttu-id="45a1d-192">Url(s) do servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="45a1d-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="45a1d-193">subjectAlternativeNameFormats</span><span class="sxs-lookup"><span data-stu-id="45a1d-193">subjectAlternativeNameFormats</span></span>|<span data-ttu-id="45a1d-194">[Coleção windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="45a1d-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) collection</span></span>|<span data-ttu-id="45a1d-195">Atributos personalizados do AAD.</span><span class="sxs-lookup"><span data-stu-id="45a1d-195">Custom AAD Attributes.</span></span>|
|<span data-ttu-id="45a1d-196">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="45a1d-196">subjectNameFormatString</span></span>|<span data-ttu-id="45a1d-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a1d-197">String</span></span>|<span data-ttu-id="45a1d-198">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="45a1d-198">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="45a1d-199">Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="45a1d-199">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|



## <a name="response"></a><span data-ttu-id="45a1d-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a1d-200">Response</span></span>
<span data-ttu-id="45a1d-201">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45a1d-201">If successful, this method returns a `201 Created` response code and a [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45a1d-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45a1d-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="45a1d-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a1d-203">Request</span></span>
<span data-ttu-id="45a1d-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45a1d-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 1178

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "certificateStore": "machine",
  "certificateValidityPeriodScale": "months",
  "certificateValidityPeriodValue": 14,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "hashAlgorithm": [
    "sha2"
  ],
  "keySize": "size2048",
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "keyUsage": "digitalSignature",
  "renewalThresholdPercentage": 10,
  "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="45a1d-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a1d-205">Response</span></span>
<span data-ttu-id="45a1d-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45a1d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1291

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "certificateStore": "machine",
  "certificateValidityPeriodScale": "months",
  "certificateValidityPeriodValue": 14,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "hashAlgorithm": [
    "sha2"
  ],
  "keySize": "size2048",
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "keyUsage": "digitalSignature",
  "renewalThresholdPercentage": 10,
  "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value"
}
```




