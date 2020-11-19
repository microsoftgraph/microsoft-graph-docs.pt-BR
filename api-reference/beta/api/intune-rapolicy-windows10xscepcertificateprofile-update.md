---
title: Atualizar windows10XSCEPCertificateProfile
description: Atualiza as propriedades de um objeto windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a534517625466753f3f11adcc2a2424394d92887
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241300"
---
# <a name="update-windows10xscepcertificateprofile"></a><span data-ttu-id="89846-103">Atualizar windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="89846-103">Update windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="89846-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89846-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89846-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89846-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89846-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89846-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89846-107">Atualiza as propriedades de um objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="89846-107">Update the properties of a [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89846-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89846-108">Prerequisites</span></span>
<span data-ttu-id="89846-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89846-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89846-111">Permission type</span></span>|<span data-ttu-id="89846-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89846-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89846-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89846-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89846-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89846-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="89846-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89846-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89846-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89846-116">Not supported.</span></span>|
|<span data-ttu-id="89846-117">Application</span><span class="sxs-lookup"><span data-stu-id="89846-117">Application</span></span>|<span data-ttu-id="89846-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89846-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89846-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89846-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="89846-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89846-120">Request headers</span></span>
|<span data-ttu-id="89846-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89846-121">Header</span></span>|<span data-ttu-id="89846-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89846-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89846-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89846-123">Authorization</span></span>|<span data-ttu-id="89846-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89846-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89846-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89846-125">Accept</span></span>|<span data-ttu-id="89846-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89846-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89846-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89846-127">Request body</span></span>
<span data-ttu-id="89846-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="89846-128">In the request body, supply a JSON representation for the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="89846-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="89846-129">The following table shows the properties that are required when you create the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md).</span></span>

|<span data-ttu-id="89846-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89846-130">Property</span></span>|<span data-ttu-id="89846-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89846-131">Type</span></span>|<span data-ttu-id="89846-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89846-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89846-133">id</span><span class="sxs-lookup"><span data-stu-id="89846-133">id</span></span>|<span data-ttu-id="89846-134">String</span><span class="sxs-lookup"><span data-stu-id="89846-134">String</span></span>|<span data-ttu-id="89846-135">Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-136">versão</span><span class="sxs-lookup"><span data-stu-id="89846-136">version</span></span>|<span data-ttu-id="89846-137">Int32</span><span class="sxs-lookup"><span data-stu-id="89846-137">Int32</span></span>|<span data-ttu-id="89846-138">Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-139">displayName</span><span class="sxs-lookup"><span data-stu-id="89846-139">displayName</span></span>|<span data-ttu-id="89846-140">String</span><span class="sxs-lookup"><span data-stu-id="89846-140">String</span></span>|<span data-ttu-id="89846-141">Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-142">description</span><span class="sxs-lookup"><span data-stu-id="89846-142">description</span></span>|<span data-ttu-id="89846-143">String</span><span class="sxs-lookup"><span data-stu-id="89846-143">String</span></span>|<span data-ttu-id="89846-144">Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-145">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="89846-145">creationDateTime</span></span>|<span data-ttu-id="89846-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89846-146">DateTimeOffset</span></span>|<span data-ttu-id="89846-147">O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89846-148">lastModifiedDateTime</span></span>|<span data-ttu-id="89846-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89846-149">DateTimeOffset</span></span>|<span data-ttu-id="89846-150">O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89846-151">roleScopeTagIds</span></span>|<span data-ttu-id="89846-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="89846-152">String collection</span></span>|<span data-ttu-id="89846-153">Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89846-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="89846-154">certificateStore</span><span class="sxs-lookup"><span data-stu-id="89846-154">certificateStore</span></span>|[<span data-ttu-id="89846-155">certificateStore</span><span class="sxs-lookup"><span data-stu-id="89846-155">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="89846-156">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="89846-156">Target store certificate.</span></span> <span data-ttu-id="89846-157">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="89846-157">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="89846-158">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89846-158">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="89846-159">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89846-159">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="89846-160">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="89846-160">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="89846-161">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="89846-161">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="89846-162">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="89846-162">certificateValidityPeriodValue</span></span>|<span data-ttu-id="89846-163">Int32</span><span class="sxs-lookup"><span data-stu-id="89846-163">Int32</span></span>|<span data-ttu-id="89846-164">Valor para o período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="89846-164">Value for the Certificate Validity Period</span></span>|
|<span data-ttu-id="89846-165">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="89846-165">extendedKeyUsages</span></span>|<span data-ttu-id="89846-166">coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="89846-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="89846-167">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="89846-167">Extended Key Usage (EKU) settings.</span></span>|
|<span data-ttu-id="89846-168">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="89846-168">hashAlgorithm</span></span>|<span data-ttu-id="89846-169">coleção [HashAlgorithm](../resources/intune-shared-hashalgorithms.md)</span><span class="sxs-lookup"><span data-stu-id="89846-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) collection</span></span>|<span data-ttu-id="89846-170">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="89846-170">SCEP Hash Algorithm.</span></span> <span data-ttu-id="89846-171">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="89846-171">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="89846-172">keySize</span><span class="sxs-lookup"><span data-stu-id="89846-172">keySize</span></span>|[<span data-ttu-id="89846-173">keySize</span><span class="sxs-lookup"><span data-stu-id="89846-173">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="89846-174">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="89846-174">SCEP Key Size.</span></span> <span data-ttu-id="89846-175">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="89846-175">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="89846-176">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="89846-176">keyStorageProvider</span></span>|[<span data-ttu-id="89846-177">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="89846-177">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="89846-178">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="89846-178">Key Storage Provider (KSP).</span></span> <span data-ttu-id="89846-179">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="89846-179">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="89846-180">uso de</span><span class="sxs-lookup"><span data-stu-id="89846-180">keyUsage</span></span>|[<span data-ttu-id="89846-181">usos de</span><span class="sxs-lookup"><span data-stu-id="89846-181">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="89846-182">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="89846-182">SCEP Key Usage.</span></span> <span data-ttu-id="89846-183">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="89846-183">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="89846-184">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="89846-184">renewalThresholdPercentage</span></span>|<span data-ttu-id="89846-185">Int32</span><span class="sxs-lookup"><span data-stu-id="89846-185">Int32</span></span>|<span data-ttu-id="89846-186">Porcentagem de limite de renovação de certificado</span><span class="sxs-lookup"><span data-stu-id="89846-186">Certificate renewal threshold percentage</span></span>|
|<span data-ttu-id="89846-187">rootCertificateId</span><span class="sxs-lookup"><span data-stu-id="89846-187">rootCertificateId</span></span>|<span data-ttu-id="89846-188">Guid</span><span class="sxs-lookup"><span data-stu-id="89846-188">Guid</span></span>|<span data-ttu-id="89846-189">ID de certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="89846-189">Trusted Root Certificate ID</span></span>|
|<span data-ttu-id="89846-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="89846-190">scepServerUrls</span></span>|<span data-ttu-id="89846-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="89846-191">String collection</span></span>|<span data-ttu-id="89846-192">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="89846-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="89846-193">subjectAlternativeNameFormats</span><span class="sxs-lookup"><span data-stu-id="89846-193">subjectAlternativeNameFormats</span></span>|<span data-ttu-id="89846-194">coleção [windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="89846-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) collection</span></span>|<span data-ttu-id="89846-195">Atributos AAD personalizados.</span><span class="sxs-lookup"><span data-stu-id="89846-195">Custom AAD Attributes.</span></span>|
|<span data-ttu-id="89846-196">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="89846-196">subjectNameFormatString</span></span>|<span data-ttu-id="89846-197">String</span><span class="sxs-lookup"><span data-stu-id="89846-197">String</span></span>|<span data-ttu-id="89846-198">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="89846-198">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="89846-199">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="89846-199">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|



## <a name="response"></a><span data-ttu-id="89846-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="89846-200">Response</span></span>
<span data-ttu-id="89846-201">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89846-201">If successful, this method returns a `200 OK` response code and an updated [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89846-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89846-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="89846-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89846-203">Request</span></span>
<span data-ttu-id="89846-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89846-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
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

### <a name="response"></a><span data-ttu-id="89846-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="89846-205">Response</span></span>
<span data-ttu-id="89846-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89846-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




