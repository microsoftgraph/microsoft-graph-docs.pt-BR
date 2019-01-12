---
title: Atualizar userPFXCertificate
description: Atualize as propriedades de um objeto userPFXCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47d0ad37abed0a6cca231890be06c7b5666b3371
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913244"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="3c93e-103">Atualizar userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="3c93e-103">Update userPFXCertificate</span></span>

> <span data-ttu-id="3c93e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c93e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c93e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c93e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c93e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c93e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c93e-107">Atualize as propriedades de um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="3c93e-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c93e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c93e-108">Prerequisites</span></span>
<span data-ttu-id="3c93e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c93e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c93e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c93e-111">Permission type</span></span>|<span data-ttu-id="3c93e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c93e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c93e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c93e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c93e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c93e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c93e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c93e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c93e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c93e-116">Not supported.</span></span>|
|<span data-ttu-id="3c93e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c93e-117">Application</span></span>|<span data-ttu-id="3c93e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c93e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c93e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c93e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="3c93e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c93e-120">Request headers</span></span>
|<span data-ttu-id="3c93e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c93e-121">Header</span></span>|<span data-ttu-id="3c93e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c93e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c93e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c93e-123">Authorization</span></span>|<span data-ttu-id="3c93e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c93e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c93e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c93e-125">Accept</span></span>|<span data-ttu-id="3c93e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c93e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c93e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c93e-127">Request body</span></span>
<span data-ttu-id="3c93e-128">No corpo da solicitação, fornece uma representação JSON para o objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="3c93e-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="3c93e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="3c93e-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="3c93e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c93e-130">Property</span></span>|<span data-ttu-id="3c93e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c93e-131">Type</span></span>|<span data-ttu-id="3c93e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c93e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c93e-133">id</span><span class="sxs-lookup"><span data-stu-id="3c93e-133">id</span></span>|<span data-ttu-id="3c93e-134">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-134">String</span></span>|<span data-ttu-id="3c93e-135">Identificador exclusivo para o certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="3c93e-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="3c93e-136">impressão digital</span><span class="sxs-lookup"><span data-stu-id="3c93e-136">thumbprint</span></span>|<span data-ttu-id="3c93e-137">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-137">String</span></span>|<span data-ttu-id="3c93e-138">SHA-1 impressão digital do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="3c93e-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="3c93e-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3c93e-139">intendedPurpose</span></span>|[<span data-ttu-id="3c93e-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3c93e-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="3c93e-141">Destinada a finalidade do ponto de vista da implantação do certificado.</span><span class="sxs-lookup"><span data-stu-id="3c93e-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="3c93e-142">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="3c93e-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="3c93e-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3c93e-143">userPrincipalName</span></span>|<span data-ttu-id="3c93e-144">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-144">String</span></span>|<span data-ttu-id="3c93e-145">Nome Principal de usuário do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="3c93e-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="3c93e-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3c93e-146">startDateTime</span></span>|<span data-ttu-id="3c93e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c93e-147">DateTimeOffset</span></span>|<span data-ttu-id="3c93e-148">Data/hora de início da validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3c93e-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="3c93e-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3c93e-149">expirationDateTime</span></span>|<span data-ttu-id="3c93e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c93e-150">DateTimeOffset</span></span>|<span data-ttu-id="3c93e-151">Data de expiração de validade/hora do certificado.</span><span class="sxs-lookup"><span data-stu-id="3c93e-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="3c93e-152">providerName</span><span class="sxs-lookup"><span data-stu-id="3c93e-152">providerName</span></span>|<span data-ttu-id="3c93e-153">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-153">String</span></span>|<span data-ttu-id="3c93e-154">Provedor de criptografia usado para criptografar essa blob.</span><span class="sxs-lookup"><span data-stu-id="3c93e-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="3c93e-155">nome chave</span><span class="sxs-lookup"><span data-stu-id="3c93e-155">keyName</span></span>|<span data-ttu-id="3c93e-156">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-156">String</span></span>|<span data-ttu-id="3c93e-157">Nome da chave (dentro do provedor) usado para criptografar o blob.</span><span class="sxs-lookup"><span data-stu-id="3c93e-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="3c93e-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="3c93e-158">paddingScheme</span></span>|[<span data-ttu-id="3c93e-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="3c93e-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="3c93e-160">Esquema usado pelo provedor durante a criptografia/descriptografia de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="3c93e-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="3c93e-161">Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="3c93e-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="3c93e-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="3c93e-162">encryptedPfxBlob</span></span>|<span data-ttu-id="3c93e-163">Binária</span><span class="sxs-lookup"><span data-stu-id="3c93e-163">Binary</span></span>|<span data-ttu-id="3c93e-164">Blob PFX criptografado.</span><span class="sxs-lookup"><span data-stu-id="3c93e-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="3c93e-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="3c93e-165">encryptedPfxPassword</span></span>|<span data-ttu-id="3c93e-166">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-166">String</span></span>|<span data-ttu-id="3c93e-167">Senha PFX criptografada.</span><span class="sxs-lookup"><span data-stu-id="3c93e-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="3c93e-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c93e-168">createdDateTime</span></span>|<span data-ttu-id="3c93e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c93e-169">DateTimeOffset</span></span>|<span data-ttu-id="3c93e-170">Data/hora quando esse certificado PFX foi importado.</span><span class="sxs-lookup"><span data-stu-id="3c93e-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="3c93e-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c93e-171">lastModifiedDateTime</span></span>|<span data-ttu-id="3c93e-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c93e-172">DateTimeOffset</span></span>|<span data-ttu-id="3c93e-173">Data/hora da última modificação desse certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="3c93e-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3c93e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c93e-174">Response</span></span>
<span data-ttu-id="3c93e-175">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c93e-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c93e-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c93e-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c93e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c93e-177">Request</span></span>
<span data-ttu-id="3c93e-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c93e-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 530

{
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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3c93e-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c93e-179">Response</span></span>
<span data-ttu-id="3c93e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c93e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





