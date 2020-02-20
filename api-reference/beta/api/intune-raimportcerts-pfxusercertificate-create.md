---
title: Criar pfxUserCertificate
description: Criar um novo objeto pfxUserCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44932e657452796a2e7363a8d8f33842e34de086
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161555"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="8cb1f-103">Criar pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="8cb1f-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="8cb1f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cb1f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb1f-106">Criar um novo objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="8cb1f-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cb1f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cb1f-107">Prerequisites</span></span>
<span data-ttu-id="8cb1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cb1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb1f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cb1f-110">Permission type</span></span>|<span data-ttu-id="8cb1f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cb1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb1f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cb1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cb1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cb1f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cb1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb1f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-115">Not supported.</span></span>|
|<span data-ttu-id="8cb1f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cb1f-116">Application</span></span>|<span data-ttu-id="8cb1f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb1f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb1f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cb1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="8cb1f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb1f-119">Request headers</span></span>
|<span data-ttu-id="8cb1f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cb1f-120">Header</span></span>|<span data-ttu-id="8cb1f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8cb1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb1f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cb1f-122">Authorization</span></span>|<span data-ttu-id="8cb1f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb1f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cb1f-124">Accept</span></span>|<span data-ttu-id="8cb1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb1f-126">Request body</span></span>
<span data-ttu-id="8cb1f-127">No corpo da solicitação, forneça uma representação JSON do objeto pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="8cb1f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar pfxUserCertificate.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="8cb1f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cb1f-129">Property</span></span>|<span data-ttu-id="8cb1f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cb1f-130">Type</span></span>|<span data-ttu-id="8cb1f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb1f-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="8cb1f-132">tenantId</span></span>|<span data-ttu-id="8cb1f-133">Guid</span><span class="sxs-lookup"><span data-stu-id="8cb1f-133">Guid</span></span>|<span data-ttu-id="8cb1f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-134">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-135">userId</span><span class="sxs-lookup"><span data-stu-id="8cb1f-135">userId</span></span>|<span data-ttu-id="8cb1f-136">Guid</span><span class="sxs-lookup"><span data-stu-id="8cb1f-136">Guid</span></span>|<span data-ttu-id="8cb1f-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-137">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-138">identificação</span><span class="sxs-lookup"><span data-stu-id="8cb1f-138">thumbprint</span></span>|<span data-ttu-id="8cb1f-139">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-139">String</span></span>|<span data-ttu-id="8cb1f-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-140">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="8cb1f-141">userUpn</span></span>|<span data-ttu-id="8cb1f-142">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-142">String</span></span>|<span data-ttu-id="8cb1f-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-143">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="8cb1f-144">encryptedPfxBlob</span></span>|<span data-ttu-id="8cb1f-145">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-145">String</span></span>|<span data-ttu-id="8cb1f-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-146">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="8cb1f-147">encryptedPfxPassword</span></span>|<span data-ttu-id="8cb1f-148">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-148">String</span></span>|<span data-ttu-id="8cb1f-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-149">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="8cb1f-150">certStartDate</span></span>|<span data-ttu-id="8cb1f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb1f-151">DateTimeOffset</span></span>|<span data-ttu-id="8cb1f-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-152">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="8cb1f-153">certExpirationDate</span></span>|<span data-ttu-id="8cb1f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb1f-154">DateTimeOffset</span></span>|<span data-ttu-id="8cb1f-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-155">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-156">providerName</span><span class="sxs-lookup"><span data-stu-id="8cb1f-156">providerName</span></span>|<span data-ttu-id="8cb1f-157">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-157">String</span></span>|<span data-ttu-id="8cb1f-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-158">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="8cb1f-159">encryptionKeyName</span></span>|<span data-ttu-id="8cb1f-160">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-160">String</span></span>|<span data-ttu-id="8cb1f-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-161">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="8cb1f-162">paddingScheme</span></span>|<span data-ttu-id="8cb1f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="8cb1f-163">Int32</span></span>|<span data-ttu-id="8cb1f-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-164">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-165">status</span><span class="sxs-lookup"><span data-stu-id="8cb1f-165">status</span></span>|<span data-ttu-id="8cb1f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8cb1f-166">Int32</span></span>|<span data-ttu-id="8cb1f-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-167">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-168">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="8cb1f-168">intendedPurpose</span></span>|<span data-ttu-id="8cb1f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8cb1f-169">Int32</span></span>|<span data-ttu-id="8cb1f-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-170">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-171">createdtime</span><span class="sxs-lookup"><span data-stu-id="8cb1f-171">createdTime</span></span>|<span data-ttu-id="8cb1f-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb1f-172">DateTimeOffset</span></span>|<span data-ttu-id="8cb1f-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-173">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8cb1f-174">isDeleted</span></span>|<span data-ttu-id="8cb1f-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="8cb1f-175">Boolean</span></span>|<span data-ttu-id="8cb1f-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-176">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8cb1f-177">lastModifiedTime</span></span>|<span data-ttu-id="8cb1f-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb1f-178">DateTimeOffset</span></span>|<span data-ttu-id="8cb1f-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-179">Not yet documented</span></span>|
|<span data-ttu-id="8cb1f-180">eTag</span><span class="sxs-lookup"><span data-stu-id="8cb1f-180">eTag</span></span>|<span data-ttu-id="8cb1f-181">String</span><span class="sxs-lookup"><span data-stu-id="8cb1f-181">String</span></span>|<span data-ttu-id="8cb1f-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cb1f-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8cb1f-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb1f-183">Response</span></span>
<span data-ttu-id="8cb1f-184">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb1f-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cb1f-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cb1f-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb1f-186">Request</span></span>
<span data-ttu-id="8cb1f-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8cb1f-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb1f-188">Response</span></span>
<span data-ttu-id="8cb1f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cb1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





