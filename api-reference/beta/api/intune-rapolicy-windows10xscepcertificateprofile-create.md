---
title: Criar windows10XSCEPCertificateProfile
description: Criar um novo objeto windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d6fae55ffb8f97ab12eda59f4ac5b2d066e9f59
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241304"
---
# <a name="create-windows10xscepcertificateprofile"></a><span data-ttu-id="0a0a5-103">Criar windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0a0a5-103">Create windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="0a0a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a0a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a0a5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a0a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a0a5-107">Criar um novo objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0a0a5-107">Create a new [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a0a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a0a5-108">Prerequisites</span></span>
<span data-ttu-id="0a0a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a0a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a0a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a0a5-111">Permission type</span></span>|<span data-ttu-id="0a0a5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a0a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a0a5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a0a5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a0a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a0a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-116">Not supported.</span></span>|
|<span data-ttu-id="0a0a5-117">Application</span><span class="sxs-lookup"><span data-stu-id="0a0a5-117">Application</span></span>|<span data-ttu-id="0a0a5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a0a5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a0a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a0a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0a0a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a0a5-120">Request headers</span></span>
|<span data-ttu-id="0a0a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a0a5-121">Header</span></span>|<span data-ttu-id="0a0a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0a0a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a0a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a0a5-123">Authorization</span></span>|<span data-ttu-id="0a0a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a0a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a0a5-125">Accept</span></span>|<span data-ttu-id="0a0a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a0a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a0a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a0a5-127">Request body</span></span>
<span data-ttu-id="0a0a5-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10XSCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-128">In the request body, supply a JSON representation for the windows10XSCEPCertificateProfile object.</span></span>

<span data-ttu-id="0a0a5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10XSCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-129">The following table shows the properties that are required when you create the windows10XSCEPCertificateProfile.</span></span>

|<span data-ttu-id="0a0a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a0a5-130">Property</span></span>|<span data-ttu-id="0a0a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a0a5-131">Type</span></span>|<span data-ttu-id="0a0a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a0a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a0a5-133">id</span><span class="sxs-lookup"><span data-stu-id="0a0a5-133">id</span></span>|<span data-ttu-id="0a0a5-134">String</span><span class="sxs-lookup"><span data-stu-id="0a0a5-134">String</span></span>|<span data-ttu-id="0a0a5-135">Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-136">versão</span><span class="sxs-lookup"><span data-stu-id="0a0a5-136">version</span></span>|<span data-ttu-id="0a0a5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0a0a5-137">Int32</span></span>|<span data-ttu-id="0a0a5-138">Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0a0a5-139">displayName</span></span>|<span data-ttu-id="0a0a5-140">String</span><span class="sxs-lookup"><span data-stu-id="0a0a5-140">String</span></span>|<span data-ttu-id="0a0a5-141">Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-142">description</span><span class="sxs-lookup"><span data-stu-id="0a0a5-142">description</span></span>|<span data-ttu-id="0a0a5-143">String</span><span class="sxs-lookup"><span data-stu-id="0a0a5-143">String</span></span>|<span data-ttu-id="0a0a5-144">Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-145">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="0a0a5-145">creationDateTime</span></span>|<span data-ttu-id="0a0a5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a0a5-146">DateTimeOffset</span></span>|<span data-ttu-id="0a0a5-147">O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a0a5-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0a0a5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a0a5-149">DateTimeOffset</span></span>|<span data-ttu-id="0a0a5-150">O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a0a5-151">roleScopeTagIds</span></span>|<span data-ttu-id="0a0a5-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0a5-152">String collection</span></span>|<span data-ttu-id="0a0a5-153">Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="0a0a5-154">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0a0a5-154">certificateStore</span></span>|[<span data-ttu-id="0a0a5-155">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0a0a5-155">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="0a0a5-156">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-156">Target store certificate.</span></span> <span data-ttu-id="0a0a5-157">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-157">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0a0a5-158">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0a0a5-158">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0a0a5-159">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0a0a5-159">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="0a0a5-160">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-160">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0a0a5-161">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-161">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0a0a5-162">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0a0a5-162">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0a0a5-163">Int32</span><span class="sxs-lookup"><span data-stu-id="0a0a5-163">Int32</span></span>|<span data-ttu-id="0a0a5-164">Valor para o período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="0a0a5-164">Value for the Certificate Validity Period</span></span>|
|<span data-ttu-id="0a0a5-165">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0a0a5-165">extendedKeyUsages</span></span>|<span data-ttu-id="0a0a5-166">coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0a0a5-167">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="0a0a5-167">Extended Key Usage (EKU) settings.</span></span>|
|<span data-ttu-id="0a0a5-168">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0a0a5-168">hashAlgorithm</span></span>|<span data-ttu-id="0a0a5-169">coleção [HashAlgorithm](../resources/intune-shared-hashalgorithms.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) collection</span></span>|<span data-ttu-id="0a0a5-170">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-170">SCEP Hash Algorithm.</span></span> <span data-ttu-id="0a0a5-171">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-171">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="0a0a5-172">keySize</span><span class="sxs-lookup"><span data-stu-id="0a0a5-172">keySize</span></span>|[<span data-ttu-id="0a0a5-173">keySize</span><span class="sxs-lookup"><span data-stu-id="0a0a5-173">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="0a0a5-174">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-174">SCEP Key Size.</span></span> <span data-ttu-id="0a0a5-175">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-175">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="0a0a5-176">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="0a0a5-176">keyStorageProvider</span></span>|[<span data-ttu-id="0a0a5-177">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="0a0a5-177">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="0a0a5-178">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="0a0a5-178">Key Storage Provider (KSP).</span></span> <span data-ttu-id="0a0a5-179">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-179">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="0a0a5-180">uso de</span><span class="sxs-lookup"><span data-stu-id="0a0a5-180">keyUsage</span></span>|[<span data-ttu-id="0a0a5-181">usos de</span><span class="sxs-lookup"><span data-stu-id="0a0a5-181">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="0a0a5-182">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-182">SCEP Key Usage.</span></span> <span data-ttu-id="0a0a5-183">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-183">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="0a0a5-184">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0a0a5-184">renewalThresholdPercentage</span></span>|<span data-ttu-id="0a0a5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0a0a5-185">Int32</span></span>|<span data-ttu-id="0a0a5-186">Porcentagem de limite de renovação de certificado</span><span class="sxs-lookup"><span data-stu-id="0a0a5-186">Certificate renewal threshold percentage</span></span>|
|<span data-ttu-id="0a0a5-187">rootCertificateId</span><span class="sxs-lookup"><span data-stu-id="0a0a5-187">rootCertificateId</span></span>|<span data-ttu-id="0a0a5-188">Guid</span><span class="sxs-lookup"><span data-stu-id="0a0a5-188">Guid</span></span>|<span data-ttu-id="0a0a5-189">ID de certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="0a0a5-189">Trusted Root Certificate ID</span></span>|
|<span data-ttu-id="0a0a5-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="0a0a5-190">scepServerUrls</span></span>|<span data-ttu-id="0a0a5-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0a5-191">String collection</span></span>|<span data-ttu-id="0a0a5-192">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="0a0a5-193">subjectAlternativeNameFormats</span><span class="sxs-lookup"><span data-stu-id="0a0a5-193">subjectAlternativeNameFormats</span></span>|<span data-ttu-id="0a0a5-194">coleção [windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a5-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) collection</span></span>|<span data-ttu-id="0a0a5-195">Atributos AAD personalizados.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-195">Custom AAD Attributes.</span></span>|
|<span data-ttu-id="0a0a5-196">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0a0a5-196">subjectNameFormatString</span></span>|<span data-ttu-id="0a0a5-197">String</span><span class="sxs-lookup"><span data-stu-id="0a0a5-197">String</span></span>|<span data-ttu-id="0a0a5-198">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-198">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="0a0a5-199">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="0a0a5-199">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|



## <a name="response"></a><span data-ttu-id="0a0a5-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a0a5-200">Response</span></span>
<span data-ttu-id="0a0a5-201">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-201">If successful, this method returns a `201 Created` response code and a [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a0a5-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a0a5-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a0a5-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a0a5-203">Request</span></span>
<span data-ttu-id="0a0a5-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a0a5-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a0a5-205">Response</span></span>
<span data-ttu-id="0a0a5-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a0a5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




