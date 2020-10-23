---
title: Atualizar pfxUserCertificate
description: Atualiza as propriedades de um objeto pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd11409a4e3a07b15d79104e7815f469d749522f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708001"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="d6ce4-103">Atualizar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="d6ce4-103">Update pfxUserCertificate</span></span>

<span data-ttu-id="d6ce4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6ce4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6ce4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6ce4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6ce4-107">Atualiza as propriedades de um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d6ce4-107">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6ce4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6ce4-108">Prerequisites</span></span>
<span data-ttu-id="d6ce4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6ce4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6ce4-111">Permission type</span></span>|<span data-ttu-id="d6ce4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6ce4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6ce4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6ce4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6ce4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ce4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6ce4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6ce4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6ce4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-116">Not supported.</span></span>|
|<span data-ttu-id="d6ce4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6ce4-117">Application</span></span>|<span data-ttu-id="d6ce4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ce4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6ce4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ce4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="d6ce4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ce4-120">Request headers</span></span>
|<span data-ttu-id="d6ce4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6ce4-121">Header</span></span>|<span data-ttu-id="d6ce4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6ce4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6ce4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6ce4-123">Authorization</span></span>|<span data-ttu-id="d6ce4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6ce4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6ce4-125">Accept</span></span>|<span data-ttu-id="d6ce4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6ce4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6ce4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ce4-127">Request body</span></span>
<span data-ttu-id="d6ce4-128">No corpo da solicitação, forneça uma representação JSON do objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d6ce4-128">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="d6ce4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d6ce4-129">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="d6ce4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6ce4-130">Property</span></span>|<span data-ttu-id="d6ce4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ce4-131">Type</span></span>|<span data-ttu-id="d6ce4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ce4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6ce4-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="d6ce4-133">tenantId</span></span>|<span data-ttu-id="d6ce4-134">Guid</span><span class="sxs-lookup"><span data-stu-id="d6ce4-134">Guid</span></span>|<span data-ttu-id="d6ce4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-135">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-136">userId</span><span class="sxs-lookup"><span data-stu-id="d6ce4-136">userId</span></span>|<span data-ttu-id="d6ce4-137">Guid</span><span class="sxs-lookup"><span data-stu-id="d6ce4-137">Guid</span></span>|<span data-ttu-id="d6ce4-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-138">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-139">identificação</span><span class="sxs-lookup"><span data-stu-id="d6ce4-139">thumbprint</span></span>|<span data-ttu-id="d6ce4-140">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-140">String</span></span>|<span data-ttu-id="d6ce4-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-141">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="d6ce4-142">userUpn</span></span>|<span data-ttu-id="d6ce4-143">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-143">String</span></span>|<span data-ttu-id="d6ce4-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-144">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="d6ce4-145">encryptedPfxBlob</span></span>|<span data-ttu-id="d6ce4-146">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-146">String</span></span>|<span data-ttu-id="d6ce4-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-147">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="d6ce4-148">encryptedPfxPassword</span></span>|<span data-ttu-id="d6ce4-149">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-149">String</span></span>|<span data-ttu-id="d6ce4-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-150">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="d6ce4-151">certStartDate</span></span>|<span data-ttu-id="d6ce4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6ce4-152">DateTimeOffset</span></span>|<span data-ttu-id="d6ce4-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-153">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d6ce4-154">certExpirationDate</span></span>|<span data-ttu-id="d6ce4-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6ce4-155">DateTimeOffset</span></span>|<span data-ttu-id="d6ce4-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-156">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-157">providerName</span><span class="sxs-lookup"><span data-stu-id="d6ce4-157">providerName</span></span>|<span data-ttu-id="d6ce4-158">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-158">String</span></span>|<span data-ttu-id="d6ce4-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-159">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="d6ce4-160">encryptionKeyName</span></span>|<span data-ttu-id="d6ce4-161">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-161">String</span></span>|<span data-ttu-id="d6ce4-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-162">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="d6ce4-163">paddingScheme</span></span>|<span data-ttu-id="d6ce4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d6ce4-164">Int32</span></span>|<span data-ttu-id="d6ce4-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-165">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-166">status</span><span class="sxs-lookup"><span data-stu-id="d6ce4-166">status</span></span>|<span data-ttu-id="d6ce4-167">Int32</span><span class="sxs-lookup"><span data-stu-id="d6ce4-167">Int32</span></span>|<span data-ttu-id="d6ce4-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-168">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-169">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="d6ce4-169">intendedPurpose</span></span>|<span data-ttu-id="d6ce4-170">Int32</span><span class="sxs-lookup"><span data-stu-id="d6ce4-170">Int32</span></span>|<span data-ttu-id="d6ce4-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-171">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-172">createdtime</span><span class="sxs-lookup"><span data-stu-id="d6ce4-172">createdTime</span></span>|<span data-ttu-id="d6ce4-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6ce4-173">DateTimeOffset</span></span>|<span data-ttu-id="d6ce4-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-174">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d6ce4-175">isDeleted</span></span>|<span data-ttu-id="d6ce4-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6ce4-176">Boolean</span></span>|<span data-ttu-id="d6ce4-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-177">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d6ce4-178">lastModifiedTime</span></span>|<span data-ttu-id="d6ce4-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6ce4-179">DateTimeOffset</span></span>|<span data-ttu-id="d6ce4-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-180">Not yet documented</span></span>|
|<span data-ttu-id="d6ce4-181">eTag</span><span class="sxs-lookup"><span data-stu-id="d6ce4-181">eTag</span></span>|<span data-ttu-id="d6ce4-182">String</span><span class="sxs-lookup"><span data-stu-id="d6ce4-182">String</span></span>|<span data-ttu-id="d6ce4-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ce4-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6ce4-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ce4-184">Response</span></span>
<span data-ttu-id="d6ce4-185">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-185">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6ce4-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6ce4-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6ce4-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ce4-187">Request</span></span>
<span data-ttu-id="d6ce4-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6ce4-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ce4-189">Response</span></span>
<span data-ttu-id="d6ce4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6ce4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





