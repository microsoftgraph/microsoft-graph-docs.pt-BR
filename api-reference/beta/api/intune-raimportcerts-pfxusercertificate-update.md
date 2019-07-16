---
title: Atualizar pfxUserCertificate
description: Atualiza as propriedades de um objeto pfxUserCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6756a6c35818426790e24d7f348ca760355ffec6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725835"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="395cc-103">Atualizar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="395cc-103">Update pfxUserCertificate</span></span>

> <span data-ttu-id="395cc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="395cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="395cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="395cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="395cc-106">Atualiza as propriedades de um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="395cc-106">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="395cc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="395cc-107">Prerequisites</span></span>
<span data-ttu-id="395cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="395cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="395cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="395cc-110">Permission type</span></span>|<span data-ttu-id="395cc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="395cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="395cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="395cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="395cc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="395cc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="395cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="395cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="395cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="395cc-115">Not supported.</span></span>|
|<span data-ttu-id="395cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="395cc-116">Application</span></span>|<span data-ttu-id="395cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="395cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="395cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="395cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="395cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="395cc-119">Request headers</span></span>
|<span data-ttu-id="395cc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="395cc-120">Header</span></span>|<span data-ttu-id="395cc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="395cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="395cc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="395cc-122">Authorization</span></span>|<span data-ttu-id="395cc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="395cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="395cc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="395cc-124">Accept</span></span>|<span data-ttu-id="395cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="395cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="395cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="395cc-126">Request body</span></span>
<span data-ttu-id="395cc-127">No corpo da solicitação, forneça uma representação JSON do objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="395cc-127">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="395cc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="395cc-128">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="395cc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="395cc-129">Property</span></span>|<span data-ttu-id="395cc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="395cc-130">Type</span></span>|<span data-ttu-id="395cc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="395cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="395cc-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="395cc-132">tenantId</span></span>|<span data-ttu-id="395cc-133">Guid</span><span class="sxs-lookup"><span data-stu-id="395cc-133">Guid</span></span>|<span data-ttu-id="395cc-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-134">Not yet documented</span></span>|
|<span data-ttu-id="395cc-135">userId</span><span class="sxs-lookup"><span data-stu-id="395cc-135">userId</span></span>|<span data-ttu-id="395cc-136">Guid</span><span class="sxs-lookup"><span data-stu-id="395cc-136">Guid</span></span>|<span data-ttu-id="395cc-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-137">Not yet documented</span></span>|
|<span data-ttu-id="395cc-138">identificação</span><span class="sxs-lookup"><span data-stu-id="395cc-138">thumbprint</span></span>|<span data-ttu-id="395cc-139">String</span><span class="sxs-lookup"><span data-stu-id="395cc-139">String</span></span>|<span data-ttu-id="395cc-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-140">Not yet documented</span></span>|
|<span data-ttu-id="395cc-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="395cc-141">userUpn</span></span>|<span data-ttu-id="395cc-142">String</span><span class="sxs-lookup"><span data-stu-id="395cc-142">String</span></span>|<span data-ttu-id="395cc-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-143">Not yet documented</span></span>|
|<span data-ttu-id="395cc-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="395cc-144">encryptedPfxBlob</span></span>|<span data-ttu-id="395cc-145">String</span><span class="sxs-lookup"><span data-stu-id="395cc-145">String</span></span>|<span data-ttu-id="395cc-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-146">Not yet documented</span></span>|
|<span data-ttu-id="395cc-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="395cc-147">encryptedPfxPassword</span></span>|<span data-ttu-id="395cc-148">String</span><span class="sxs-lookup"><span data-stu-id="395cc-148">String</span></span>|<span data-ttu-id="395cc-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-149">Not yet documented</span></span>|
|<span data-ttu-id="395cc-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="395cc-150">certStartDate</span></span>|<span data-ttu-id="395cc-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="395cc-151">DateTimeOffset</span></span>|<span data-ttu-id="395cc-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-152">Not yet documented</span></span>|
|<span data-ttu-id="395cc-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="395cc-153">certExpirationDate</span></span>|<span data-ttu-id="395cc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="395cc-154">DateTimeOffset</span></span>|<span data-ttu-id="395cc-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-155">Not yet documented</span></span>|
|<span data-ttu-id="395cc-156">providerName</span><span class="sxs-lookup"><span data-stu-id="395cc-156">providerName</span></span>|<span data-ttu-id="395cc-157">String</span><span class="sxs-lookup"><span data-stu-id="395cc-157">String</span></span>|<span data-ttu-id="395cc-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-158">Not yet documented</span></span>|
|<span data-ttu-id="395cc-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="395cc-159">encryptionKeyName</span></span>|<span data-ttu-id="395cc-160">String</span><span class="sxs-lookup"><span data-stu-id="395cc-160">String</span></span>|<span data-ttu-id="395cc-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-161">Not yet documented</span></span>|
|<span data-ttu-id="395cc-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="395cc-162">paddingScheme</span></span>|<span data-ttu-id="395cc-163">Int32</span><span class="sxs-lookup"><span data-stu-id="395cc-163">Int32</span></span>|<span data-ttu-id="395cc-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-164">Not yet documented</span></span>|
|<span data-ttu-id="395cc-165">status</span><span class="sxs-lookup"><span data-stu-id="395cc-165">status</span></span>|<span data-ttu-id="395cc-166">Int32</span><span class="sxs-lookup"><span data-stu-id="395cc-166">Int32</span></span>|<span data-ttu-id="395cc-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-167">Not yet documented</span></span>|
|<span data-ttu-id="395cc-168">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="395cc-168">intendedPurpose</span></span>|<span data-ttu-id="395cc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="395cc-169">Int32</span></span>|<span data-ttu-id="395cc-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-170">Not yet documented</span></span>|
|<span data-ttu-id="395cc-171">createdtime</span><span class="sxs-lookup"><span data-stu-id="395cc-171">createdTime</span></span>|<span data-ttu-id="395cc-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="395cc-172">DateTimeOffset</span></span>|<span data-ttu-id="395cc-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-173">Not yet documented</span></span>|
|<span data-ttu-id="395cc-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="395cc-174">isDeleted</span></span>|<span data-ttu-id="395cc-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="395cc-175">Boolean</span></span>|<span data-ttu-id="395cc-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-176">Not yet documented</span></span>|
|<span data-ttu-id="395cc-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="395cc-177">lastModifiedTime</span></span>|<span data-ttu-id="395cc-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="395cc-178">DateTimeOffset</span></span>|<span data-ttu-id="395cc-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-179">Not yet documented</span></span>|
|<span data-ttu-id="395cc-180">eTag</span><span class="sxs-lookup"><span data-stu-id="395cc-180">eTag</span></span>|<span data-ttu-id="395cc-181">String</span><span class="sxs-lookup"><span data-stu-id="395cc-181">String</span></span>|<span data-ttu-id="395cc-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="395cc-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="395cc-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="395cc-183">Response</span></span>
<span data-ttu-id="395cc-184">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="395cc-184">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="395cc-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="395cc-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="395cc-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="395cc-186">Request</span></span>
<span data-ttu-id="395cc-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="395cc-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
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

### <a name="response"></a><span data-ttu-id="395cc-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="395cc-188">Response</span></span>
<span data-ttu-id="395cc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="395cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





