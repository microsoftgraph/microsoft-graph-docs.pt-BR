---
title: Atualizar pfxRecryptionRequest
description: Atualiza as propriedades de um objeto pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc07258a39547ca6d7833dec2bee205b12fa69a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698481"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="a6bd2-103">Atualizar pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="a6bd2-103">Update pfxRecryptionRequest</span></span>

<span data-ttu-id="a6bd2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6bd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6bd2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6bd2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6bd2-107">Atualiza as propriedades de um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a6bd2-107">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6bd2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6bd2-108">Prerequisites</span></span>
<span data-ttu-id="a6bd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6bd2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6bd2-111">Permission type</span></span>|<span data-ttu-id="a6bd2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6bd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6bd2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6bd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6bd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6bd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6bd2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6bd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6bd2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-116">Not supported.</span></span>|
|<span data-ttu-id="a6bd2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6bd2-117">Application</span></span>|<span data-ttu-id="a6bd2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6bd2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6bd2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6bd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="a6bd2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6bd2-120">Request headers</span></span>
|<span data-ttu-id="a6bd2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6bd2-121">Header</span></span>|<span data-ttu-id="a6bd2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6bd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6bd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6bd2-123">Authorization</span></span>|<span data-ttu-id="a6bd2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6bd2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6bd2-125">Accept</span></span>|<span data-ttu-id="a6bd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6bd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6bd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6bd2-127">Request body</span></span>
<span data-ttu-id="a6bd2-128">No corpo da solicitação, forneça uma representação JSON do objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a6bd2-128">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="a6bd2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a6bd2-129">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="a6bd2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6bd2-130">Property</span></span>|<span data-ttu-id="a6bd2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6bd2-131">Type</span></span>|<span data-ttu-id="a6bd2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6bd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6bd2-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="a6bd2-133">tenantId</span></span>|<span data-ttu-id="a6bd2-134">Guid</span><span class="sxs-lookup"><span data-stu-id="a6bd2-134">Guid</span></span>|<span data-ttu-id="a6bd2-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-135">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-136">userId</span><span class="sxs-lookup"><span data-stu-id="a6bd2-136">userId</span></span>|<span data-ttu-id="a6bd2-137">Guid</span><span class="sxs-lookup"><span data-stu-id="a6bd2-137">Guid</span></span>|<span data-ttu-id="a6bd2-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-138">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="a6bd2-139">deviceId</span></span>|<span data-ttu-id="a6bd2-140">Guid</span><span class="sxs-lookup"><span data-stu-id="a6bd2-140">Guid</span></span>|<span data-ttu-id="a6bd2-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-141">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-142">ProfileId</span><span class="sxs-lookup"><span data-stu-id="a6bd2-142">profileId</span></span>|<span data-ttu-id="a6bd2-143">Guid</span><span class="sxs-lookup"><span data-stu-id="a6bd2-143">Guid</span></span>|<span data-ttu-id="a6bd2-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-144">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-145">identificação</span><span class="sxs-lookup"><span data-stu-id="a6bd2-145">thumbprint</span></span>|<span data-ttu-id="a6bd2-146">String</span><span class="sxs-lookup"><span data-stu-id="a6bd2-146">String</span></span>|<span data-ttu-id="a6bd2-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-147">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-148">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="a6bd2-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="a6bd2-149">String</span><span class="sxs-lookup"><span data-stu-id="a6bd2-149">String</span></span>|<span data-ttu-id="a6bd2-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-150">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-151">status</span><span class="sxs-lookup"><span data-stu-id="a6bd2-151">status</span></span>|<span data-ttu-id="a6bd2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a6bd2-152">Int32</span></span>|<span data-ttu-id="a6bd2-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-153">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="a6bd2-154">sourceType</span></span>|<span data-ttu-id="a6bd2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a6bd2-155">Int32</span></span>|<span data-ttu-id="a6bd2-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-156">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-157">createdtime</span><span class="sxs-lookup"><span data-stu-id="a6bd2-157">createdTime</span></span>|<span data-ttu-id="a6bd2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6bd2-158">DateTimeOffset</span></span>|<span data-ttu-id="a6bd2-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-159">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a6bd2-160">lastModifiedTime</span></span>|<span data-ttu-id="a6bd2-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6bd2-161">DateTimeOffset</span></span>|<span data-ttu-id="a6bd2-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-162">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a6bd2-163">isDeleted</span></span>|<span data-ttu-id="a6bd2-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6bd2-164">Boolean</span></span>|<span data-ttu-id="a6bd2-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-165">Not yet documented</span></span>|
|<span data-ttu-id="a6bd2-166">eTag</span><span class="sxs-lookup"><span data-stu-id="a6bd2-166">eTag</span></span>|<span data-ttu-id="a6bd2-167">String</span><span class="sxs-lookup"><span data-stu-id="a6bd2-167">String</span></span>|<span data-ttu-id="a6bd2-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6bd2-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6bd2-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6bd2-169">Response</span></span>
<span data-ttu-id="a6bd2-170">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-170">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6bd2-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6bd2-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6bd2-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6bd2-172">Request</span></span>
<span data-ttu-id="a6bd2-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
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

### <a name="response"></a><span data-ttu-id="a6bd2-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6bd2-174">Response</span></span>
<span data-ttu-id="a6bd2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6bd2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





