---
title: Criar cloudPcProvisioningPolicy
description: Crie uma nova política de provisionamento de computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6c28d27cced97d2e1ab927de14d888ae15d8e902
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547608"
---
# <a name="create-cloudpcprovisioningpolicy"></a><span data-ttu-id="edbab-103">Criar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="edbab-103">Create cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="edbab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edbab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edbab-105">Crie um novo [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="edbab-105">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="edbab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="edbab-106">Permissions</span></span>

<span data-ttu-id="edbab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edbab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edbab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edbab-109">Permission type</span></span>|<span data-ttu-id="edbab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="edbab-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edbab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edbab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="edbab-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbab-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="edbab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edbab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edbab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edbab-114">Not supported.</span></span>|
|<span data-ttu-id="edbab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edbab-115">Application</span></span>|<span data-ttu-id="edbab-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbab-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edbab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edbab-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a><span data-ttu-id="edbab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edbab-118">Request headers</span></span>

| <span data-ttu-id="edbab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="edbab-119">Name</span></span>          | <span data-ttu-id="edbab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="edbab-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="edbab-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="edbab-121">Authorization</span></span> | <span data-ttu-id="edbab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edbab-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="edbab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edbab-124">Content-Type</span></span>  | <span data-ttu-id="edbab-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edbab-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="edbab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edbab-127">Request body</span></span>

<span data-ttu-id="edbab-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="edbab-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="edbab-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="edbab-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="edbab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edbab-130">Property</span></span>|<span data-ttu-id="edbab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="edbab-131">Type</span></span>|<span data-ttu-id="edbab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="edbab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edbab-133">displayName</span><span class="sxs-lookup"><span data-stu-id="edbab-133">displayName</span></span>|<span data-ttu-id="edbab-134">String</span><span class="sxs-lookup"><span data-stu-id="edbab-134">String</span></span>|<span data-ttu-id="edbab-135">O nome de exibição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="edbab-135">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="edbab-136">descrição</span><span class="sxs-lookup"><span data-stu-id="edbab-136">description</span></span>|<span data-ttu-id="edbab-137">String</span><span class="sxs-lookup"><span data-stu-id="edbab-137">String</span></span>|<span data-ttu-id="edbab-138">A descrição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="edbab-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="edbab-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="edbab-139">onPremisesConnectionId</span></span>|<span data-ttu-id="edbab-140">String</span><span class="sxs-lookup"><span data-stu-id="edbab-140">String</span></span>|<span data-ttu-id="edbab-141">A ID do cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="edbab-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="edbab-142">Para garantir que os computadores de nuvem tenham conectividade de rede e que eles participem do domínio, escolha uma conexão com uma rede virtual validada pelo serviço de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="edbab-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="edbab-143">imageId</span><span class="sxs-lookup"><span data-stu-id="edbab-143">imageId</span></span>|<span data-ttu-id="edbab-144">String</span><span class="sxs-lookup"><span data-stu-id="edbab-144">String</span></span>|<span data-ttu-id="edbab-145">A ID da imagem do sistema operacional que você deseja provisionar em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="edbab-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="edbab-146">O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="edbab-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="edbab-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="edbab-147">imageDisplayName</span></span>|<span data-ttu-id="edbab-148">String</span><span class="sxs-lookup"><span data-stu-id="edbab-148">String</span></span>|<span data-ttu-id="edbab-149">O nome de exibição da imagem do sistema operacional que você está provisionando.</span><span class="sxs-lookup"><span data-stu-id="edbab-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="edbab-150">imageType</span><span class="sxs-lookup"><span data-stu-id="edbab-150">imageType</span></span>|<span data-ttu-id="edbab-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="edbab-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="edbab-152">O tipo de imagem do sistema operacional (personalizado ou galeria) que você deseja provisionar em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="edbab-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="edbab-153">Os valores possíveis são: `gallery` e `custom`.</span><span class="sxs-lookup"><span data-stu-id="edbab-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="edbab-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="edbab-154">Response</span></span>

<span data-ttu-id="edbab-155">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edbab-155">If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="edbab-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="edbab-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="edbab-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edbab-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="edbab-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="edbab-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "gallery"
}
```
# <a name="c"></a>[<span data-ttu-id="edbab-159">C#</span><span class="sxs-lookup"><span data-stu-id="edbab-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edbab-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edbab-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edbab-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edbab-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edbab-162">Java</span><span class="sxs-lookup"><span data-stu-id="edbab-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="edbab-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="edbab-163">Response</span></span>

<span data-ttu-id="edbab-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="edbab-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
  }
```
