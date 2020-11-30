---
title: Atualizar cloudPcOnPremisesConnection
description: Atualiza as propriedades de um objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b4f50441c46cc74dad5da08a3836aa471c158ad7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378211"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="a5c91-103">Atualizar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="a5c91-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="a5c91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5c91-105">Atualiza as propriedades de um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="a5c91-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="a5c91-106">Quando a conexão local passar na verificação de integridade, que é indicada pela `healthCheckStatus` propriedade, não será possível atualizá-la.</span><span class="sxs-lookup"><span data-stu-id="a5c91-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5c91-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a5c91-107">Permissions</span></span>

<span data-ttu-id="a5c91-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c91-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5c91-110">Permission type</span></span>|<span data-ttu-id="a5c91-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5c91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5c91-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5c91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5c91-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5c91-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a5c91-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5c91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5c91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5c91-115">Not supported.</span></span>|
|<span data-ttu-id="a5c91-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5c91-116">Application</span></span>|<span data-ttu-id="a5c91-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5c91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5c91-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c91-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5c91-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5c91-119">Request headers</span></span>

| <span data-ttu-id="a5c91-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5c91-120">Name</span></span>          | <span data-ttu-id="a5c91-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5c91-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="a5c91-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5c91-122">Authorization</span></span> | <span data-ttu-id="a5c91-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5c91-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5c91-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5c91-125">Content-Type</span></span>  | <span data-ttu-id="a5c91-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5c91-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5c91-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5c91-128">Request body</span></span>

<span data-ttu-id="a5c91-129">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="a5c91-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="a5c91-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="a5c91-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="a5c91-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5c91-131">Property</span></span>|<span data-ttu-id="a5c91-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5c91-132">Type</span></span>|<span data-ttu-id="a5c91-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5c91-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c91-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a5c91-134">displayName</span></span>|<span data-ttu-id="a5c91-135">String</span><span class="sxs-lookup"><span data-stu-id="a5c91-135">String</span></span>|<span data-ttu-id="a5c91-136">O nome de exibição para a conexão local.</span><span class="sxs-lookup"><span data-stu-id="a5c91-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="a5c91-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="a5c91-137">subscriptionId</span></span>|<span data-ttu-id="a5c91-138">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-138">String</span></span>|<span data-ttu-id="a5c91-139">A ID da assinatura de destino do Azure que está associada ao seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a5c91-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="a5c91-140">adDomainName</span><span class="sxs-lookup"><span data-stu-id="a5c91-140">adDomainName</span></span>|<span data-ttu-id="a5c91-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-141">String</span></span>|<span data-ttu-id="a5c91-142">O FQDN (nome de domínio totalmente qualificado) do domínio do Active Directory que você deseja ingressar.</span><span class="sxs-lookup"><span data-stu-id="a5c91-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="a5c91-143">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="a5c91-143">adDomainUsername</span></span>|<span data-ttu-id="a5c91-144">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-144">String</span></span>|<span data-ttu-id="a5c91-145">O nome de usuário de uma conta do Active Directory (usuário ou conta de serviço) que tem permissões para criar objetos de computador no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a5c91-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="a5c91-146">Formato obrigatório: contoso@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="a5c91-146">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="a5c91-147">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="a5c91-147">adDomainPassword</span></span>|<span data-ttu-id="a5c91-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-148">String</span></span>|<span data-ttu-id="a5c91-149">A senha associada ao adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="a5c91-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="a5c91-150">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="a5c91-150">resourceGroupId</span></span>|<span data-ttu-id="a5c91-151">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-151">String</span></span>|<span data-ttu-id="a5c91-152">A ID do grupo de recursos de destino.</span><span class="sxs-lookup"><span data-stu-id="a5c91-152">The ID of the target resource group.</span></span> <span data-ttu-id="a5c91-153">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="a5c91-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="a5c91-154">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="a5c91-154">virtualNetworkId</span></span>|<span data-ttu-id="a5c91-155">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-155">String</span></span>|<span data-ttu-id="a5c91-156">A ID da rede virtual de destino.</span><span class="sxs-lookup"><span data-stu-id="a5c91-156">The ID of the target virtual network.</span></span> <span data-ttu-id="a5c91-157">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="a5c91-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="a5c91-158">subnetid</span><span class="sxs-lookup"><span data-stu-id="a5c91-158">subnetId</span></span>|<span data-ttu-id="a5c91-159">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a5c91-159">String</span></span>|<span data-ttu-id="a5c91-160">A ID da sub-rede de destino.</span><span class="sxs-lookup"><span data-stu-id="a5c91-160">The ID of the target subnet.</span></span> <span data-ttu-id="a5c91-161">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="a5c91-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="a5c91-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5c91-162">Response</span></span>

<span data-ttu-id="a5c91-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5c91-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5c91-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5c91-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5c91-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5c91-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_onpremisesconnections"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
Content-Type: application/json
Content-length: 800

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
}
```

### <a name="response"></a><span data-ttu-id="a5c91-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5c91-166">Response</span></span>

<span data-ttu-id="a5c91-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5c91-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdcc4ffff",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
  "healthCheckStatus": "running",
  "inUse": false
}
```
