---
title: Criar onPremEncryptedPayload
description: Criar um novo objeto onPremEncryptedPayload.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bbc01a660ea201f4acdc2b8afc44019a7c324be
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690823"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="9b825-103">Criar onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="9b825-103">Create onPremEncryptedPayload</span></span>

<span data-ttu-id="9b825-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b825-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b825-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b825-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b825-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b825-107">Criar um novo objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="9b825-107">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b825-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b825-108">Prerequisites</span></span>
<span data-ttu-id="9b825-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b825-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b825-111">Permission type</span></span>|<span data-ttu-id="9b825-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b825-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b825-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b825-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b825-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b825-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b825-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b825-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b825-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b825-116">Not supported.</span></span>|
|<span data-ttu-id="9b825-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b825-117">Application</span></span>|<span data-ttu-id="9b825-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b825-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b825-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b825-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="9b825-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b825-120">Request headers</span></span>
|<span data-ttu-id="9b825-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b825-121">Header</span></span>|<span data-ttu-id="9b825-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b825-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b825-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b825-123">Authorization</span></span>|<span data-ttu-id="9b825-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b825-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b825-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b825-125">Accept</span></span>|<span data-ttu-id="9b825-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b825-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b825-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b825-127">Request body</span></span>
<span data-ttu-id="9b825-128">No corpo da solicitação, forneça uma representação JSON do objeto onPremEncryptedPayload.</span><span class="sxs-lookup"><span data-stu-id="9b825-128">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="9b825-129">A tabela a seguir mostra as propriedades que são necessárias ao criar onPremEncryptedPayload.</span><span class="sxs-lookup"><span data-stu-id="9b825-129">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="9b825-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b825-130">Property</span></span>|<span data-ttu-id="9b825-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b825-131">Type</span></span>|<span data-ttu-id="9b825-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b825-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b825-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="9b825-133">tenantId</span></span>|<span data-ttu-id="9b825-134">Guid</span><span class="sxs-lookup"><span data-stu-id="9b825-134">Guid</span></span>|<span data-ttu-id="9b825-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-135">Not yet documented</span></span>|
|<span data-ttu-id="9b825-136">userId</span><span class="sxs-lookup"><span data-stu-id="9b825-136">userId</span></span>|<span data-ttu-id="9b825-137">Guid</span><span class="sxs-lookup"><span data-stu-id="9b825-137">Guid</span></span>|<span data-ttu-id="9b825-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-138">Not yet documented</span></span>|
|<span data-ttu-id="9b825-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="9b825-139">deviceId</span></span>|<span data-ttu-id="9b825-140">Guid</span><span class="sxs-lookup"><span data-stu-id="9b825-140">Guid</span></span>|<span data-ttu-id="9b825-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-141">Not yet documented</span></span>|
|<span data-ttu-id="9b825-142">payloadId</span><span class="sxs-lookup"><span data-stu-id="9b825-142">payloadId</span></span>|<span data-ttu-id="9b825-143">Guid</span><span class="sxs-lookup"><span data-stu-id="9b825-143">Guid</span></span>|<span data-ttu-id="9b825-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-144">Not yet documented</span></span>|
|<span data-ttu-id="9b825-145">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="9b825-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="9b825-146">String</span><span class="sxs-lookup"><span data-stu-id="9b825-146">String</span></span>|<span data-ttu-id="9b825-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-147">Not yet documented</span></span>|
|<span data-ttu-id="9b825-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="9b825-148">cert1PayloadUUID</span></span>|<span data-ttu-id="9b825-149">String</span><span class="sxs-lookup"><span data-stu-id="9b825-149">String</span></span>|<span data-ttu-id="9b825-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-150">Not yet documented</span></span>|
|<span data-ttu-id="9b825-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="9b825-151">cert2PayloadUUID</span></span>|<span data-ttu-id="9b825-152">String</span><span class="sxs-lookup"><span data-stu-id="9b825-152">String</span></span>|<span data-ttu-id="9b825-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-153">Not yet documented</span></span>|
|<span data-ttu-id="9b825-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="9b825-154">cert3PayloadUUID</span></span>|<span data-ttu-id="9b825-155">String</span><span class="sxs-lookup"><span data-stu-id="9b825-155">String</span></span>|<span data-ttu-id="9b825-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-156">Not yet documented</span></span>|
|<span data-ttu-id="9b825-157">plisttemplate</span><span class="sxs-lookup"><span data-stu-id="9b825-157">plistTemplate</span></span>|<span data-ttu-id="9b825-158">String</span><span class="sxs-lookup"><span data-stu-id="9b825-158">String</span></span>|<span data-ttu-id="9b825-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-159">Not yet documented</span></span>|
|<span data-ttu-id="9b825-160">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="9b825-160">encryptedBlob</span></span>|<span data-ttu-id="9b825-161">Binária</span><span class="sxs-lookup"><span data-stu-id="9b825-161">Binary</span></span>|<span data-ttu-id="9b825-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-162">Not yet documented</span></span>|
|<span data-ttu-id="9b825-163">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="9b825-163">payloadVersion</span></span>|<span data-ttu-id="9b825-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9b825-164">Int32</span></span>|<span data-ttu-id="9b825-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-165">Not yet documented</span></span>|
|<span data-ttu-id="9b825-166">status</span><span class="sxs-lookup"><span data-stu-id="9b825-166">status</span></span>|<span data-ttu-id="9b825-167">Int32</span><span class="sxs-lookup"><span data-stu-id="9b825-167">Int32</span></span>|<span data-ttu-id="9b825-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-168">Not yet documented</span></span>|
|<span data-ttu-id="9b825-169">createdtime</span><span class="sxs-lookup"><span data-stu-id="9b825-169">createdTime</span></span>|<span data-ttu-id="9b825-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b825-170">DateTimeOffset</span></span>|<span data-ttu-id="9b825-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-171">Not yet documented</span></span>|
|<span data-ttu-id="9b825-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="9b825-172">lastModifiedTime</span></span>|<span data-ttu-id="9b825-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b825-173">DateTimeOffset</span></span>|<span data-ttu-id="9b825-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-174">Not yet documented</span></span>|
|<span data-ttu-id="9b825-175">eTag</span><span class="sxs-lookup"><span data-stu-id="9b825-175">eTag</span></span>|<span data-ttu-id="9b825-176">String</span><span class="sxs-lookup"><span data-stu-id="9b825-176">String</span></span>|<span data-ttu-id="9b825-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-177">Not yet documented</span></span>|
|<span data-ttu-id="9b825-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9b825-178">isDeleted</span></span>|<span data-ttu-id="9b825-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b825-179">Boolean</span></span>|<span data-ttu-id="9b825-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b825-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b825-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b825-181">Response</span></span>
<span data-ttu-id="9b825-182">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b825-182">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b825-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b825-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b825-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b825-184">Request</span></span>
<span data-ttu-id="9b825-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b825-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b825-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b825-186">Response</span></span>
<span data-ttu-id="9b825-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b825-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





