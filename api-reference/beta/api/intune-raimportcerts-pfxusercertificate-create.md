---
title: Criar pfxUserCertificate
description: Criar um novo objeto pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c564f89cb711981708684da2d8be943e8531e10
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437693"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="f7c0f-103">Criar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="f7c0f-103">Create pfxUserCertificate</span></span>

<span data-ttu-id="f7c0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7c0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7c0f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7c0f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7c0f-107">Criar um novo objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="f7c0f-107">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7c0f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7c0f-108">Prerequisites</span></span>
<span data-ttu-id="f7c0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c0f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7c0f-111">Permission type</span></span>|<span data-ttu-id="f7c0f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7c0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7c0f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7c0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7c0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7c0f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7c0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-116">Not supported.</span></span>|
|<span data-ttu-id="f7c0f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7c0f-117">Application</span></span>|<span data-ttu-id="f7c0f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c0f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7c0f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="f7c0f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7c0f-120">Request headers</span></span>
|<span data-ttu-id="f7c0f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7c0f-121">Header</span></span>|<span data-ttu-id="f7c0f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7c0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7c0f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7c0f-123">Authorization</span></span>|<span data-ttu-id="f7c0f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7c0f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7c0f-125">Accept</span></span>|<span data-ttu-id="f7c0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7c0f-127">Request body</span></span>
<span data-ttu-id="f7c0f-128">No corpo da solicitação, forneça uma representação JSON do objeto pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-128">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="f7c0f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-129">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="f7c0f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7c0f-130">Property</span></span>|<span data-ttu-id="f7c0f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7c0f-131">Type</span></span>|<span data-ttu-id="f7c0f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7c0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7c0f-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="f7c0f-133">tenantId</span></span>|<span data-ttu-id="f7c0f-134">Guid</span><span class="sxs-lookup"><span data-stu-id="f7c0f-134">Guid</span></span>|<span data-ttu-id="f7c0f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-135">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-136">userId</span><span class="sxs-lookup"><span data-stu-id="f7c0f-136">userId</span></span>|<span data-ttu-id="f7c0f-137">Guid</span><span class="sxs-lookup"><span data-stu-id="f7c0f-137">Guid</span></span>|<span data-ttu-id="f7c0f-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-138">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-139">identificação</span><span class="sxs-lookup"><span data-stu-id="f7c0f-139">thumbprint</span></span>|<span data-ttu-id="f7c0f-140">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-140">String</span></span>|<span data-ttu-id="f7c0f-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-141">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="f7c0f-142">userUpn</span></span>|<span data-ttu-id="f7c0f-143">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-143">String</span></span>|<span data-ttu-id="f7c0f-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-144">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="f7c0f-145">encryptedPfxBlob</span></span>|<span data-ttu-id="f7c0f-146">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-146">String</span></span>|<span data-ttu-id="f7c0f-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-147">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="f7c0f-148">encryptedPfxPassword</span></span>|<span data-ttu-id="f7c0f-149">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-149">String</span></span>|<span data-ttu-id="f7c0f-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-150">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="f7c0f-151">certStartDate</span></span>|<span data-ttu-id="f7c0f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7c0f-152">DateTimeOffset</span></span>|<span data-ttu-id="f7c0f-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-153">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="f7c0f-154">certExpirationDate</span></span>|<span data-ttu-id="f7c0f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7c0f-155">DateTimeOffset</span></span>|<span data-ttu-id="f7c0f-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-156">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-157">providerName</span><span class="sxs-lookup"><span data-stu-id="f7c0f-157">providerName</span></span>|<span data-ttu-id="f7c0f-158">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-158">String</span></span>|<span data-ttu-id="f7c0f-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-159">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="f7c0f-160">encryptionKeyName</span></span>|<span data-ttu-id="f7c0f-161">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-161">String</span></span>|<span data-ttu-id="f7c0f-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-162">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="f7c0f-163">paddingScheme</span></span>|<span data-ttu-id="f7c0f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f7c0f-164">Int32</span></span>|<span data-ttu-id="f7c0f-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-165">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-166">status</span><span class="sxs-lookup"><span data-stu-id="f7c0f-166">status</span></span>|<span data-ttu-id="f7c0f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="f7c0f-167">Int32</span></span>|<span data-ttu-id="f7c0f-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-168">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-169">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="f7c0f-169">intendedPurpose</span></span>|<span data-ttu-id="f7c0f-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f7c0f-170">Int32</span></span>|<span data-ttu-id="f7c0f-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-171">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-172">createdtime</span><span class="sxs-lookup"><span data-stu-id="f7c0f-172">createdTime</span></span>|<span data-ttu-id="f7c0f-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7c0f-173">DateTimeOffset</span></span>|<span data-ttu-id="f7c0f-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-174">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f7c0f-175">isDeleted</span></span>|<span data-ttu-id="f7c0f-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7c0f-176">Boolean</span></span>|<span data-ttu-id="f7c0f-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-177">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f7c0f-178">lastModifiedTime</span></span>|<span data-ttu-id="f7c0f-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7c0f-179">DateTimeOffset</span></span>|<span data-ttu-id="f7c0f-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-180">Not yet documented</span></span>|
|<span data-ttu-id="f7c0f-181">eTag</span><span class="sxs-lookup"><span data-stu-id="f7c0f-181">eTag</span></span>|<span data-ttu-id="f7c0f-182">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-182">String</span></span>|<span data-ttu-id="f7c0f-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7c0f-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7c0f-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7c0f-184">Response</span></span>
<span data-ttu-id="f7c0f-185">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-185">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c0f-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7c0f-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7c0f-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7c0f-187">Request</span></span>
<span data-ttu-id="f7c0f-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7c0f-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7c0f-189">Response</span></span>
<span data-ttu-id="f7c0f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



