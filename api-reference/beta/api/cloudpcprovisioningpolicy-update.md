---
title: Atualizar cloudPcProvisioningPolicy
description: Atualiza as propriedades de um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e96c9a45504f225440d529ae621280a46b09fd02
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378232"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="11137-103">Atualizar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="11137-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="11137-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11137-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11137-105">Atualiza as propriedades de um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11137-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11137-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="11137-106">Permissions</span></span>

<span data-ttu-id="11137-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11137-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11137-109">Permission type</span></span>|<span data-ttu-id="11137-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11137-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11137-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11137-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11137-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11137-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="11137-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11137-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11137-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11137-114">Not supported.</span></span>|
|<span data-ttu-id="11137-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11137-115">Application</span></span>|<span data-ttu-id="11137-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11137-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11137-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11137-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11137-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11137-118">Request headers</span></span>

| <span data-ttu-id="11137-119">Nome</span><span class="sxs-lookup"><span data-stu-id="11137-119">Name</span></span>          | <span data-ttu-id="11137-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11137-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="11137-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11137-121">Authorization</span></span> | <span data-ttu-id="11137-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11137-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="11137-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11137-124">Content-Type</span></span>  | <span data-ttu-id="11137-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11137-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11137-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11137-127">Request body</span></span>

<span data-ttu-id="11137-128">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11137-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="11137-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11137-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="11137-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11137-130">Property</span></span>|<span data-ttu-id="11137-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11137-131">Type</span></span>|<span data-ttu-id="11137-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11137-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11137-133">displayName</span><span class="sxs-lookup"><span data-stu-id="11137-133">displayName</span></span>|<span data-ttu-id="11137-134">String</span><span class="sxs-lookup"><span data-stu-id="11137-134">String</span></span>|<span data-ttu-id="11137-135">O nome de exibição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="11137-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="11137-136">description</span><span class="sxs-lookup"><span data-stu-id="11137-136">description</span></span>|<span data-ttu-id="11137-137">String</span><span class="sxs-lookup"><span data-stu-id="11137-137">String</span></span>|<span data-ttu-id="11137-138">A descrição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="11137-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="11137-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="11137-139">onPremisesConnectionId</span></span>|<span data-ttu-id="11137-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="11137-140">String</span></span>|<span data-ttu-id="11137-141">A ID do cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="11137-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="11137-142">Para garantir que os computadores em nuvem tenham conectividade de rede e que eles ingressem no domínio, escolha uma conexão com uma rede virtual validada pelo serviço de Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="11137-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="11137-143">imageid</span><span class="sxs-lookup"><span data-stu-id="11137-143">imageId</span></span>|<span data-ttu-id="11137-144">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="11137-144">String</span></span>|<span data-ttu-id="11137-145">A ID da imagem do sistema operacional que você deseja provisionar em PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="11137-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="11137-146">O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="11137-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="11137-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="11137-147">imageDisplayName</span></span>|<span data-ttu-id="11137-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="11137-148">String</span></span>|<span data-ttu-id="11137-149">O nome de exibição para a imagem do sistema operacional que você está Provisionando.</span><span class="sxs-lookup"><span data-stu-id="11137-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="11137-150">ImageType</span><span class="sxs-lookup"><span data-stu-id="11137-150">imageType</span></span>|<span data-ttu-id="11137-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="11137-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="11137-152">O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="11137-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="11137-153">Os valores possíveis são: `gallery` e `custom`.</span><span class="sxs-lookup"><span data-stu-id="11137-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="11137-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="11137-154">Response</span></span>

<span data-ttu-id="11137-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11137-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11137-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11137-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11137-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11137-157">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="11137-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="11137-158">Response</span></span>

<span data-ttu-id="11137-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11137-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
