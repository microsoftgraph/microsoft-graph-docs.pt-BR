---
title: Atualizar userPFXCertificate
description: Atualiza as propriedades de um objeto userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d25087ef6ccd2bfbcd7b98baa674295653c0ca2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731138"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="71a8b-103">Atualizar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="71a8b-103">Update userPFXCertificate</span></span>

<span data-ttu-id="71a8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71a8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71a8b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71a8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71a8b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71a8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71a8b-107">Atualiza as propriedades de um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="71a8b-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71a8b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71a8b-108">Prerequisites</span></span>
<span data-ttu-id="71a8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71a8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71a8b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71a8b-111">Permission type</span></span>|<span data-ttu-id="71a8b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71a8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71a8b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71a8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71a8b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a8b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71a8b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71a8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71a8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71a8b-116">Not supported.</span></span>|
|<span data-ttu-id="71a8b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71a8b-117">Application</span></span>|<span data-ttu-id="71a8b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a8b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71a8b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71a8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="71a8b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71a8b-120">Request headers</span></span>
|<span data-ttu-id="71a8b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71a8b-121">Header</span></span>|<span data-ttu-id="71a8b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="71a8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71a8b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71a8b-123">Authorization</span></span>|<span data-ttu-id="71a8b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71a8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71a8b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71a8b-125">Accept</span></span>|<span data-ttu-id="71a8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71a8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71a8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71a8b-127">Request body</span></span>
<span data-ttu-id="71a8b-128">No corpo da solicitação, forneça uma representação JSON do objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="71a8b-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="71a8b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="71a8b-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="71a8b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71a8b-130">Property</span></span>|<span data-ttu-id="71a8b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71a8b-131">Type</span></span>|<span data-ttu-id="71a8b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71a8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71a8b-133">id</span><span class="sxs-lookup"><span data-stu-id="71a8b-133">id</span></span>|<span data-ttu-id="71a8b-134">String</span><span class="sxs-lookup"><span data-stu-id="71a8b-134">String</span></span>|<span data-ttu-id="71a8b-135">Identificador exclusivo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="71a8b-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="71a8b-136">identificação</span><span class="sxs-lookup"><span data-stu-id="71a8b-136">thumbprint</span></span>|<span data-ttu-id="71a8b-137">String</span><span class="sxs-lookup"><span data-stu-id="71a8b-137">String</span></span>|<span data-ttu-id="71a8b-138">Impressão digital SHA-1 do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="71a8b-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="71a8b-139">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="71a8b-139">intendedPurpose</span></span>|[<span data-ttu-id="71a8b-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="71a8b-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="71a8b-141">Finalidade do certificado do ponto de vista da implantação.</span><span class="sxs-lookup"><span data-stu-id="71a8b-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="71a8b-142">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="71a8b-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="71a8b-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="71a8b-143">userPrincipalName</span></span>|<span data-ttu-id="71a8b-144">String</span><span class="sxs-lookup"><span data-stu-id="71a8b-144">String</span></span>|<span data-ttu-id="71a8b-145">Nome principal de usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="71a8b-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="71a8b-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="71a8b-146">startDateTime</span></span>|<span data-ttu-id="71a8b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71a8b-147">DateTimeOffset</span></span>|<span data-ttu-id="71a8b-148">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="71a8b-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="71a8b-149">expirationDateTime</span></span>|<span data-ttu-id="71a8b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71a8b-150">DateTimeOffset</span></span>|<span data-ttu-id="71a8b-151">Data/hora de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="71a8b-152">providerName</span><span class="sxs-lookup"><span data-stu-id="71a8b-152">providerName</span></span>|<span data-ttu-id="71a8b-153">String</span><span class="sxs-lookup"><span data-stu-id="71a8b-153">String</span></span>|<span data-ttu-id="71a8b-154">Provedor de criptografia usado para criptografar este BLOB.</span><span class="sxs-lookup"><span data-stu-id="71a8b-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="71a8b-155">keyName</span><span class="sxs-lookup"><span data-stu-id="71a8b-155">keyName</span></span>|<span data-ttu-id="71a8b-156">String</span><span class="sxs-lookup"><span data-stu-id="71a8b-156">String</span></span>|<span data-ttu-id="71a8b-157">Nome da chave (dentro do provedor) usada para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="71a8b-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="71a8b-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="71a8b-158">paddingScheme</span></span>|[<span data-ttu-id="71a8b-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="71a8b-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="71a8b-160">Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia.</span><span class="sxs-lookup"><span data-stu-id="71a8b-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="71a8b-161">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="71a8b-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="71a8b-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="71a8b-162">encryptedPfxBlob</span></span>|<span data-ttu-id="71a8b-163">Binária</span><span class="sxs-lookup"><span data-stu-id="71a8b-163">Binary</span></span>|<span data-ttu-id="71a8b-164">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="71a8b-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="71a8b-165">encryptedPfxPassword</span></span>|<span data-ttu-id="71a8b-166">String</span><span class="sxs-lookup"><span data-stu-id="71a8b-166">String</span></span>|<span data-ttu-id="71a8b-167">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="71a8b-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="71a8b-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71a8b-168">createdDateTime</span></span>|<span data-ttu-id="71a8b-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71a8b-169">DateTimeOffset</span></span>|<span data-ttu-id="71a8b-170">Data/hora em que este certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="71a8b-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71a8b-171">lastModifiedDateTime</span></span>|<span data-ttu-id="71a8b-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71a8b-172">DateTimeOffset</span></span>|<span data-ttu-id="71a8b-173">Data/hora em que este certificado PFX foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="71a8b-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="71a8b-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="71a8b-174">Response</span></span>
<span data-ttu-id="71a8b-175">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71a8b-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71a8b-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71a8b-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="71a8b-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71a8b-177">Request</span></span>
<span data-ttu-id="71a8b-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71a8b-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
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

### <a name="response"></a><span data-ttu-id="71a8b-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="71a8b-179">Response</span></span>
<span data-ttu-id="71a8b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71a8b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





