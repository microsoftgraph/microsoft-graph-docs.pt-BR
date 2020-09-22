---
title: Criar pfxRecryptionRequest
description: Criar um novo objeto pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b961e11bf5ee6fc34e8e9d9fe9e70e5b0f3dd7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093242"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="89ef7-103">Criar pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="89ef7-103">Create pfxRecryptionRequest</span></span>

<span data-ttu-id="89ef7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89ef7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89ef7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89ef7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89ef7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89ef7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ef7-107">Criar um novo objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="89ef7-107">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89ef7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89ef7-108">Prerequisites</span></span>
<span data-ttu-id="89ef7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ef7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ef7-111">Permission type</span></span>|<span data-ttu-id="89ef7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89ef7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ef7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ef7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89ef7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ef7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89ef7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89ef7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ef7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ef7-116">Not supported.</span></span>|
|<span data-ttu-id="89ef7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89ef7-117">Application</span></span>|<span data-ttu-id="89ef7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ef7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ef7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ef7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="89ef7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89ef7-120">Request headers</span></span>
|<span data-ttu-id="89ef7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89ef7-121">Header</span></span>|<span data-ttu-id="89ef7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89ef7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89ef7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ef7-123">Authorization</span></span>|<span data-ttu-id="89ef7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ef7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89ef7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89ef7-125">Accept</span></span>|<span data-ttu-id="89ef7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89ef7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ef7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ef7-127">Request body</span></span>
<span data-ttu-id="89ef7-128">No corpo da solicitação, forneça uma representação JSON do objeto pfxRecryptionRequest.</span><span class="sxs-lookup"><span data-stu-id="89ef7-128">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="89ef7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar pfxRecryptionRequest.</span><span class="sxs-lookup"><span data-stu-id="89ef7-129">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="89ef7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89ef7-130">Property</span></span>|<span data-ttu-id="89ef7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89ef7-131">Type</span></span>|<span data-ttu-id="89ef7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ef7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ef7-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="89ef7-133">tenantId</span></span>|<span data-ttu-id="89ef7-134">Guid</span><span class="sxs-lookup"><span data-stu-id="89ef7-134">Guid</span></span>|<span data-ttu-id="89ef7-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-135">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-136">userId</span><span class="sxs-lookup"><span data-stu-id="89ef7-136">userId</span></span>|<span data-ttu-id="89ef7-137">Guid</span><span class="sxs-lookup"><span data-stu-id="89ef7-137">Guid</span></span>|<span data-ttu-id="89ef7-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-138">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="89ef7-139">deviceId</span></span>|<span data-ttu-id="89ef7-140">Guid</span><span class="sxs-lookup"><span data-stu-id="89ef7-140">Guid</span></span>|<span data-ttu-id="89ef7-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-141">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-142">ProfileId</span><span class="sxs-lookup"><span data-stu-id="89ef7-142">profileId</span></span>|<span data-ttu-id="89ef7-143">Guid</span><span class="sxs-lookup"><span data-stu-id="89ef7-143">Guid</span></span>|<span data-ttu-id="89ef7-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-144">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-145">identificação</span><span class="sxs-lookup"><span data-stu-id="89ef7-145">thumbprint</span></span>|<span data-ttu-id="89ef7-146">String</span><span class="sxs-lookup"><span data-stu-id="89ef7-146">String</span></span>|<span data-ttu-id="89ef7-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-147">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-148">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="89ef7-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="89ef7-149">String</span><span class="sxs-lookup"><span data-stu-id="89ef7-149">String</span></span>|<span data-ttu-id="89ef7-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-150">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-151">status</span><span class="sxs-lookup"><span data-stu-id="89ef7-151">status</span></span>|<span data-ttu-id="89ef7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="89ef7-152">Int32</span></span>|<span data-ttu-id="89ef7-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-153">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="89ef7-154">sourceType</span></span>|<span data-ttu-id="89ef7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="89ef7-155">Int32</span></span>|<span data-ttu-id="89ef7-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-156">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-157">createdtime</span><span class="sxs-lookup"><span data-stu-id="89ef7-157">createdTime</span></span>|<span data-ttu-id="89ef7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89ef7-158">DateTimeOffset</span></span>|<span data-ttu-id="89ef7-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-159">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="89ef7-160">lastModifiedTime</span></span>|<span data-ttu-id="89ef7-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89ef7-161">DateTimeOffset</span></span>|<span data-ttu-id="89ef7-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-162">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="89ef7-163">isDeleted</span></span>|<span data-ttu-id="89ef7-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="89ef7-164">Boolean</span></span>|<span data-ttu-id="89ef7-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-165">Not yet documented</span></span>|
|<span data-ttu-id="89ef7-166">eTag</span><span class="sxs-lookup"><span data-stu-id="89ef7-166">eTag</span></span>|<span data-ttu-id="89ef7-167">String</span><span class="sxs-lookup"><span data-stu-id="89ef7-167">String</span></span>|<span data-ttu-id="89ef7-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89ef7-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89ef7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ef7-169">Response</span></span>
<span data-ttu-id="89ef7-170">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ef7-170">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ef7-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89ef7-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="89ef7-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89ef7-172">Request</span></span>
<span data-ttu-id="89ef7-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89ef7-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxRecryptionRequests
Content-type: application/json
Content-length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="89ef7-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ef7-174">Response</span></span>
<span data-ttu-id="89ef7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89ef7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```






