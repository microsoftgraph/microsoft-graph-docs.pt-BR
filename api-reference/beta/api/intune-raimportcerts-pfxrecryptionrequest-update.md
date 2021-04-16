---
title: Atualizar pfxRecryptionRequest
description: Atualize as propriedades de um objeto pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb7c4856f0b383a6273c2d9d885efcf676532c3f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868369"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="f546f-103">Atualizar pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="f546f-103">Update pfxRecryptionRequest</span></span>

<span data-ttu-id="f546f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f546f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f546f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f546f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f546f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f546f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f546f-107">Atualize as propriedades de um [objeto pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f546f-107">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f546f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f546f-108">Prerequisites</span></span>
<span data-ttu-id="f546f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f546f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f546f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f546f-111">Permission type</span></span>|<span data-ttu-id="f546f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f546f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f546f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f546f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f546f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f546f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f546f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f546f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f546f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f546f-116">Not supported.</span></span>|
|<span data-ttu-id="f546f-117">Application</span><span class="sxs-lookup"><span data-stu-id="f546f-117">Application</span></span>|<span data-ttu-id="f546f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f546f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f546f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f546f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="f546f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f546f-120">Request headers</span></span>
|<span data-ttu-id="f546f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f546f-121">Header</span></span>|<span data-ttu-id="f546f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f546f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f546f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f546f-123">Authorization</span></span>|<span data-ttu-id="f546f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f546f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f546f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f546f-125">Accept</span></span>|<span data-ttu-id="f546f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f546f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f546f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f546f-127">Request body</span></span>
<span data-ttu-id="f546f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f546f-128">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="f546f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f546f-129">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="f546f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f546f-130">Property</span></span>|<span data-ttu-id="f546f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f546f-131">Type</span></span>|<span data-ttu-id="f546f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f546f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f546f-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="f546f-133">tenantId</span></span>|<span data-ttu-id="f546f-134">Guid</span><span class="sxs-lookup"><span data-stu-id="f546f-134">Guid</span></span>|<span data-ttu-id="f546f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-135">Not yet documented</span></span>|
|<span data-ttu-id="f546f-136">userId</span><span class="sxs-lookup"><span data-stu-id="f546f-136">userId</span></span>|<span data-ttu-id="f546f-137">Guid</span><span class="sxs-lookup"><span data-stu-id="f546f-137">Guid</span></span>|<span data-ttu-id="f546f-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-138">Not yet documented</span></span>|
|<span data-ttu-id="f546f-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f546f-139">deviceId</span></span>|<span data-ttu-id="f546f-140">Guid</span><span class="sxs-lookup"><span data-stu-id="f546f-140">Guid</span></span>|<span data-ttu-id="f546f-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-141">Not yet documented</span></span>|
|<span data-ttu-id="f546f-142">profileId</span><span class="sxs-lookup"><span data-stu-id="f546f-142">profileId</span></span>|<span data-ttu-id="f546f-143">Guid</span><span class="sxs-lookup"><span data-stu-id="f546f-143">Guid</span></span>|<span data-ttu-id="f546f-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-144">Not yet documented</span></span>|
|<span data-ttu-id="f546f-145">thumbprint</span><span class="sxs-lookup"><span data-stu-id="f546f-145">thumbprint</span></span>|<span data-ttu-id="f546f-146">String</span><span class="sxs-lookup"><span data-stu-id="f546f-146">String</span></span>|<span data-ttu-id="f546f-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-147">Not yet documented</span></span>|
|<span data-ttu-id="f546f-148">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="f546f-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="f546f-149">String</span><span class="sxs-lookup"><span data-stu-id="f546f-149">String</span></span>|<span data-ttu-id="f546f-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-150">Not yet documented</span></span>|
|<span data-ttu-id="f546f-151">status</span><span class="sxs-lookup"><span data-stu-id="f546f-151">status</span></span>|<span data-ttu-id="f546f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f546f-152">Int32</span></span>|<span data-ttu-id="f546f-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-153">Not yet documented</span></span>|
|<span data-ttu-id="f546f-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="f546f-154">sourceType</span></span>|<span data-ttu-id="f546f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f546f-155">Int32</span></span>|<span data-ttu-id="f546f-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-156">Not yet documented</span></span>|
|<span data-ttu-id="f546f-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="f546f-157">createdTime</span></span>|<span data-ttu-id="f546f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f546f-158">DateTimeOffset</span></span>|<span data-ttu-id="f546f-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-159">Not yet documented</span></span>|
|<span data-ttu-id="f546f-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f546f-160">lastModifiedTime</span></span>|<span data-ttu-id="f546f-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f546f-161">DateTimeOffset</span></span>|<span data-ttu-id="f546f-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-162">Not yet documented</span></span>|
|<span data-ttu-id="f546f-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f546f-163">isDeleted</span></span>|<span data-ttu-id="f546f-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="f546f-164">Boolean</span></span>|<span data-ttu-id="f546f-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-165">Not yet documented</span></span>|
|<span data-ttu-id="f546f-166">eTag</span><span class="sxs-lookup"><span data-stu-id="f546f-166">eTag</span></span>|<span data-ttu-id="f546f-167">String</span><span class="sxs-lookup"><span data-stu-id="f546f-167">String</span></span>|<span data-ttu-id="f546f-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f546f-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f546f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f546f-169">Response</span></span>
<span data-ttu-id="f546f-170">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f546f-170">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f546f-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f546f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f546f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f546f-172">Request</span></span>
<span data-ttu-id="f546f-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f546f-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f546f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f546f-174">Response</span></span>
<span data-ttu-id="f546f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f546f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




