---
title: Criar pfxUserCertificate
description: Criar um novo objeto pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbfd3a3ed0166771b8c7dd77043b212fb36f4be8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285153"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="1efac-103">Criar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="1efac-103">Create pfxUserCertificate</span></span>

<span data-ttu-id="1efac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1efac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1efac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1efac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1efac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1efac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1efac-107">Criar um novo objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1efac-107">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1efac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1efac-108">Prerequisites</span></span>
<span data-ttu-id="1efac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1efac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1efac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1efac-111">Permission type</span></span>|<span data-ttu-id="1efac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1efac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1efac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1efac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1efac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1efac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1efac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1efac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1efac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1efac-116">Not supported.</span></span>|
|<span data-ttu-id="1efac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1efac-117">Application</span></span>|<span data-ttu-id="1efac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1efac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1efac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1efac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="1efac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1efac-120">Request headers</span></span>
|<span data-ttu-id="1efac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1efac-121">Header</span></span>|<span data-ttu-id="1efac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1efac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1efac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1efac-123">Authorization</span></span>|<span data-ttu-id="1efac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1efac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1efac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1efac-125">Accept</span></span>|<span data-ttu-id="1efac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1efac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1efac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1efac-127">Request body</span></span>
<span data-ttu-id="1efac-128">No corpo da solicitação, forneça uma representação JSON do objeto pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="1efac-128">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="1efac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="1efac-129">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="1efac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1efac-130">Property</span></span>|<span data-ttu-id="1efac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1efac-131">Type</span></span>|<span data-ttu-id="1efac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1efac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efac-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="1efac-133">tenantId</span></span>|<span data-ttu-id="1efac-134">Guid</span><span class="sxs-lookup"><span data-stu-id="1efac-134">Guid</span></span>|<span data-ttu-id="1efac-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-135">Not yet documented</span></span>|
|<span data-ttu-id="1efac-136">userId</span><span class="sxs-lookup"><span data-stu-id="1efac-136">userId</span></span>|<span data-ttu-id="1efac-137">Guid</span><span class="sxs-lookup"><span data-stu-id="1efac-137">Guid</span></span>|<span data-ttu-id="1efac-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-138">Not yet documented</span></span>|
|<span data-ttu-id="1efac-139">identificação</span><span class="sxs-lookup"><span data-stu-id="1efac-139">thumbprint</span></span>|<span data-ttu-id="1efac-140">String</span><span class="sxs-lookup"><span data-stu-id="1efac-140">String</span></span>|<span data-ttu-id="1efac-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-141">Not yet documented</span></span>|
|<span data-ttu-id="1efac-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="1efac-142">userUpn</span></span>|<span data-ttu-id="1efac-143">String</span><span class="sxs-lookup"><span data-stu-id="1efac-143">String</span></span>|<span data-ttu-id="1efac-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-144">Not yet documented</span></span>|
|<span data-ttu-id="1efac-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="1efac-145">encryptedPfxBlob</span></span>|<span data-ttu-id="1efac-146">String</span><span class="sxs-lookup"><span data-stu-id="1efac-146">String</span></span>|<span data-ttu-id="1efac-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-147">Not yet documented</span></span>|
|<span data-ttu-id="1efac-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="1efac-148">encryptedPfxPassword</span></span>|<span data-ttu-id="1efac-149">String</span><span class="sxs-lookup"><span data-stu-id="1efac-149">String</span></span>|<span data-ttu-id="1efac-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-150">Not yet documented</span></span>|
|<span data-ttu-id="1efac-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="1efac-151">certStartDate</span></span>|<span data-ttu-id="1efac-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efac-152">DateTimeOffset</span></span>|<span data-ttu-id="1efac-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-153">Not yet documented</span></span>|
|<span data-ttu-id="1efac-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="1efac-154">certExpirationDate</span></span>|<span data-ttu-id="1efac-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efac-155">DateTimeOffset</span></span>|<span data-ttu-id="1efac-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-156">Not yet documented</span></span>|
|<span data-ttu-id="1efac-157">providerName</span><span class="sxs-lookup"><span data-stu-id="1efac-157">providerName</span></span>|<span data-ttu-id="1efac-158">String</span><span class="sxs-lookup"><span data-stu-id="1efac-158">String</span></span>|<span data-ttu-id="1efac-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-159">Not yet documented</span></span>|
|<span data-ttu-id="1efac-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="1efac-160">encryptionKeyName</span></span>|<span data-ttu-id="1efac-161">String</span><span class="sxs-lookup"><span data-stu-id="1efac-161">String</span></span>|<span data-ttu-id="1efac-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-162">Not yet documented</span></span>|
|<span data-ttu-id="1efac-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="1efac-163">paddingScheme</span></span>|<span data-ttu-id="1efac-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1efac-164">Int32</span></span>|<span data-ttu-id="1efac-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-165">Not yet documented</span></span>|
|<span data-ttu-id="1efac-166">status</span><span class="sxs-lookup"><span data-stu-id="1efac-166">status</span></span>|<span data-ttu-id="1efac-167">Int32</span><span class="sxs-lookup"><span data-stu-id="1efac-167">Int32</span></span>|<span data-ttu-id="1efac-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-168">Not yet documented</span></span>|
|<span data-ttu-id="1efac-169">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="1efac-169">intendedPurpose</span></span>|<span data-ttu-id="1efac-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1efac-170">Int32</span></span>|<span data-ttu-id="1efac-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-171">Not yet documented</span></span>|
|<span data-ttu-id="1efac-172">createdtime</span><span class="sxs-lookup"><span data-stu-id="1efac-172">createdTime</span></span>|<span data-ttu-id="1efac-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efac-173">DateTimeOffset</span></span>|<span data-ttu-id="1efac-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-174">Not yet documented</span></span>|
|<span data-ttu-id="1efac-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1efac-175">isDeleted</span></span>|<span data-ttu-id="1efac-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="1efac-176">Boolean</span></span>|<span data-ttu-id="1efac-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-177">Not yet documented</span></span>|
|<span data-ttu-id="1efac-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1efac-178">lastModifiedTime</span></span>|<span data-ttu-id="1efac-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efac-179">DateTimeOffset</span></span>|<span data-ttu-id="1efac-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-180">Not yet documented</span></span>|
|<span data-ttu-id="1efac-181">eTag</span><span class="sxs-lookup"><span data-stu-id="1efac-181">eTag</span></span>|<span data-ttu-id="1efac-182">String</span><span class="sxs-lookup"><span data-stu-id="1efac-182">String</span></span>|<span data-ttu-id="1efac-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1efac-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1efac-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="1efac-184">Response</span></span>
<span data-ttu-id="1efac-185">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1efac-185">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1efac-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1efac-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="1efac-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1efac-187">Request</span></span>
<span data-ttu-id="1efac-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1efac-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1efac-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="1efac-189">Response</span></span>
<span data-ttu-id="1efac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1efac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




