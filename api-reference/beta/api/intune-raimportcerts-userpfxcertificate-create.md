---
title: Criar userPFXCertificate
description: Criar um novo objeto userPFXCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10fa84321b9ebc4a3e1c5b78d338b955ae3261e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988794"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="ad89a-103">Criar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="ad89a-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="ad89a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad89a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad89a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad89a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad89a-106">Criar um novo objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ad89a-106">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad89a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad89a-107">Prerequisites</span></span>
<span data-ttu-id="ad89a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad89a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad89a-110">Permission type</span></span>|<span data-ttu-id="ad89a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad89a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad89a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad89a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad89a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad89a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad89a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad89a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad89a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad89a-115">Not supported.</span></span>|
|<span data-ttu-id="ad89a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad89a-116">Application</span></span>|<span data-ttu-id="ad89a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad89a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad89a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad89a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ad89a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad89a-119">Request headers</span></span>
|<span data-ttu-id="ad89a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad89a-120">Header</span></span>|<span data-ttu-id="ad89a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ad89a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad89a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad89a-122">Authorization</span></span>|<span data-ttu-id="ad89a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad89a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad89a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad89a-124">Accept</span></span>|<span data-ttu-id="ad89a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad89a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad89a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad89a-126">Request body</span></span>
<span data-ttu-id="ad89a-127">No corpo da solicitação, forneça uma representação JSON do objeto userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="ad89a-127">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="ad89a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="ad89a-128">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="ad89a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad89a-129">Property</span></span>|<span data-ttu-id="ad89a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad89a-130">Type</span></span>|<span data-ttu-id="ad89a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad89a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad89a-132">id</span><span class="sxs-lookup"><span data-stu-id="ad89a-132">id</span></span>|<span data-ttu-id="ad89a-133">String</span><span class="sxs-lookup"><span data-stu-id="ad89a-133">String</span></span>|<span data-ttu-id="ad89a-134">Identificador exclusivo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="ad89a-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="ad89a-135">identificação</span><span class="sxs-lookup"><span data-stu-id="ad89a-135">thumbprint</span></span>|<span data-ttu-id="ad89a-136">String</span><span class="sxs-lookup"><span data-stu-id="ad89a-136">String</span></span>|<span data-ttu-id="ad89a-137">Impressão digital SHA-1 do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="ad89a-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="ad89a-138">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="ad89a-138">intendedPurpose</span></span>|[<span data-ttu-id="ad89a-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ad89a-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="ad89a-140">Finalidade do certificado do ponto de vista da implantação.</span><span class="sxs-lookup"><span data-stu-id="ad89a-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="ad89a-141">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="ad89a-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="ad89a-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad89a-142">userPrincipalName</span></span>|<span data-ttu-id="ad89a-143">String</span><span class="sxs-lookup"><span data-stu-id="ad89a-143">String</span></span>|<span data-ttu-id="ad89a-144">Nome principal de usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="ad89a-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="ad89a-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ad89a-145">startDateTime</span></span>|<span data-ttu-id="ad89a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad89a-146">DateTimeOffset</span></span>|<span data-ttu-id="ad89a-147">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ad89a-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="ad89a-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ad89a-148">expirationDateTime</span></span>|<span data-ttu-id="ad89a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad89a-149">DateTimeOffset</span></span>|<span data-ttu-id="ad89a-150">Data/hora de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ad89a-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="ad89a-151">providerName</span><span class="sxs-lookup"><span data-stu-id="ad89a-151">providerName</span></span>|<span data-ttu-id="ad89a-152">String</span><span class="sxs-lookup"><span data-stu-id="ad89a-152">String</span></span>|<span data-ttu-id="ad89a-153">Provedor de criptografia usado para criptografar este BLOB.</span><span class="sxs-lookup"><span data-stu-id="ad89a-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="ad89a-154">keyName</span><span class="sxs-lookup"><span data-stu-id="ad89a-154">keyName</span></span>|<span data-ttu-id="ad89a-155">String</span><span class="sxs-lookup"><span data-stu-id="ad89a-155">String</span></span>|<span data-ttu-id="ad89a-156">Nome da chave (dentro do provedor) usada para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="ad89a-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="ad89a-157">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="ad89a-157">paddingScheme</span></span>|[<span data-ttu-id="ad89a-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="ad89a-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="ad89a-159">Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia.</span><span class="sxs-lookup"><span data-stu-id="ad89a-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="ad89a-160">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="ad89a-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="ad89a-161">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="ad89a-161">encryptedPfxBlob</span></span>|<span data-ttu-id="ad89a-162">Binária</span><span class="sxs-lookup"><span data-stu-id="ad89a-162">Binary</span></span>|<span data-ttu-id="ad89a-163">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="ad89a-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="ad89a-164">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="ad89a-164">encryptedPfxPassword</span></span>|<span data-ttu-id="ad89a-165">String</span><span class="sxs-lookup"><span data-stu-id="ad89a-165">String</span></span>|<span data-ttu-id="ad89a-166">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="ad89a-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="ad89a-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad89a-167">createdDateTime</span></span>|<span data-ttu-id="ad89a-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad89a-168">DateTimeOffset</span></span>|<span data-ttu-id="ad89a-169">Data/hora em que este certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="ad89a-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="ad89a-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad89a-170">lastModifiedDateTime</span></span>|<span data-ttu-id="ad89a-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad89a-171">DateTimeOffset</span></span>|<span data-ttu-id="ad89a-172">Data/hora em que este certificado PFX foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ad89a-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ad89a-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad89a-173">Response</span></span>
<span data-ttu-id="ad89a-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad89a-174">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad89a-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad89a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad89a-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad89a-176">Request</span></span>
<span data-ttu-id="ad89a-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad89a-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 523

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### <a name="response"></a><span data-ttu-id="ad89a-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad89a-178">Response</span></span>
<span data-ttu-id="ad89a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad89a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "045c159b-159b-045c-9b15-5c049b155c04",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





