---
title: Atualizar pfxUserCertificate
description: Atualiza as propriedades de um objeto pfxUserCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4498260afe255b5b71e5d2bcfab44df331e5c24
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460063"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="0dfc7-103">Atualizar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="0dfc7-103">Update pfxUserCertificate</span></span>

<span data-ttu-id="0dfc7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0dfc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dfc7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dfc7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dfc7-107">Atualiza as propriedades de um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="0dfc7-107">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dfc7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0dfc7-108">Prerequisites</span></span>
<span data-ttu-id="0dfc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dfc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dfc7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dfc7-111">Permission type</span></span>|<span data-ttu-id="0dfc7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0dfc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dfc7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dfc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dfc7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfc7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0dfc7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dfc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dfc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-116">Not supported.</span></span>|
|<span data-ttu-id="0dfc7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dfc7-117">Application</span></span>|<span data-ttu-id="0dfc7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfc7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dfc7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dfc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="0dfc7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dfc7-120">Request headers</span></span>
|<span data-ttu-id="0dfc7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0dfc7-121">Header</span></span>|<span data-ttu-id="0dfc7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0dfc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dfc7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dfc7-123">Authorization</span></span>|<span data-ttu-id="0dfc7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dfc7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0dfc7-125">Accept</span></span>|<span data-ttu-id="0dfc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dfc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dfc7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dfc7-127">Request body</span></span>
<span data-ttu-id="0dfc7-128">No corpo da solicitação, forneça uma representação JSON do objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="0dfc7-128">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="0dfc7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0dfc7-129">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="0dfc7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dfc7-130">Property</span></span>|<span data-ttu-id="0dfc7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dfc7-131">Type</span></span>|<span data-ttu-id="0dfc7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dfc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dfc7-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="0dfc7-133">tenantId</span></span>|<span data-ttu-id="0dfc7-134">Guid</span><span class="sxs-lookup"><span data-stu-id="0dfc7-134">Guid</span></span>|<span data-ttu-id="0dfc7-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-135">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-136">userId</span><span class="sxs-lookup"><span data-stu-id="0dfc7-136">userId</span></span>|<span data-ttu-id="0dfc7-137">Guid</span><span class="sxs-lookup"><span data-stu-id="0dfc7-137">Guid</span></span>|<span data-ttu-id="0dfc7-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-138">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-139">identificação</span><span class="sxs-lookup"><span data-stu-id="0dfc7-139">thumbprint</span></span>|<span data-ttu-id="0dfc7-140">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-140">String</span></span>|<span data-ttu-id="0dfc7-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-141">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="0dfc7-142">userUpn</span></span>|<span data-ttu-id="0dfc7-143">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-143">String</span></span>|<span data-ttu-id="0dfc7-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-144">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="0dfc7-145">encryptedPfxBlob</span></span>|<span data-ttu-id="0dfc7-146">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-146">String</span></span>|<span data-ttu-id="0dfc7-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-147">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="0dfc7-148">encryptedPfxPassword</span></span>|<span data-ttu-id="0dfc7-149">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-149">String</span></span>|<span data-ttu-id="0dfc7-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-150">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="0dfc7-151">certStartDate</span></span>|<span data-ttu-id="0dfc7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dfc7-152">DateTimeOffset</span></span>|<span data-ttu-id="0dfc7-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-153">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0dfc7-154">certExpirationDate</span></span>|<span data-ttu-id="0dfc7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dfc7-155">DateTimeOffset</span></span>|<span data-ttu-id="0dfc7-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-156">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-157">providerName</span><span class="sxs-lookup"><span data-stu-id="0dfc7-157">providerName</span></span>|<span data-ttu-id="0dfc7-158">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-158">String</span></span>|<span data-ttu-id="0dfc7-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-159">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="0dfc7-160">encryptionKeyName</span></span>|<span data-ttu-id="0dfc7-161">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-161">String</span></span>|<span data-ttu-id="0dfc7-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-162">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="0dfc7-163">paddingScheme</span></span>|<span data-ttu-id="0dfc7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfc7-164">Int32</span></span>|<span data-ttu-id="0dfc7-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-165">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-166">status</span><span class="sxs-lookup"><span data-stu-id="0dfc7-166">status</span></span>|<span data-ttu-id="0dfc7-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfc7-167">Int32</span></span>|<span data-ttu-id="0dfc7-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-168">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-169">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="0dfc7-169">intendedPurpose</span></span>|<span data-ttu-id="0dfc7-170">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfc7-170">Int32</span></span>|<span data-ttu-id="0dfc7-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-171">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-172">createdtime</span><span class="sxs-lookup"><span data-stu-id="0dfc7-172">createdTime</span></span>|<span data-ttu-id="0dfc7-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dfc7-173">DateTimeOffset</span></span>|<span data-ttu-id="0dfc7-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-174">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0dfc7-175">isDeleted</span></span>|<span data-ttu-id="0dfc7-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="0dfc7-176">Boolean</span></span>|<span data-ttu-id="0dfc7-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-177">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0dfc7-178">lastModifiedTime</span></span>|<span data-ttu-id="0dfc7-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dfc7-179">DateTimeOffset</span></span>|<span data-ttu-id="0dfc7-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-180">Not yet documented</span></span>|
|<span data-ttu-id="0dfc7-181">eTag</span><span class="sxs-lookup"><span data-stu-id="0dfc7-181">eTag</span></span>|<span data-ttu-id="0dfc7-182">String</span><span class="sxs-lookup"><span data-stu-id="0dfc7-182">String</span></span>|<span data-ttu-id="0dfc7-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dfc7-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0dfc7-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dfc7-184">Response</span></span>
<span data-ttu-id="0dfc7-185">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-185">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dfc7-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0dfc7-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dfc7-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dfc7-187">Request</span></span>
<span data-ttu-id="0dfc7-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0dfc7-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dfc7-189">Response</span></span>
<span data-ttu-id="0dfc7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0dfc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





