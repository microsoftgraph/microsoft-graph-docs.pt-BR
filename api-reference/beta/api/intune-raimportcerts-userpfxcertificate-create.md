---
title: Criar userPFXCertificate
description: Criar um novo objeto userPFXCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b72b94a1ec89cd618665cce41c71c51488688d11
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801842"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="2fc23-103">Criar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="2fc23-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="2fc23-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2fc23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fc23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fc23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fc23-106">Criar um novo objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="2fc23-106">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fc23-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fc23-107">Prerequisites</span></span>
<span data-ttu-id="2fc23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fc23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fc23-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fc23-110">Permission type</span></span>|<span data-ttu-id="2fc23-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2fc23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fc23-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fc23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2fc23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fc23-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fc23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fc23-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fc23-115">Not supported.</span></span>|
|<span data-ttu-id="2fc23-116">Application</span><span class="sxs-lookup"><span data-stu-id="2fc23-116">Application</span></span>|<span data-ttu-id="2fc23-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc23-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fc23-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fc23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="2fc23-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc23-119">Request headers</span></span>
|<span data-ttu-id="2fc23-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fc23-120">Header</span></span>|<span data-ttu-id="2fc23-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2fc23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fc23-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fc23-122">Authorization</span></span>|<span data-ttu-id="2fc23-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fc23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fc23-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2fc23-124">Accept</span></span>|<span data-ttu-id="2fc23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2fc23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fc23-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc23-126">Request body</span></span>
<span data-ttu-id="2fc23-127">No corpo da solicitação, forneça uma representação JSON do objeto userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="2fc23-127">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="2fc23-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="2fc23-128">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="2fc23-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fc23-129">Property</span></span>|<span data-ttu-id="2fc23-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fc23-130">Type</span></span>|<span data-ttu-id="2fc23-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fc23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc23-132">id</span><span class="sxs-lookup"><span data-stu-id="2fc23-132">id</span></span>|<span data-ttu-id="2fc23-133">String</span><span class="sxs-lookup"><span data-stu-id="2fc23-133">String</span></span>|<span data-ttu-id="2fc23-134">Identificador exclusivo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="2fc23-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="2fc23-135">identificação</span><span class="sxs-lookup"><span data-stu-id="2fc23-135">thumbprint</span></span>|<span data-ttu-id="2fc23-136">String</span><span class="sxs-lookup"><span data-stu-id="2fc23-136">String</span></span>|<span data-ttu-id="2fc23-137">Impressão digital SHA-1 do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="2fc23-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="2fc23-138">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="2fc23-138">intendedPurpose</span></span>|[<span data-ttu-id="2fc23-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="2fc23-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="2fc23-140">Finalidade do certificado do ponto de vista da implantação.</span><span class="sxs-lookup"><span data-stu-id="2fc23-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="2fc23-141">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="2fc23-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="2fc23-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2fc23-142">userPrincipalName</span></span>|<span data-ttu-id="2fc23-143">String</span><span class="sxs-lookup"><span data-stu-id="2fc23-143">String</span></span>|<span data-ttu-id="2fc23-144">Nome principal de usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="2fc23-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="2fc23-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc23-145">startDateTime</span></span>|<span data-ttu-id="2fc23-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc23-146">DateTimeOffset</span></span>|<span data-ttu-id="2fc23-147">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="2fc23-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="2fc23-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc23-148">expirationDateTime</span></span>|<span data-ttu-id="2fc23-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc23-149">DateTimeOffset</span></span>|<span data-ttu-id="2fc23-150">Data/hora de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="2fc23-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="2fc23-151">providerName</span><span class="sxs-lookup"><span data-stu-id="2fc23-151">providerName</span></span>|<span data-ttu-id="2fc23-152">String</span><span class="sxs-lookup"><span data-stu-id="2fc23-152">String</span></span>|<span data-ttu-id="2fc23-153">Provedor de criptografia usado para criptografar este BLOB.</span><span class="sxs-lookup"><span data-stu-id="2fc23-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="2fc23-154">keyName</span><span class="sxs-lookup"><span data-stu-id="2fc23-154">keyName</span></span>|<span data-ttu-id="2fc23-155">String</span><span class="sxs-lookup"><span data-stu-id="2fc23-155">String</span></span>|<span data-ttu-id="2fc23-156">Nome da chave (dentro do provedor) usada para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="2fc23-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="2fc23-157">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="2fc23-157">paddingScheme</span></span>|[<span data-ttu-id="2fc23-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="2fc23-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="2fc23-159">Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia.</span><span class="sxs-lookup"><span data-stu-id="2fc23-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="2fc23-160">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="2fc23-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="2fc23-161">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="2fc23-161">encryptedPfxBlob</span></span>|<span data-ttu-id="2fc23-162">Binária</span><span class="sxs-lookup"><span data-stu-id="2fc23-162">Binary</span></span>|<span data-ttu-id="2fc23-163">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="2fc23-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="2fc23-164">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="2fc23-164">encryptedPfxPassword</span></span>|<span data-ttu-id="2fc23-165">String</span><span class="sxs-lookup"><span data-stu-id="2fc23-165">String</span></span>|<span data-ttu-id="2fc23-166">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="2fc23-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="2fc23-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc23-167">createdDateTime</span></span>|<span data-ttu-id="2fc23-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc23-168">DateTimeOffset</span></span>|<span data-ttu-id="2fc23-169">Data/hora em que este certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="2fc23-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="2fc23-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc23-170">lastModifiedDateTime</span></span>|<span data-ttu-id="2fc23-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc23-171">DateTimeOffset</span></span>|<span data-ttu-id="2fc23-172">Data/hora em que este certificado PFX foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2fc23-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2fc23-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fc23-173">Response</span></span>
<span data-ttu-id="2fc23-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fc23-174">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fc23-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fc23-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fc23-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc23-176">Request</span></span>
<span data-ttu-id="2fc23-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fc23-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fc23-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fc23-178">Response</span></span>
<span data-ttu-id="2fc23-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fc23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




