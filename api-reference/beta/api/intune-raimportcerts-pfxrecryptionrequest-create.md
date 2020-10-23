---
title: Criar pfxRecryptionRequest
description: Criar um novo objeto pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80b5ea14a3127bdfb607c79b9435cb7ccd1b90c8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706405"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="f2e4a-103">Criar pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="f2e4a-103">Create pfxRecryptionRequest</span></span>

<span data-ttu-id="f2e4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2e4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2e4a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2e4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e4a-107">Criar um novo objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f2e4a-107">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2e4a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2e4a-108">Prerequisites</span></span>
<span data-ttu-id="f2e4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2e4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2e4a-111">Permission type</span></span>|<span data-ttu-id="f2e4a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2e4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2e4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2e4a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e4a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2e4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2e4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-116">Not supported.</span></span>|
|<span data-ttu-id="f2e4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2e4a-117">Application</span></span>|<span data-ttu-id="f2e4a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e4a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2e4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="f2e4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e4a-120">Request headers</span></span>
|<span data-ttu-id="f2e4a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2e4a-121">Header</span></span>|<span data-ttu-id="f2e4a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2e4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2e4a-123">Authorization</span></span>|<span data-ttu-id="f2e4a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2e4a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2e4a-125">Accept</span></span>|<span data-ttu-id="f2e4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e4a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e4a-127">Request body</span></span>
<span data-ttu-id="f2e4a-128">No corpo da solicitação, forneça uma representação JSON do objeto pfxRecryptionRequest.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-128">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="f2e4a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar pfxRecryptionRequest.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-129">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="f2e4a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2e4a-130">Property</span></span>|<span data-ttu-id="f2e4a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2e4a-131">Type</span></span>|<span data-ttu-id="f2e4a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2e4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e4a-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="f2e4a-133">tenantId</span></span>|<span data-ttu-id="f2e4a-134">Guid</span><span class="sxs-lookup"><span data-stu-id="f2e4a-134">Guid</span></span>|<span data-ttu-id="f2e4a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-135">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-136">userId</span><span class="sxs-lookup"><span data-stu-id="f2e4a-136">userId</span></span>|<span data-ttu-id="f2e4a-137">Guid</span><span class="sxs-lookup"><span data-stu-id="f2e4a-137">Guid</span></span>|<span data-ttu-id="f2e4a-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-138">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f2e4a-139">deviceId</span></span>|<span data-ttu-id="f2e4a-140">Guid</span><span class="sxs-lookup"><span data-stu-id="f2e4a-140">Guid</span></span>|<span data-ttu-id="f2e4a-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-141">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-142">ProfileId</span><span class="sxs-lookup"><span data-stu-id="f2e4a-142">profileId</span></span>|<span data-ttu-id="f2e4a-143">Guid</span><span class="sxs-lookup"><span data-stu-id="f2e4a-143">Guid</span></span>|<span data-ttu-id="f2e4a-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-144">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-145">identificação</span><span class="sxs-lookup"><span data-stu-id="f2e4a-145">thumbprint</span></span>|<span data-ttu-id="f2e4a-146">String</span><span class="sxs-lookup"><span data-stu-id="f2e4a-146">String</span></span>|<span data-ttu-id="f2e4a-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-147">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-148">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="f2e4a-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="f2e4a-149">String</span><span class="sxs-lookup"><span data-stu-id="f2e4a-149">String</span></span>|<span data-ttu-id="f2e4a-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-150">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-151">status</span><span class="sxs-lookup"><span data-stu-id="f2e4a-151">status</span></span>|<span data-ttu-id="f2e4a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f2e4a-152">Int32</span></span>|<span data-ttu-id="f2e4a-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-153">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="f2e4a-154">sourceType</span></span>|<span data-ttu-id="f2e4a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f2e4a-155">Int32</span></span>|<span data-ttu-id="f2e4a-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-156">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-157">createdtime</span><span class="sxs-lookup"><span data-stu-id="f2e4a-157">createdTime</span></span>|<span data-ttu-id="f2e4a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e4a-158">DateTimeOffset</span></span>|<span data-ttu-id="f2e4a-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-159">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f2e4a-160">lastModifiedTime</span></span>|<span data-ttu-id="f2e4a-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e4a-161">DateTimeOffset</span></span>|<span data-ttu-id="f2e4a-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-162">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f2e4a-163">isDeleted</span></span>|<span data-ttu-id="f2e4a-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="f2e4a-164">Boolean</span></span>|<span data-ttu-id="f2e4a-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-165">Not yet documented</span></span>|
|<span data-ttu-id="f2e4a-166">eTag</span><span class="sxs-lookup"><span data-stu-id="f2e4a-166">eTag</span></span>|<span data-ttu-id="f2e4a-167">String</span><span class="sxs-lookup"><span data-stu-id="f2e4a-167">String</span></span>|<span data-ttu-id="f2e4a-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2e4a-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f2e4a-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2e4a-169">Response</span></span>
<span data-ttu-id="f2e4a-170">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-170">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e4a-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2e4a-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2e4a-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e4a-172">Request</span></span>
<span data-ttu-id="f2e4a-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2e4a-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2e4a-174">Response</span></span>
<span data-ttu-id="f2e4a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





