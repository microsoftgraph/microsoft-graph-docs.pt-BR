---
title: Criar userPFXCertificate
description: Crie um novo objeto userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f8b60d952f4d9ab8013636541a647a49ffdc05d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152247"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="cf4d6-103">Criar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="cf4d6-103">Create userPFXCertificate</span></span>

<span data-ttu-id="cf4d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf4d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf4d6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf4d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf4d6-107">Crie um novo [objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="cf4d6-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf4d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf4d6-108">Prerequisites</span></span>
<span data-ttu-id="cf4d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf4d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf4d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf4d6-111">Permission type</span></span>|<span data-ttu-id="cf4d6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf4d6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf4d6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf4d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf4d6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4d6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf4d6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf4d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf4d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-116">Not supported.</span></span>|
|<span data-ttu-id="cf4d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf4d6-117">Application</span></span>|<span data-ttu-id="cf4d6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4d6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf4d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf4d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="cf4d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf4d6-120">Request headers</span></span>
|<span data-ttu-id="cf4d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf4d6-121">Header</span></span>|<span data-ttu-id="cf4d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf4d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf4d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf4d6-123">Authorization</span></span>|<span data-ttu-id="cf4d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf4d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf4d6-125">Accept</span></span>|<span data-ttu-id="cf4d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf4d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf4d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf4d6-127">Request body</span></span>
<span data-ttu-id="cf4d6-128">No corpo da solicitação, fornece uma representação JSON para o objeto userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="cf4d6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="cf4d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf4d6-130">Property</span></span>|<span data-ttu-id="cf4d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf4d6-131">Type</span></span>|<span data-ttu-id="cf4d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf4d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf4d6-133">id</span><span class="sxs-lookup"><span data-stu-id="cf4d6-133">id</span></span>|<span data-ttu-id="cf4d6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf4d6-134">String</span></span>|<span data-ttu-id="cf4d6-135">Identificador exclusivo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="cf4d6-136">thumbprint</span><span class="sxs-lookup"><span data-stu-id="cf4d6-136">thumbprint</span></span>|<span data-ttu-id="cf4d6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf4d6-137">String</span></span>|<span data-ttu-id="cf4d6-138">Impressão digital SHA-1 do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="cf4d6-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="cf4d6-139">intendedPurpose</span></span>|[<span data-ttu-id="cf4d6-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="cf4d6-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="cf4d6-141">Finalidade pretendido do certificado do ponto de vista da implantação.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="cf4d6-142">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="cf4d6-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf4d6-143">userPrincipalName</span></span>|<span data-ttu-id="cf4d6-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf4d6-144">String</span></span>|<span data-ttu-id="cf4d6-145">Nome principal do usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="cf4d6-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cf4d6-146">startDateTime</span></span>|<span data-ttu-id="cf4d6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf4d6-147">DateTimeOffset</span></span>|<span data-ttu-id="cf4d6-148">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="cf4d6-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cf4d6-149">expirationDateTime</span></span>|<span data-ttu-id="cf4d6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf4d6-150">DateTimeOffset</span></span>|<span data-ttu-id="cf4d6-151">Data/hora de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="cf4d6-152">providerName</span><span class="sxs-lookup"><span data-stu-id="cf4d6-152">providerName</span></span>|<span data-ttu-id="cf4d6-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf4d6-153">String</span></span>|<span data-ttu-id="cf4d6-154">Provedor de criptografia usado para criptografar esse blob.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="cf4d6-155">keyName</span><span class="sxs-lookup"><span data-stu-id="cf4d6-155">keyName</span></span>|<span data-ttu-id="cf4d6-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf4d6-156">String</span></span>|<span data-ttu-id="cf4d6-157">Nome da chave (dentro do provedor) usada para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="cf4d6-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="cf4d6-158">paddingScheme</span></span>|[<span data-ttu-id="cf4d6-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="cf4d6-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="cf4d6-160">Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="cf4d6-161">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="cf4d6-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="cf4d6-162">encryptedPfxBlob</span></span>|<span data-ttu-id="cf4d6-163">Binário</span><span class="sxs-lookup"><span data-stu-id="cf4d6-163">Binary</span></span>|<span data-ttu-id="cf4d6-164">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="cf4d6-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="cf4d6-165">encryptedPfxPassword</span></span>|<span data-ttu-id="cf4d6-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf4d6-166">String</span></span>|<span data-ttu-id="cf4d6-167">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="cf4d6-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf4d6-168">createdDateTime</span></span>|<span data-ttu-id="cf4d6-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf4d6-169">DateTimeOffset</span></span>|<span data-ttu-id="cf4d6-170">Data/hora em que esse certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="cf4d6-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf4d6-171">lastModifiedDateTime</span></span>|<span data-ttu-id="cf4d6-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf4d6-172">DateTimeOffset</span></span>|<span data-ttu-id="cf4d6-173">Data/hora em que esse certificado PFX foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="cf4d6-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf4d6-174">Response</span></span>
<span data-ttu-id="cf4d6-175">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf4d6-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf4d6-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf4d6-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf4d6-177">Request</span></span>
<span data-ttu-id="cf4d6-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf4d6-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf4d6-179">Response</span></span>
<span data-ttu-id="cf4d6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf4d6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




