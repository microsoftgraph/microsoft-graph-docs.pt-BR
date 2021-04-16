---
title: Criar onPremEncryptedPayload
description: Crie um novo objeto onPremEncryptedPayload.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d59d96b814505f4c19cf3a0257b2744ac907182
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868259"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="83f83-103">Criar onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="83f83-103">Create onPremEncryptedPayload</span></span>

<span data-ttu-id="83f83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83f83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83f83-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83f83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83f83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83f83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f83-107">Crie um novo [objeto onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)</span><span class="sxs-lookup"><span data-stu-id="83f83-107">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83f83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83f83-108">Prerequisites</span></span>
<span data-ttu-id="83f83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83f83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83f83-111">Permission type</span></span>|<span data-ttu-id="83f83-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83f83-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83f83-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83f83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83f83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83f83-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83f83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83f83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83f83-116">Not supported.</span></span>|
|<span data-ttu-id="83f83-117">Application</span><span class="sxs-lookup"><span data-stu-id="83f83-117">Application</span></span>|<span data-ttu-id="83f83-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f83-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83f83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83f83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="83f83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83f83-120">Request headers</span></span>
|<span data-ttu-id="83f83-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83f83-121">Header</span></span>|<span data-ttu-id="83f83-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83f83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83f83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83f83-123">Authorization</span></span>|<span data-ttu-id="83f83-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83f83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83f83-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83f83-125">Accept</span></span>|<span data-ttu-id="83f83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83f83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83f83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83f83-127">Request body</span></span>
<span data-ttu-id="83f83-128">No corpo da solicitação, fornece uma representação JSON para o objeto onPremEncryptedPayload.</span><span class="sxs-lookup"><span data-stu-id="83f83-128">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="83f83-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o onPremEncryptedPayload.</span><span class="sxs-lookup"><span data-stu-id="83f83-129">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="83f83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83f83-130">Property</span></span>|<span data-ttu-id="83f83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="83f83-131">Type</span></span>|<span data-ttu-id="83f83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="83f83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83f83-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="83f83-133">tenantId</span></span>|<span data-ttu-id="83f83-134">Guid</span><span class="sxs-lookup"><span data-stu-id="83f83-134">Guid</span></span>|<span data-ttu-id="83f83-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-135">Not yet documented</span></span>|
|<span data-ttu-id="83f83-136">userId</span><span class="sxs-lookup"><span data-stu-id="83f83-136">userId</span></span>|<span data-ttu-id="83f83-137">Guid</span><span class="sxs-lookup"><span data-stu-id="83f83-137">Guid</span></span>|<span data-ttu-id="83f83-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-138">Not yet documented</span></span>|
|<span data-ttu-id="83f83-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="83f83-139">deviceId</span></span>|<span data-ttu-id="83f83-140">Guid</span><span class="sxs-lookup"><span data-stu-id="83f83-140">Guid</span></span>|<span data-ttu-id="83f83-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-141">Not yet documented</span></span>|
|<span data-ttu-id="83f83-142">payloadId</span><span class="sxs-lookup"><span data-stu-id="83f83-142">payloadId</span></span>|<span data-ttu-id="83f83-143">Guid</span><span class="sxs-lookup"><span data-stu-id="83f83-143">Guid</span></span>|<span data-ttu-id="83f83-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-144">Not yet documented</span></span>|
|<span data-ttu-id="83f83-145">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="83f83-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="83f83-146">String</span><span class="sxs-lookup"><span data-stu-id="83f83-146">String</span></span>|<span data-ttu-id="83f83-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-147">Not yet documented</span></span>|
|<span data-ttu-id="83f83-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="83f83-148">cert1PayloadUUID</span></span>|<span data-ttu-id="83f83-149">String</span><span class="sxs-lookup"><span data-stu-id="83f83-149">String</span></span>|<span data-ttu-id="83f83-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-150">Not yet documented</span></span>|
|<span data-ttu-id="83f83-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="83f83-151">cert2PayloadUUID</span></span>|<span data-ttu-id="83f83-152">String</span><span class="sxs-lookup"><span data-stu-id="83f83-152">String</span></span>|<span data-ttu-id="83f83-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-153">Not yet documented</span></span>|
|<span data-ttu-id="83f83-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="83f83-154">cert3PayloadUUID</span></span>|<span data-ttu-id="83f83-155">String</span><span class="sxs-lookup"><span data-stu-id="83f83-155">String</span></span>|<span data-ttu-id="83f83-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-156">Not yet documented</span></span>|
|<span data-ttu-id="83f83-157">plistTemplate</span><span class="sxs-lookup"><span data-stu-id="83f83-157">plistTemplate</span></span>|<span data-ttu-id="83f83-158">String</span><span class="sxs-lookup"><span data-stu-id="83f83-158">String</span></span>|<span data-ttu-id="83f83-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-159">Not yet documented</span></span>|
|<span data-ttu-id="83f83-160">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="83f83-160">encryptedBlob</span></span>|<span data-ttu-id="83f83-161">Binário</span><span class="sxs-lookup"><span data-stu-id="83f83-161">Binary</span></span>|<span data-ttu-id="83f83-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-162">Not yet documented</span></span>|
|<span data-ttu-id="83f83-163">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="83f83-163">payloadVersion</span></span>|<span data-ttu-id="83f83-164">Int32</span><span class="sxs-lookup"><span data-stu-id="83f83-164">Int32</span></span>|<span data-ttu-id="83f83-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-165">Not yet documented</span></span>|
|<span data-ttu-id="83f83-166">status</span><span class="sxs-lookup"><span data-stu-id="83f83-166">status</span></span>|<span data-ttu-id="83f83-167">Int32</span><span class="sxs-lookup"><span data-stu-id="83f83-167">Int32</span></span>|<span data-ttu-id="83f83-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-168">Not yet documented</span></span>|
|<span data-ttu-id="83f83-169">createdTime</span><span class="sxs-lookup"><span data-stu-id="83f83-169">createdTime</span></span>|<span data-ttu-id="83f83-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f83-170">DateTimeOffset</span></span>|<span data-ttu-id="83f83-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-171">Not yet documented</span></span>|
|<span data-ttu-id="83f83-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="83f83-172">lastModifiedTime</span></span>|<span data-ttu-id="83f83-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f83-173">DateTimeOffset</span></span>|<span data-ttu-id="83f83-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-174">Not yet documented</span></span>|
|<span data-ttu-id="83f83-175">eTag</span><span class="sxs-lookup"><span data-stu-id="83f83-175">eTag</span></span>|<span data-ttu-id="83f83-176">String</span><span class="sxs-lookup"><span data-stu-id="83f83-176">String</span></span>|<span data-ttu-id="83f83-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-177">Not yet documented</span></span>|
|<span data-ttu-id="83f83-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="83f83-178">isDeleted</span></span>|<span data-ttu-id="83f83-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="83f83-179">Boolean</span></span>|<span data-ttu-id="83f83-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83f83-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="83f83-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="83f83-181">Response</span></span>
<span data-ttu-id="83f83-182">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83f83-182">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83f83-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83f83-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="83f83-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83f83-184">Request</span></span>
<span data-ttu-id="83f83-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83f83-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/onPremEncryptedPayloads
Content-type: application/json
Content-length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```

### <a name="response"></a><span data-ttu-id="83f83-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="83f83-186">Response</span></span>
<span data-ttu-id="83f83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83f83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```




