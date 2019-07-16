---
title: Atualizar onPremEncryptedPayload
description: Atualiza as propriedades de um objeto onPremEncryptedPayload.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50048080072c8bcc7feb08cac69d74a18460c19
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741263"
---
# <a name="update-onpremencryptedpayload"></a><span data-ttu-id="ef318-103">Atualizar onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="ef318-103">Update onPremEncryptedPayload</span></span>

> <span data-ttu-id="ef318-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef318-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef318-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef318-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef318-106">Atualiza as propriedades de um objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="ef318-106">Update the properties of a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef318-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef318-107">Prerequisites</span></span>
<span data-ttu-id="ef318-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef318-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef318-110">Permission type</span></span>|<span data-ttu-id="ef318-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef318-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef318-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef318-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef318-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef318-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef318-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef318-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef318-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef318-115">Not supported.</span></span>|
|<span data-ttu-id="ef318-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef318-116">Application</span></span>|<span data-ttu-id="ef318-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef318-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef318-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef318-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="ef318-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef318-119">Request headers</span></span>
|<span data-ttu-id="ef318-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef318-120">Header</span></span>|<span data-ttu-id="ef318-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef318-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef318-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef318-122">Authorization</span></span>|<span data-ttu-id="ef318-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef318-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef318-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef318-124">Accept</span></span>|<span data-ttu-id="ef318-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef318-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef318-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef318-126">Request body</span></span>
<span data-ttu-id="ef318-127">No corpo da solicitação, forneça uma representação JSON do objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="ef318-127">In the request body, supply a JSON representation for the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

<span data-ttu-id="ef318-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span><span class="sxs-lookup"><span data-stu-id="ef318-128">The following table shows the properties that are required when you create the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

|<span data-ttu-id="ef318-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef318-129">Property</span></span>|<span data-ttu-id="ef318-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef318-130">Type</span></span>|<span data-ttu-id="ef318-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef318-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef318-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="ef318-132">tenantId</span></span>|<span data-ttu-id="ef318-133">Guid</span><span class="sxs-lookup"><span data-stu-id="ef318-133">Guid</span></span>|<span data-ttu-id="ef318-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-134">Not yet documented</span></span>|
|<span data-ttu-id="ef318-135">userId</span><span class="sxs-lookup"><span data-stu-id="ef318-135">userId</span></span>|<span data-ttu-id="ef318-136">Guid</span><span class="sxs-lookup"><span data-stu-id="ef318-136">Guid</span></span>|<span data-ttu-id="ef318-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-137">Not yet documented</span></span>|
|<span data-ttu-id="ef318-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="ef318-138">deviceId</span></span>|<span data-ttu-id="ef318-139">Guid</span><span class="sxs-lookup"><span data-stu-id="ef318-139">Guid</span></span>|<span data-ttu-id="ef318-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-140">Not yet documented</span></span>|
|<span data-ttu-id="ef318-141">payloadId</span><span class="sxs-lookup"><span data-stu-id="ef318-141">payloadId</span></span>|<span data-ttu-id="ef318-142">Guid</span><span class="sxs-lookup"><span data-stu-id="ef318-142">Guid</span></span>|<span data-ttu-id="ef318-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-143">Not yet documented</span></span>|
|<span data-ttu-id="ef318-144">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="ef318-144">deviceKeyThumbprint</span></span>|<span data-ttu-id="ef318-145">String</span><span class="sxs-lookup"><span data-stu-id="ef318-145">String</span></span>|<span data-ttu-id="ef318-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-146">Not yet documented</span></span>|
|<span data-ttu-id="ef318-147">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="ef318-147">cert1PayloadUUID</span></span>|<span data-ttu-id="ef318-148">String</span><span class="sxs-lookup"><span data-stu-id="ef318-148">String</span></span>|<span data-ttu-id="ef318-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-149">Not yet documented</span></span>|
|<span data-ttu-id="ef318-150">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="ef318-150">cert2PayloadUUID</span></span>|<span data-ttu-id="ef318-151">String</span><span class="sxs-lookup"><span data-stu-id="ef318-151">String</span></span>|<span data-ttu-id="ef318-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-152">Not yet documented</span></span>|
|<span data-ttu-id="ef318-153">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="ef318-153">cert3PayloadUUID</span></span>|<span data-ttu-id="ef318-154">String</span><span class="sxs-lookup"><span data-stu-id="ef318-154">String</span></span>|<span data-ttu-id="ef318-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-155">Not yet documented</span></span>|
|<span data-ttu-id="ef318-156">plisttemplate</span><span class="sxs-lookup"><span data-stu-id="ef318-156">plistTemplate</span></span>|<span data-ttu-id="ef318-157">String</span><span class="sxs-lookup"><span data-stu-id="ef318-157">String</span></span>|<span data-ttu-id="ef318-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-158">Not yet documented</span></span>|
|<span data-ttu-id="ef318-159">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="ef318-159">encryptedBlob</span></span>|<span data-ttu-id="ef318-160">Binária</span><span class="sxs-lookup"><span data-stu-id="ef318-160">Binary</span></span>|<span data-ttu-id="ef318-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-161">Not yet documented</span></span>|
|<span data-ttu-id="ef318-162">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="ef318-162">payloadVersion</span></span>|<span data-ttu-id="ef318-163">Int32</span><span class="sxs-lookup"><span data-stu-id="ef318-163">Int32</span></span>|<span data-ttu-id="ef318-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-164">Not yet documented</span></span>|
|<span data-ttu-id="ef318-165">status</span><span class="sxs-lookup"><span data-stu-id="ef318-165">status</span></span>|<span data-ttu-id="ef318-166">Int32</span><span class="sxs-lookup"><span data-stu-id="ef318-166">Int32</span></span>|<span data-ttu-id="ef318-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-167">Not yet documented</span></span>|
|<span data-ttu-id="ef318-168">createdtime</span><span class="sxs-lookup"><span data-stu-id="ef318-168">createdTime</span></span>|<span data-ttu-id="ef318-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef318-169">DateTimeOffset</span></span>|<span data-ttu-id="ef318-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-170">Not yet documented</span></span>|
|<span data-ttu-id="ef318-171">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ef318-171">lastModifiedTime</span></span>|<span data-ttu-id="ef318-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef318-172">DateTimeOffset</span></span>|<span data-ttu-id="ef318-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-173">Not yet documented</span></span>|
|<span data-ttu-id="ef318-174">eTag</span><span class="sxs-lookup"><span data-stu-id="ef318-174">eTag</span></span>|<span data-ttu-id="ef318-175">String</span><span class="sxs-lookup"><span data-stu-id="ef318-175">String</span></span>|<span data-ttu-id="ef318-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-176">Not yet documented</span></span>|
|<span data-ttu-id="ef318-177">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ef318-177">isDeleted</span></span>|<span data-ttu-id="ef318-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef318-178">Boolean</span></span>|<span data-ttu-id="ef318-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef318-179">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ef318-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef318-180">Response</span></span>
<span data-ttu-id="ef318-181">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef318-181">If successful, this method returns a `200 OK` response code and an updated [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef318-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef318-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef318-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef318-183">Request</span></span>
<span data-ttu-id="ef318-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef318-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
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

### <a name="response"></a><span data-ttu-id="ef318-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef318-185">Response</span></span>
<span data-ttu-id="ef318-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef318-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





