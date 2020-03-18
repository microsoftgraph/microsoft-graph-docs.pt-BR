---
title: Criar pfxUserCertificate
description: Criar um novo objeto pfxUserCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b320c1d7893fabc824ec3c5c6a456df3bc45b26
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801877"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="a15e7-103">Criar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="a15e7-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="a15e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a15e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a15e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a15e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a15e7-106">Criar um novo objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="a15e7-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a15e7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a15e7-107">Prerequisites</span></span>
<span data-ttu-id="a15e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a15e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a15e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a15e7-110">Permission type</span></span>|<span data-ttu-id="a15e7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a15e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a15e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a15e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a15e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a15e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a15e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a15e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a15e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a15e7-115">Not supported.</span></span>|
|<span data-ttu-id="a15e7-116">Application</span><span class="sxs-lookup"><span data-stu-id="a15e7-116">Application</span></span>|<span data-ttu-id="a15e7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a15e7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a15e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a15e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="a15e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a15e7-119">Request headers</span></span>
|<span data-ttu-id="a15e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a15e7-120">Header</span></span>|<span data-ttu-id="a15e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a15e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a15e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a15e7-122">Authorization</span></span>|<span data-ttu-id="a15e7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a15e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a15e7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a15e7-124">Accept</span></span>|<span data-ttu-id="a15e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a15e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a15e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a15e7-126">Request body</span></span>
<span data-ttu-id="a15e7-127">No corpo da solicitação, forneça uma representação JSON do objeto pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="a15e7-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="a15e7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="a15e7-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="a15e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a15e7-129">Property</span></span>|<span data-ttu-id="a15e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a15e7-130">Type</span></span>|<span data-ttu-id="a15e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a15e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a15e7-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="a15e7-132">tenantId</span></span>|<span data-ttu-id="a15e7-133">Guid</span><span class="sxs-lookup"><span data-stu-id="a15e7-133">Guid</span></span>|<span data-ttu-id="a15e7-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-134">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-135">userId</span><span class="sxs-lookup"><span data-stu-id="a15e7-135">userId</span></span>|<span data-ttu-id="a15e7-136">Guid</span><span class="sxs-lookup"><span data-stu-id="a15e7-136">Guid</span></span>|<span data-ttu-id="a15e7-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-137">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-138">identificação</span><span class="sxs-lookup"><span data-stu-id="a15e7-138">thumbprint</span></span>|<span data-ttu-id="a15e7-139">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-139">String</span></span>|<span data-ttu-id="a15e7-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-140">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="a15e7-141">userUpn</span></span>|<span data-ttu-id="a15e7-142">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-142">String</span></span>|<span data-ttu-id="a15e7-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-143">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="a15e7-144">encryptedPfxBlob</span></span>|<span data-ttu-id="a15e7-145">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-145">String</span></span>|<span data-ttu-id="a15e7-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-146">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="a15e7-147">encryptedPfxPassword</span></span>|<span data-ttu-id="a15e7-148">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-148">String</span></span>|<span data-ttu-id="a15e7-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-149">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="a15e7-150">certStartDate</span></span>|<span data-ttu-id="a15e7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15e7-151">DateTimeOffset</span></span>|<span data-ttu-id="a15e7-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-152">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="a15e7-153">certExpirationDate</span></span>|<span data-ttu-id="a15e7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15e7-154">DateTimeOffset</span></span>|<span data-ttu-id="a15e7-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-155">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-156">providerName</span><span class="sxs-lookup"><span data-stu-id="a15e7-156">providerName</span></span>|<span data-ttu-id="a15e7-157">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-157">String</span></span>|<span data-ttu-id="a15e7-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-158">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="a15e7-159">encryptionKeyName</span></span>|<span data-ttu-id="a15e7-160">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-160">String</span></span>|<span data-ttu-id="a15e7-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-161">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="a15e7-162">paddingScheme</span></span>|<span data-ttu-id="a15e7-163">Int32</span><span class="sxs-lookup"><span data-stu-id="a15e7-163">Int32</span></span>|<span data-ttu-id="a15e7-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-164">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-165">status</span><span class="sxs-lookup"><span data-stu-id="a15e7-165">status</span></span>|<span data-ttu-id="a15e7-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a15e7-166">Int32</span></span>|<span data-ttu-id="a15e7-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-167">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-168">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="a15e7-168">intendedPurpose</span></span>|<span data-ttu-id="a15e7-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a15e7-169">Int32</span></span>|<span data-ttu-id="a15e7-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-170">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-171">createdtime</span><span class="sxs-lookup"><span data-stu-id="a15e7-171">createdTime</span></span>|<span data-ttu-id="a15e7-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15e7-172">DateTimeOffset</span></span>|<span data-ttu-id="a15e7-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-173">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a15e7-174">isDeleted</span></span>|<span data-ttu-id="a15e7-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="a15e7-175">Boolean</span></span>|<span data-ttu-id="a15e7-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-176">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a15e7-177">lastModifiedTime</span></span>|<span data-ttu-id="a15e7-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15e7-178">DateTimeOffset</span></span>|<span data-ttu-id="a15e7-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-179">Not yet documented</span></span>|
|<span data-ttu-id="a15e7-180">eTag</span><span class="sxs-lookup"><span data-stu-id="a15e7-180">eTag</span></span>|<span data-ttu-id="a15e7-181">String</span><span class="sxs-lookup"><span data-stu-id="a15e7-181">String</span></span>|<span data-ttu-id="a15e7-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a15e7-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a15e7-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="a15e7-183">Response</span></span>
<span data-ttu-id="a15e7-184">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a15e7-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a15e7-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a15e7-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="a15e7-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a15e7-186">Request</span></span>
<span data-ttu-id="a15e7-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a15e7-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxUserCertificates
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="a15e7-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="a15e7-188">Response</span></span>
<span data-ttu-id="a15e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a15e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```




