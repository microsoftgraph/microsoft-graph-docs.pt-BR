---
title: Criar userPFXCertificate
description: Crie um novo objeto de userPFXCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8896e3bb300507f0d1a89892852a2e1d4865d9b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418166"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="06a11-103">Criar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="06a11-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="06a11-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="06a11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06a11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06a11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06a11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="06a11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06a11-107">Crie um novo objeto de [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="06a11-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06a11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06a11-108">Prerequisites</span></span>
<span data-ttu-id="06a11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="06a11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06a11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06a11-111">Permission type</span></span>|<span data-ttu-id="06a11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06a11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06a11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06a11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06a11-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a11-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06a11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06a11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06a11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06a11-116">Not supported.</span></span>|
|<span data-ttu-id="06a11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a11-117">Application</span></span>|<span data-ttu-id="06a11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06a11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06a11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06a11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="06a11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06a11-120">Request headers</span></span>
|<span data-ttu-id="06a11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06a11-121">Header</span></span>|<span data-ttu-id="06a11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06a11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06a11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06a11-123">Authorization</span></span>|<span data-ttu-id="06a11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06a11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06a11-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06a11-125">Accept</span></span>|<span data-ttu-id="06a11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06a11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06a11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06a11-127">Request body</span></span>
<span data-ttu-id="06a11-128">No corpo da solicitação, fornece uma representação JSON para o objeto userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="06a11-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="06a11-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="06a11-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="06a11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06a11-130">Property</span></span>|<span data-ttu-id="06a11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06a11-131">Type</span></span>|<span data-ttu-id="06a11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06a11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06a11-133">id</span><span class="sxs-lookup"><span data-stu-id="06a11-133">id</span></span>|<span data-ttu-id="06a11-134">String</span><span class="sxs-lookup"><span data-stu-id="06a11-134">String</span></span>|<span data-ttu-id="06a11-135">Identificador exclusivo para o certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="06a11-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="06a11-136">impressão digital</span><span class="sxs-lookup"><span data-stu-id="06a11-136">thumbprint</span></span>|<span data-ttu-id="06a11-137">String</span><span class="sxs-lookup"><span data-stu-id="06a11-137">String</span></span>|<span data-ttu-id="06a11-138">SHA-1 impressão digital do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="06a11-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="06a11-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="06a11-139">intendedPurpose</span></span>|[<span data-ttu-id="06a11-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="06a11-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="06a11-141">Destinada a finalidade do ponto de vista da implantação do certificado.</span><span class="sxs-lookup"><span data-stu-id="06a11-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="06a11-142">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="06a11-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="06a11-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06a11-143">userPrincipalName</span></span>|<span data-ttu-id="06a11-144">String</span><span class="sxs-lookup"><span data-stu-id="06a11-144">String</span></span>|<span data-ttu-id="06a11-145">Nome Principal de usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="06a11-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="06a11-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06a11-146">startDateTime</span></span>|<span data-ttu-id="06a11-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a11-147">DateTimeOffset</span></span>|<span data-ttu-id="06a11-148">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="06a11-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="06a11-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="06a11-149">expirationDateTime</span></span>|<span data-ttu-id="06a11-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a11-150">DateTimeOffset</span></span>|<span data-ttu-id="06a11-151">Data de expiração de validade/hora do certificado.</span><span class="sxs-lookup"><span data-stu-id="06a11-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="06a11-152">providerName</span><span class="sxs-lookup"><span data-stu-id="06a11-152">providerName</span></span>|<span data-ttu-id="06a11-153">String</span><span class="sxs-lookup"><span data-stu-id="06a11-153">String</span></span>|<span data-ttu-id="06a11-154">Provedor de criptografia usado para criptografar essa blob.</span><span class="sxs-lookup"><span data-stu-id="06a11-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="06a11-155">nome chave</span><span class="sxs-lookup"><span data-stu-id="06a11-155">keyName</span></span>|<span data-ttu-id="06a11-156">String</span><span class="sxs-lookup"><span data-stu-id="06a11-156">String</span></span>|<span data-ttu-id="06a11-157">Nome da chave (dentro do provedor) usado para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="06a11-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="06a11-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="06a11-158">paddingScheme</span></span>|[<span data-ttu-id="06a11-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="06a11-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="06a11-160">Esquema usado pelo provedor durante a criptografia/descriptografia de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="06a11-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="06a11-161">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="06a11-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="06a11-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="06a11-162">encryptedPfxBlob</span></span>|<span data-ttu-id="06a11-163">Binária</span><span class="sxs-lookup"><span data-stu-id="06a11-163">Binary</span></span>|<span data-ttu-id="06a11-164">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="06a11-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="06a11-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="06a11-165">encryptedPfxPassword</span></span>|<span data-ttu-id="06a11-166">String</span><span class="sxs-lookup"><span data-stu-id="06a11-166">String</span></span>|<span data-ttu-id="06a11-167">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="06a11-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="06a11-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06a11-168">createdDateTime</span></span>|<span data-ttu-id="06a11-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a11-169">DateTimeOffset</span></span>|<span data-ttu-id="06a11-170">Data/hora quando esse certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="06a11-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="06a11-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06a11-171">lastModifiedDateTime</span></span>|<span data-ttu-id="06a11-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a11-172">DateTimeOffset</span></span>|<span data-ttu-id="06a11-173">Data/hora da última modificação desse certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="06a11-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="06a11-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a11-174">Response</span></span>
<span data-ttu-id="06a11-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06a11-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a11-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06a11-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="06a11-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06a11-177">Request</span></span>
<span data-ttu-id="06a11-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06a11-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06a11-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a11-179">Response</span></span>
<span data-ttu-id="06a11-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06a11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




