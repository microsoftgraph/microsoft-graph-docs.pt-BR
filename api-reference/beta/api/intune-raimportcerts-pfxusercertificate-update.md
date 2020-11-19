---
title: Atualizar pfxUserCertificate
description: Atualiza as propriedades de um objeto pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47f91d5a4ad9f534c03d207d4a317382ea050831
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270068"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="950ca-103">Atualizar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="950ca-103">Update pfxUserCertificate</span></span>

<span data-ttu-id="950ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="950ca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="950ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="950ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="950ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950ca-107">Atualiza as propriedades de um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="950ca-107">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="950ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="950ca-108">Prerequisites</span></span>
<span data-ttu-id="950ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="950ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="950ca-111">Permission type</span></span>|<span data-ttu-id="950ca-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="950ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="950ca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="950ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="950ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="950ca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="950ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="950ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="950ca-116">Not supported.</span></span>|
|<span data-ttu-id="950ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="950ca-117">Application</span></span>|<span data-ttu-id="950ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="950ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="950ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="950ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="950ca-120">Request headers</span></span>
|<span data-ttu-id="950ca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="950ca-121">Header</span></span>|<span data-ttu-id="950ca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="950ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="950ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="950ca-123">Authorization</span></span>|<span data-ttu-id="950ca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="950ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="950ca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="950ca-125">Accept</span></span>|<span data-ttu-id="950ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="950ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="950ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="950ca-127">Request body</span></span>
<span data-ttu-id="950ca-128">No corpo da solicitação, forneça uma representação JSON do objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="950ca-128">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="950ca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="950ca-129">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="950ca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="950ca-130">Property</span></span>|<span data-ttu-id="950ca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="950ca-131">Type</span></span>|<span data-ttu-id="950ca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="950ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950ca-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="950ca-133">tenantId</span></span>|<span data-ttu-id="950ca-134">Guid</span><span class="sxs-lookup"><span data-stu-id="950ca-134">Guid</span></span>|<span data-ttu-id="950ca-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-135">Not yet documented</span></span>|
|<span data-ttu-id="950ca-136">userId</span><span class="sxs-lookup"><span data-stu-id="950ca-136">userId</span></span>|<span data-ttu-id="950ca-137">Guid</span><span class="sxs-lookup"><span data-stu-id="950ca-137">Guid</span></span>|<span data-ttu-id="950ca-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-138">Not yet documented</span></span>|
|<span data-ttu-id="950ca-139">identificação</span><span class="sxs-lookup"><span data-stu-id="950ca-139">thumbprint</span></span>|<span data-ttu-id="950ca-140">String</span><span class="sxs-lookup"><span data-stu-id="950ca-140">String</span></span>|<span data-ttu-id="950ca-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-141">Not yet documented</span></span>|
|<span data-ttu-id="950ca-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="950ca-142">userUpn</span></span>|<span data-ttu-id="950ca-143">String</span><span class="sxs-lookup"><span data-stu-id="950ca-143">String</span></span>|<span data-ttu-id="950ca-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-144">Not yet documented</span></span>|
|<span data-ttu-id="950ca-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="950ca-145">encryptedPfxBlob</span></span>|<span data-ttu-id="950ca-146">String</span><span class="sxs-lookup"><span data-stu-id="950ca-146">String</span></span>|<span data-ttu-id="950ca-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-147">Not yet documented</span></span>|
|<span data-ttu-id="950ca-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="950ca-148">encryptedPfxPassword</span></span>|<span data-ttu-id="950ca-149">String</span><span class="sxs-lookup"><span data-stu-id="950ca-149">String</span></span>|<span data-ttu-id="950ca-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-150">Not yet documented</span></span>|
|<span data-ttu-id="950ca-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="950ca-151">certStartDate</span></span>|<span data-ttu-id="950ca-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950ca-152">DateTimeOffset</span></span>|<span data-ttu-id="950ca-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-153">Not yet documented</span></span>|
|<span data-ttu-id="950ca-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="950ca-154">certExpirationDate</span></span>|<span data-ttu-id="950ca-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950ca-155">DateTimeOffset</span></span>|<span data-ttu-id="950ca-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-156">Not yet documented</span></span>|
|<span data-ttu-id="950ca-157">providerName</span><span class="sxs-lookup"><span data-stu-id="950ca-157">providerName</span></span>|<span data-ttu-id="950ca-158">String</span><span class="sxs-lookup"><span data-stu-id="950ca-158">String</span></span>|<span data-ttu-id="950ca-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-159">Not yet documented</span></span>|
|<span data-ttu-id="950ca-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="950ca-160">encryptionKeyName</span></span>|<span data-ttu-id="950ca-161">String</span><span class="sxs-lookup"><span data-stu-id="950ca-161">String</span></span>|<span data-ttu-id="950ca-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-162">Not yet documented</span></span>|
|<span data-ttu-id="950ca-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="950ca-163">paddingScheme</span></span>|<span data-ttu-id="950ca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="950ca-164">Int32</span></span>|<span data-ttu-id="950ca-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-165">Not yet documented</span></span>|
|<span data-ttu-id="950ca-166">status</span><span class="sxs-lookup"><span data-stu-id="950ca-166">status</span></span>|<span data-ttu-id="950ca-167">Int32</span><span class="sxs-lookup"><span data-stu-id="950ca-167">Int32</span></span>|<span data-ttu-id="950ca-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-168">Not yet documented</span></span>|
|<span data-ttu-id="950ca-169">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="950ca-169">intendedPurpose</span></span>|<span data-ttu-id="950ca-170">Int32</span><span class="sxs-lookup"><span data-stu-id="950ca-170">Int32</span></span>|<span data-ttu-id="950ca-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-171">Not yet documented</span></span>|
|<span data-ttu-id="950ca-172">createdtime</span><span class="sxs-lookup"><span data-stu-id="950ca-172">createdTime</span></span>|<span data-ttu-id="950ca-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950ca-173">DateTimeOffset</span></span>|<span data-ttu-id="950ca-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-174">Not yet documented</span></span>|
|<span data-ttu-id="950ca-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="950ca-175">isDeleted</span></span>|<span data-ttu-id="950ca-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="950ca-176">Boolean</span></span>|<span data-ttu-id="950ca-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-177">Not yet documented</span></span>|
|<span data-ttu-id="950ca-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="950ca-178">lastModifiedTime</span></span>|<span data-ttu-id="950ca-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950ca-179">DateTimeOffset</span></span>|<span data-ttu-id="950ca-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-180">Not yet documented</span></span>|
|<span data-ttu-id="950ca-181">eTag</span><span class="sxs-lookup"><span data-stu-id="950ca-181">eTag</span></span>|<span data-ttu-id="950ca-182">String</span><span class="sxs-lookup"><span data-stu-id="950ca-182">String</span></span>|<span data-ttu-id="950ca-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="950ca-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="950ca-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="950ca-184">Response</span></span>
<span data-ttu-id="950ca-185">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="950ca-185">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="950ca-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="950ca-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="950ca-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="950ca-187">Request</span></span>
<span data-ttu-id="950ca-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="950ca-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="950ca-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="950ca-189">Response</span></span>
<span data-ttu-id="950ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="950ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




