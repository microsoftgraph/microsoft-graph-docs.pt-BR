---
title: Criar onPremEncryptedPayload
description: Criar um novo objeto onPremEncryptedPayload.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c2e93423f70e99f0475541461fea033ce344b3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725844"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="690f9-103">Criar onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="690f9-103">Create onPremEncryptedPayload</span></span>

> <span data-ttu-id="690f9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="690f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="690f9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="690f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="690f9-106">Criar um novo objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="690f9-106">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="690f9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="690f9-107">Prerequisites</span></span>
<span data-ttu-id="690f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="690f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="690f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="690f9-110">Permission type</span></span>|<span data-ttu-id="690f9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="690f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="690f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="690f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="690f9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690f9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="690f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="690f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="690f9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690f9-115">Not supported.</span></span>|
|<span data-ttu-id="690f9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="690f9-116">Application</span></span>|<span data-ttu-id="690f9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690f9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="690f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="690f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="690f9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="690f9-119">Request headers</span></span>
|<span data-ttu-id="690f9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="690f9-120">Header</span></span>|<span data-ttu-id="690f9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="690f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="690f9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="690f9-122">Authorization</span></span>|<span data-ttu-id="690f9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="690f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="690f9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="690f9-124">Accept</span></span>|<span data-ttu-id="690f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="690f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="690f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="690f9-126">Request body</span></span>
<span data-ttu-id="690f9-127">No corpo da solicitação, forneça uma representação JSON do objeto onPremEncryptedPayload.</span><span class="sxs-lookup"><span data-stu-id="690f9-127">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="690f9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar onPremEncryptedPayload.</span><span class="sxs-lookup"><span data-stu-id="690f9-128">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="690f9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="690f9-129">Property</span></span>|<span data-ttu-id="690f9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="690f9-130">Type</span></span>|<span data-ttu-id="690f9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="690f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="690f9-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="690f9-132">tenantId</span></span>|<span data-ttu-id="690f9-133">Guid</span><span class="sxs-lookup"><span data-stu-id="690f9-133">Guid</span></span>|<span data-ttu-id="690f9-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-134">Not yet documented</span></span>|
|<span data-ttu-id="690f9-135">userId</span><span class="sxs-lookup"><span data-stu-id="690f9-135">userId</span></span>|<span data-ttu-id="690f9-136">Guid</span><span class="sxs-lookup"><span data-stu-id="690f9-136">Guid</span></span>|<span data-ttu-id="690f9-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-137">Not yet documented</span></span>|
|<span data-ttu-id="690f9-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="690f9-138">deviceId</span></span>|<span data-ttu-id="690f9-139">Guid</span><span class="sxs-lookup"><span data-stu-id="690f9-139">Guid</span></span>|<span data-ttu-id="690f9-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-140">Not yet documented</span></span>|
|<span data-ttu-id="690f9-141">payloadId</span><span class="sxs-lookup"><span data-stu-id="690f9-141">payloadId</span></span>|<span data-ttu-id="690f9-142">Guid</span><span class="sxs-lookup"><span data-stu-id="690f9-142">Guid</span></span>|<span data-ttu-id="690f9-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-143">Not yet documented</span></span>|
|<span data-ttu-id="690f9-144">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="690f9-144">deviceKeyThumbprint</span></span>|<span data-ttu-id="690f9-145">String</span><span class="sxs-lookup"><span data-stu-id="690f9-145">String</span></span>|<span data-ttu-id="690f9-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-146">Not yet documented</span></span>|
|<span data-ttu-id="690f9-147">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="690f9-147">cert1PayloadUUID</span></span>|<span data-ttu-id="690f9-148">String</span><span class="sxs-lookup"><span data-stu-id="690f9-148">String</span></span>|<span data-ttu-id="690f9-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-149">Not yet documented</span></span>|
|<span data-ttu-id="690f9-150">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="690f9-150">cert2PayloadUUID</span></span>|<span data-ttu-id="690f9-151">String</span><span class="sxs-lookup"><span data-stu-id="690f9-151">String</span></span>|<span data-ttu-id="690f9-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-152">Not yet documented</span></span>|
|<span data-ttu-id="690f9-153">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="690f9-153">cert3PayloadUUID</span></span>|<span data-ttu-id="690f9-154">String</span><span class="sxs-lookup"><span data-stu-id="690f9-154">String</span></span>|<span data-ttu-id="690f9-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-155">Not yet documented</span></span>|
|<span data-ttu-id="690f9-156">plisttemplate</span><span class="sxs-lookup"><span data-stu-id="690f9-156">plistTemplate</span></span>|<span data-ttu-id="690f9-157">String</span><span class="sxs-lookup"><span data-stu-id="690f9-157">String</span></span>|<span data-ttu-id="690f9-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-158">Not yet documented</span></span>|
|<span data-ttu-id="690f9-159">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="690f9-159">encryptedBlob</span></span>|<span data-ttu-id="690f9-160">Binária</span><span class="sxs-lookup"><span data-stu-id="690f9-160">Binary</span></span>|<span data-ttu-id="690f9-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-161">Not yet documented</span></span>|
|<span data-ttu-id="690f9-162">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="690f9-162">payloadVersion</span></span>|<span data-ttu-id="690f9-163">Int32</span><span class="sxs-lookup"><span data-stu-id="690f9-163">Int32</span></span>|<span data-ttu-id="690f9-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-164">Not yet documented</span></span>|
|<span data-ttu-id="690f9-165">status</span><span class="sxs-lookup"><span data-stu-id="690f9-165">status</span></span>|<span data-ttu-id="690f9-166">Int32</span><span class="sxs-lookup"><span data-stu-id="690f9-166">Int32</span></span>|<span data-ttu-id="690f9-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-167">Not yet documented</span></span>|
|<span data-ttu-id="690f9-168">createdtime</span><span class="sxs-lookup"><span data-stu-id="690f9-168">createdTime</span></span>|<span data-ttu-id="690f9-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="690f9-169">DateTimeOffset</span></span>|<span data-ttu-id="690f9-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-170">Not yet documented</span></span>|
|<span data-ttu-id="690f9-171">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="690f9-171">lastModifiedTime</span></span>|<span data-ttu-id="690f9-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="690f9-172">DateTimeOffset</span></span>|<span data-ttu-id="690f9-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-173">Not yet documented</span></span>|
|<span data-ttu-id="690f9-174">eTag</span><span class="sxs-lookup"><span data-stu-id="690f9-174">eTag</span></span>|<span data-ttu-id="690f9-175">String</span><span class="sxs-lookup"><span data-stu-id="690f9-175">String</span></span>|<span data-ttu-id="690f9-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-176">Not yet documented</span></span>|
|<span data-ttu-id="690f9-177">isDeleted</span><span class="sxs-lookup"><span data-stu-id="690f9-177">isDeleted</span></span>|<span data-ttu-id="690f9-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="690f9-178">Boolean</span></span>|<span data-ttu-id="690f9-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="690f9-179">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="690f9-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="690f9-180">Response</span></span>
<span data-ttu-id="690f9-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="690f9-181">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="690f9-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="690f9-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="690f9-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="690f9-183">Request</span></span>
<span data-ttu-id="690f9-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="690f9-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="690f9-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="690f9-185">Response</span></span>
<span data-ttu-id="690f9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="690f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





