---
title: Atualizar userPFXCertificate
description: Atualize as propriedades de um objeto userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 745faa38ded53e357cf78a56fcf0b4ab1b2298db
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152184"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="914ca-103">Atualizar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="914ca-103">Update userPFXCertificate</span></span>

<span data-ttu-id="914ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="914ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="914ca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="914ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="914ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="914ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="914ca-107">Atualize as propriedades de [um objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="914ca-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="914ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="914ca-108">Prerequisites</span></span>
<span data-ttu-id="914ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="914ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="914ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="914ca-111">Permission type</span></span>|<span data-ttu-id="914ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="914ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="914ca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="914ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="914ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="914ca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="914ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="914ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="914ca-116">Not supported.</span></span>|
|<span data-ttu-id="914ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="914ca-117">Application</span></span>|<span data-ttu-id="914ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="914ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="914ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="914ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="914ca-120">Request headers</span></span>
|<span data-ttu-id="914ca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="914ca-121">Header</span></span>|<span data-ttu-id="914ca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="914ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="914ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="914ca-123">Authorization</span></span>|<span data-ttu-id="914ca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="914ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="914ca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="914ca-125">Accept</span></span>|<span data-ttu-id="914ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="914ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="914ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="914ca-127">Request body</span></span>
<span data-ttu-id="914ca-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="914ca-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="914ca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="914ca-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="914ca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="914ca-130">Property</span></span>|<span data-ttu-id="914ca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="914ca-131">Type</span></span>|<span data-ttu-id="914ca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="914ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914ca-133">id</span><span class="sxs-lookup"><span data-stu-id="914ca-133">id</span></span>|<span data-ttu-id="914ca-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914ca-134">String</span></span>|<span data-ttu-id="914ca-135">Identificador exclusivo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="914ca-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="914ca-136">thumbprint</span><span class="sxs-lookup"><span data-stu-id="914ca-136">thumbprint</span></span>|<span data-ttu-id="914ca-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914ca-137">String</span></span>|<span data-ttu-id="914ca-138">Impressão digital SHA-1 do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="914ca-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="914ca-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="914ca-139">intendedPurpose</span></span>|[<span data-ttu-id="914ca-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="914ca-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="914ca-141">Finalidade pretendido do certificado do ponto de vista da implantação.</span><span class="sxs-lookup"><span data-stu-id="914ca-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="914ca-142">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="914ca-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="914ca-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="914ca-143">userPrincipalName</span></span>|<span data-ttu-id="914ca-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914ca-144">String</span></span>|<span data-ttu-id="914ca-145">Nome principal do usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="914ca-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="914ca-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="914ca-146">startDateTime</span></span>|<span data-ttu-id="914ca-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914ca-147">DateTimeOffset</span></span>|<span data-ttu-id="914ca-148">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="914ca-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="914ca-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="914ca-149">expirationDateTime</span></span>|<span data-ttu-id="914ca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914ca-150">DateTimeOffset</span></span>|<span data-ttu-id="914ca-151">Data/hora de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="914ca-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="914ca-152">providerName</span><span class="sxs-lookup"><span data-stu-id="914ca-152">providerName</span></span>|<span data-ttu-id="914ca-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914ca-153">String</span></span>|<span data-ttu-id="914ca-154">Provedor de criptografia usado para criptografar esse blob.</span><span class="sxs-lookup"><span data-stu-id="914ca-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="914ca-155">keyName</span><span class="sxs-lookup"><span data-stu-id="914ca-155">keyName</span></span>|<span data-ttu-id="914ca-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914ca-156">String</span></span>|<span data-ttu-id="914ca-157">Nome da chave (dentro do provedor) usada para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="914ca-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="914ca-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="914ca-158">paddingScheme</span></span>|[<span data-ttu-id="914ca-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="914ca-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="914ca-160">Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia.</span><span class="sxs-lookup"><span data-stu-id="914ca-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="914ca-161">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="914ca-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="914ca-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="914ca-162">encryptedPfxBlob</span></span>|<span data-ttu-id="914ca-163">Binário</span><span class="sxs-lookup"><span data-stu-id="914ca-163">Binary</span></span>|<span data-ttu-id="914ca-164">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="914ca-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="914ca-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="914ca-165">encryptedPfxPassword</span></span>|<span data-ttu-id="914ca-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914ca-166">String</span></span>|<span data-ttu-id="914ca-167">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="914ca-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="914ca-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="914ca-168">createdDateTime</span></span>|<span data-ttu-id="914ca-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914ca-169">DateTimeOffset</span></span>|<span data-ttu-id="914ca-170">Data/hora em que esse certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="914ca-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="914ca-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="914ca-171">lastModifiedDateTime</span></span>|<span data-ttu-id="914ca-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914ca-172">DateTimeOffset</span></span>|<span data-ttu-id="914ca-173">Data/hora em que esse certificado PFX foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="914ca-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="914ca-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="914ca-174">Response</span></span>
<span data-ttu-id="914ca-175">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="914ca-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="914ca-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="914ca-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="914ca-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="914ca-177">Request</span></span>
<span data-ttu-id="914ca-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="914ca-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="914ca-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="914ca-179">Response</span></span>
<span data-ttu-id="914ca-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="914ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




