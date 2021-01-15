---
title: Atualizar cloudPcProvisioningPolicy
description: Atualizar as propriedades de um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b070f24cc91562626467aa3b4645e67fffd6d13c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872727"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="50f79-103">Atualizar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="50f79-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="50f79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50f79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50f79-105">Atualizar as propriedades de um [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="50f79-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="50f79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50f79-106">Permissions</span></span>

<span data-ttu-id="50f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50f79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50f79-109">Permission type</span></span>|<span data-ttu-id="50f79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50f79-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50f79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50f79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50f79-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f79-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="50f79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50f79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50f79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50f79-114">Not supported.</span></span>|
|<span data-ttu-id="50f79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50f79-115">Application</span></span>|<span data-ttu-id="50f79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50f79-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50f79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50f79-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="50f79-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50f79-118">Request headers</span></span>

| <span data-ttu-id="50f79-119">Nome</span><span class="sxs-lookup"><span data-stu-id="50f79-119">Name</span></span>          | <span data-ttu-id="50f79-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f79-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="50f79-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50f79-121">Authorization</span></span> | <span data-ttu-id="50f79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f79-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50f79-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50f79-124">Content-Type</span></span>  | <span data-ttu-id="50f79-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f79-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50f79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50f79-127">Request body</span></span>

<span data-ttu-id="50f79-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="50f79-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="50f79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="50f79-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="50f79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50f79-130">Property</span></span>|<span data-ttu-id="50f79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="50f79-131">Type</span></span>|<span data-ttu-id="50f79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50f79-133">displayName</span><span class="sxs-lookup"><span data-stu-id="50f79-133">displayName</span></span>|<span data-ttu-id="50f79-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f79-134">String</span></span>|<span data-ttu-id="50f79-135">O nome de exibição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="50f79-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="50f79-136">description</span><span class="sxs-lookup"><span data-stu-id="50f79-136">description</span></span>|<span data-ttu-id="50f79-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f79-137">String</span></span>|<span data-ttu-id="50f79-138">A descrição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="50f79-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="50f79-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="50f79-139">onPremisesConnectionId</span></span>|<span data-ttu-id="50f79-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f79-140">String</span></span>|<span data-ttu-id="50f79-141">A ID da cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="50f79-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="50f79-142">Para garantir que os computadores na nuvem tenham conectividade de rede e que in joinam no domínio, escolha uma conexão com uma rede virtual validada pelo serviço de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="50f79-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="50f79-143">imageId</span><span class="sxs-lookup"><span data-stu-id="50f79-143">imageId</span></span>|<span data-ttu-id="50f79-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f79-144">String</span></span>|<span data-ttu-id="50f79-145">A ID da imagem do sistema operacional que você deseja provisionar em PCs na nuvem.</span><span class="sxs-lookup"><span data-stu-id="50f79-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="50f79-146">O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="50f79-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="50f79-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="50f79-147">imageDisplayName</span></span>|<span data-ttu-id="50f79-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f79-148">String</span></span>|<span data-ttu-id="50f79-149">O nome de exibição da imagem do sistema operacional que você está provisionando.</span><span class="sxs-lookup"><span data-stu-id="50f79-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="50f79-150">imageType</span><span class="sxs-lookup"><span data-stu-id="50f79-150">imageType</span></span>|<span data-ttu-id="50f79-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="50f79-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="50f79-152">O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="50f79-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="50f79-153">Os valores possíveis são: `gallery` e `custom`.</span><span class="sxs-lookup"><span data-stu-id="50f79-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="50f79-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f79-154">Response</span></span>

<span data-ttu-id="50f79-155">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50f79-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50f79-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="50f79-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50f79-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50f79-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="50f79-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="50f79-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_provisioningpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
Content-Type: application/json
Content-length: 308

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
}
```
# <a name="c"></a>[<span data-ttu-id="50f79-159">C#</span><span class="sxs-lookup"><span data-stu-id="50f79-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50f79-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50f79-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50f79-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50f79-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50f79-162">Java</span><span class="sxs-lookup"><span data-stu-id="50f79-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50f79-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f79-163">Response</span></span>

<span data-ttu-id="50f79-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="50f79-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "8931f750-f750-8931-50f7-318950f7ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
}
```
