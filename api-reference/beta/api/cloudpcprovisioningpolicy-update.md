---
title: Atualizar cloudPcProvisioningPolicy
description: Atualize as propriedades de um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 935dd01d22afd6b6ef916a328c40b4fa08d978fd
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546396"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="02442-103">Atualizar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="02442-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="02442-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02442-105">Atualize as propriedades de [um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="02442-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="02442-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02442-106">Permissions</span></span>

<span data-ttu-id="02442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02442-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02442-109">Permission type</span></span>|<span data-ttu-id="02442-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02442-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02442-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02442-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02442-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02442-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="02442-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02442-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02442-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02442-114">Not supported.</span></span>|
|<span data-ttu-id="02442-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02442-115">Application</span></span>|<span data-ttu-id="02442-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02442-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02442-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02442-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="02442-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02442-118">Request headers</span></span>

| <span data-ttu-id="02442-119">Nome</span><span class="sxs-lookup"><span data-stu-id="02442-119">Name</span></span>          | <span data-ttu-id="02442-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="02442-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="02442-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02442-121">Authorization</span></span> | <span data-ttu-id="02442-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02442-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="02442-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02442-124">Content-Type</span></span>  | <span data-ttu-id="02442-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02442-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02442-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02442-127">Request body</span></span>

<span data-ttu-id="02442-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="02442-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="02442-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="02442-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="02442-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02442-130">Property</span></span>|<span data-ttu-id="02442-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02442-131">Type</span></span>|<span data-ttu-id="02442-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02442-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02442-133">displayName</span><span class="sxs-lookup"><span data-stu-id="02442-133">displayName</span></span>|<span data-ttu-id="02442-134">String</span><span class="sxs-lookup"><span data-stu-id="02442-134">String</span></span>|<span data-ttu-id="02442-135">O nome de exibição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="02442-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="02442-136">descrição</span><span class="sxs-lookup"><span data-stu-id="02442-136">description</span></span>|<span data-ttu-id="02442-137">String</span><span class="sxs-lookup"><span data-stu-id="02442-137">String</span></span>|<span data-ttu-id="02442-138">A descrição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="02442-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="02442-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="02442-139">onPremisesConnectionId</span></span>|<span data-ttu-id="02442-140">String</span><span class="sxs-lookup"><span data-stu-id="02442-140">String</span></span>|<span data-ttu-id="02442-141">A ID do cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="02442-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="02442-142">Para garantir que os computadores de nuvem tenham conectividade de rede e que eles participem do domínio, escolha uma conexão com uma rede virtual validada pelo serviço de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="02442-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="02442-143">imageId</span><span class="sxs-lookup"><span data-stu-id="02442-143">imageId</span></span>|<span data-ttu-id="02442-144">String</span><span class="sxs-lookup"><span data-stu-id="02442-144">String</span></span>|<span data-ttu-id="02442-145">A ID da imagem do sistema operacional que você deseja provisionar em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="02442-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="02442-146">O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="02442-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="02442-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="02442-147">imageDisplayName</span></span>|<span data-ttu-id="02442-148">String</span><span class="sxs-lookup"><span data-stu-id="02442-148">String</span></span>|<span data-ttu-id="02442-149">O nome de exibição da imagem do sistema operacional que você está provisionando.</span><span class="sxs-lookup"><span data-stu-id="02442-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="02442-150">imageType</span><span class="sxs-lookup"><span data-stu-id="02442-150">imageType</span></span>|<span data-ttu-id="02442-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="02442-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="02442-152">O tipo de imagem do sistema operacional (personalizado ou galeria) que você deseja provisionar em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="02442-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="02442-153">Os valores possíveis são: `gallery` e `custom`.</span><span class="sxs-lookup"><span data-stu-id="02442-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="02442-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="02442-154">Response</span></span>

<span data-ttu-id="02442-155">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02442-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02442-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02442-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02442-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02442-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="02442-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="02442-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="02442-159">C#</span><span class="sxs-lookup"><span data-stu-id="02442-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02442-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02442-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02442-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02442-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02442-162">Java</span><span class="sxs-lookup"><span data-stu-id="02442-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02442-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="02442-163">Response</span></span>

<span data-ttu-id="02442-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02442-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
