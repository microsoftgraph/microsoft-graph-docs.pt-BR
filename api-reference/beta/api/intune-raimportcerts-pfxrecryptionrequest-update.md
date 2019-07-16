---
title: Atualizar pfxRecryptionRequest
description: Atualiza as propriedades de um objeto pfxRecryptionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca4addaae01a6fea69d1742338e0452ed7227380
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741244"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="4e02c-103">Atualizar pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="4e02c-103">Update pfxRecryptionRequest</span></span>

> <span data-ttu-id="4e02c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e02c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e02c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e02c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e02c-106">Atualiza as propriedades de um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4e02c-106">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e02c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e02c-107">Prerequisites</span></span>
<span data-ttu-id="4e02c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e02c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e02c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e02c-110">Permission type</span></span>|<span data-ttu-id="4e02c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e02c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e02c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e02c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e02c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e02c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e02c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e02c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e02c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e02c-115">Not supported.</span></span>|
|<span data-ttu-id="4e02c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e02c-116">Application</span></span>|<span data-ttu-id="4e02c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e02c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e02c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e02c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="4e02c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e02c-119">Request headers</span></span>
|<span data-ttu-id="4e02c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e02c-120">Header</span></span>|<span data-ttu-id="4e02c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4e02c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e02c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e02c-122">Authorization</span></span>|<span data-ttu-id="4e02c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e02c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e02c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e02c-124">Accept</span></span>|<span data-ttu-id="4e02c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e02c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e02c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e02c-126">Request body</span></span>
<span data-ttu-id="4e02c-127">No corpo da solicitação, forneça uma representação JSON do objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4e02c-127">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="4e02c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="4e02c-128">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="4e02c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e02c-129">Property</span></span>|<span data-ttu-id="4e02c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e02c-130">Type</span></span>|<span data-ttu-id="4e02c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e02c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e02c-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="4e02c-132">tenantId</span></span>|<span data-ttu-id="4e02c-133">Guid</span><span class="sxs-lookup"><span data-stu-id="4e02c-133">Guid</span></span>|<span data-ttu-id="4e02c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-134">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-135">userId</span><span class="sxs-lookup"><span data-stu-id="4e02c-135">userId</span></span>|<span data-ttu-id="4e02c-136">Guid</span><span class="sxs-lookup"><span data-stu-id="4e02c-136">Guid</span></span>|<span data-ttu-id="4e02c-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-137">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="4e02c-138">deviceId</span></span>|<span data-ttu-id="4e02c-139">Guid</span><span class="sxs-lookup"><span data-stu-id="4e02c-139">Guid</span></span>|<span data-ttu-id="4e02c-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-140">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-141">ProfileId</span><span class="sxs-lookup"><span data-stu-id="4e02c-141">profileId</span></span>|<span data-ttu-id="4e02c-142">Guid</span><span class="sxs-lookup"><span data-stu-id="4e02c-142">Guid</span></span>|<span data-ttu-id="4e02c-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-143">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-144">identificação</span><span class="sxs-lookup"><span data-stu-id="4e02c-144">thumbprint</span></span>|<span data-ttu-id="4e02c-145">String</span><span class="sxs-lookup"><span data-stu-id="4e02c-145">String</span></span>|<span data-ttu-id="4e02c-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-146">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-147">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="4e02c-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="4e02c-148">String</span><span class="sxs-lookup"><span data-stu-id="4e02c-148">String</span></span>|<span data-ttu-id="4e02c-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-149">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-150">status</span><span class="sxs-lookup"><span data-stu-id="4e02c-150">status</span></span>|<span data-ttu-id="4e02c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4e02c-151">Int32</span></span>|<span data-ttu-id="4e02c-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-152">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="4e02c-153">sourceType</span></span>|<span data-ttu-id="4e02c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4e02c-154">Int32</span></span>|<span data-ttu-id="4e02c-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-155">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-156">createdtime</span><span class="sxs-lookup"><span data-stu-id="4e02c-156">createdTime</span></span>|<span data-ttu-id="4e02c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e02c-157">DateTimeOffset</span></span>|<span data-ttu-id="4e02c-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-158">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="4e02c-159">lastModifiedTime</span></span>|<span data-ttu-id="4e02c-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e02c-160">DateTimeOffset</span></span>|<span data-ttu-id="4e02c-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-161">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4e02c-162">isDeleted</span></span>|<span data-ttu-id="4e02c-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e02c-163">Boolean</span></span>|<span data-ttu-id="4e02c-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-164">Not yet documented</span></span>|
|<span data-ttu-id="4e02c-165">eTag</span><span class="sxs-lookup"><span data-stu-id="4e02c-165">eTag</span></span>|<span data-ttu-id="4e02c-166">String</span><span class="sxs-lookup"><span data-stu-id="4e02c-166">String</span></span>|<span data-ttu-id="4e02c-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e02c-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e02c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e02c-168">Response</span></span>
<span data-ttu-id="4e02c-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e02c-169">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e02c-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e02c-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e02c-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e02c-171">Request</span></span>
<span data-ttu-id="4e02c-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e02c-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e02c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e02c-173">Response</span></span>
<span data-ttu-id="4e02c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





