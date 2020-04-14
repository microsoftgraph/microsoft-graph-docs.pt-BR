---
title: Criar userPFXCertificate
description: Criar um novo objeto userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a22cdb432fac4bd6181a0ef5752661999cc1ef51
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437658"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="02661-103">Criar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="02661-103">Create userPFXCertificate</span></span>

<span data-ttu-id="02661-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02661-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02661-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02661-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02661-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02661-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02661-107">Criar um novo objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="02661-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02661-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02661-108">Prerequisites</span></span>
<span data-ttu-id="02661-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02661-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02661-111">Permission type</span></span>|<span data-ttu-id="02661-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02661-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02661-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02661-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02661-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02661-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02661-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02661-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02661-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02661-116">Not supported.</span></span>|
|<span data-ttu-id="02661-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02661-117">Application</span></span>|<span data-ttu-id="02661-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02661-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02661-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02661-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="02661-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02661-120">Request headers</span></span>
|<span data-ttu-id="02661-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02661-121">Header</span></span>|<span data-ttu-id="02661-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02661-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02661-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02661-123">Authorization</span></span>|<span data-ttu-id="02661-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02661-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02661-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02661-125">Accept</span></span>|<span data-ttu-id="02661-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02661-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02661-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02661-127">Request body</span></span>
<span data-ttu-id="02661-128">No corpo da solicitação, forneça uma representação JSON do objeto userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="02661-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="02661-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="02661-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="02661-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02661-130">Property</span></span>|<span data-ttu-id="02661-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02661-131">Type</span></span>|<span data-ttu-id="02661-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02661-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02661-133">id</span><span class="sxs-lookup"><span data-stu-id="02661-133">id</span></span>|<span data-ttu-id="02661-134">String</span><span class="sxs-lookup"><span data-stu-id="02661-134">String</span></span>|<span data-ttu-id="02661-135">Identificador exclusivo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="02661-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="02661-136">identificação</span><span class="sxs-lookup"><span data-stu-id="02661-136">thumbprint</span></span>|<span data-ttu-id="02661-137">String</span><span class="sxs-lookup"><span data-stu-id="02661-137">String</span></span>|<span data-ttu-id="02661-138">Impressão digital SHA-1 do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="02661-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="02661-139">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="02661-139">intendedPurpose</span></span>|[<span data-ttu-id="02661-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="02661-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="02661-141">Finalidade do certificado do ponto de vista da implantação.</span><span class="sxs-lookup"><span data-stu-id="02661-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="02661-142">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="02661-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="02661-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02661-143">userPrincipalName</span></span>|<span data-ttu-id="02661-144">String</span><span class="sxs-lookup"><span data-stu-id="02661-144">String</span></span>|<span data-ttu-id="02661-145">Nome principal de usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="02661-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="02661-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="02661-146">startDateTime</span></span>|<span data-ttu-id="02661-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02661-147">DateTimeOffset</span></span>|<span data-ttu-id="02661-148">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="02661-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="02661-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="02661-149">expirationDateTime</span></span>|<span data-ttu-id="02661-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02661-150">DateTimeOffset</span></span>|<span data-ttu-id="02661-151">Data/hora de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="02661-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="02661-152">providerName</span><span class="sxs-lookup"><span data-stu-id="02661-152">providerName</span></span>|<span data-ttu-id="02661-153">String</span><span class="sxs-lookup"><span data-stu-id="02661-153">String</span></span>|<span data-ttu-id="02661-154">Provedor de criptografia usado para criptografar este BLOB.</span><span class="sxs-lookup"><span data-stu-id="02661-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="02661-155">keyName</span><span class="sxs-lookup"><span data-stu-id="02661-155">keyName</span></span>|<span data-ttu-id="02661-156">String</span><span class="sxs-lookup"><span data-stu-id="02661-156">String</span></span>|<span data-ttu-id="02661-157">Nome da chave (dentro do provedor) usada para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="02661-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="02661-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="02661-158">paddingScheme</span></span>|[<span data-ttu-id="02661-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="02661-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="02661-160">Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia.</span><span class="sxs-lookup"><span data-stu-id="02661-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="02661-161">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="02661-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="02661-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="02661-162">encryptedPfxBlob</span></span>|<span data-ttu-id="02661-163">Binária</span><span class="sxs-lookup"><span data-stu-id="02661-163">Binary</span></span>|<span data-ttu-id="02661-164">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="02661-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="02661-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="02661-165">encryptedPfxPassword</span></span>|<span data-ttu-id="02661-166">String</span><span class="sxs-lookup"><span data-stu-id="02661-166">String</span></span>|<span data-ttu-id="02661-167">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="02661-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="02661-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02661-168">createdDateTime</span></span>|<span data-ttu-id="02661-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02661-169">DateTimeOffset</span></span>|<span data-ttu-id="02661-170">Data/hora em que este certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="02661-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="02661-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02661-171">lastModifiedDateTime</span></span>|<span data-ttu-id="02661-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02661-172">DateTimeOffset</span></span>|<span data-ttu-id="02661-173">Data/hora em que este certificado PFX foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="02661-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="02661-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="02661-174">Response</span></span>
<span data-ttu-id="02661-175">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02661-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02661-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02661-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="02661-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02661-177">Request</span></span>
<span data-ttu-id="02661-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02661-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02661-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="02661-179">Response</span></span>
<span data-ttu-id="02661-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02661-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



