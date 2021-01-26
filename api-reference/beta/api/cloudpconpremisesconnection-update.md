---
title: Atualizar cloudPcOnPremisesConnection
description: Atualizar as propriedades de um objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9c7f71249f47f9027afc8e7495e8d133a9f74885
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981715"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="ccd3c-103">Atualizar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="ccd3c-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="ccd3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccd3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccd3c-105">Atualizar as propriedades de um [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="ccd3c-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="ccd3c-106">Depois que a conexão local passar na verificação de saúde, indicada pela `healthCheckStatus` propriedade, você não poderá atualizá-la.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ccd3c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccd3c-107">Permissions</span></span>

<span data-ttu-id="ccd3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd3c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccd3c-110">Permission type</span></span>|<span data-ttu-id="ccd3c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccd3c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd3c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccd3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd3c-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd3c-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd3c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccd3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-115">Not supported.</span></span>|
|<span data-ttu-id="ccd3c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccd3c-116">Application</span></span>|<span data-ttu-id="ccd3c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd3c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd3c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ccd3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd3c-119">Request headers</span></span>

| <span data-ttu-id="ccd3c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ccd3c-120">Name</span></span>          | <span data-ttu-id="ccd3c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd3c-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="ccd3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccd3c-122">Authorization</span></span> | <span data-ttu-id="ccd3c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ccd3c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccd3c-125">Content-Type</span></span>  | <span data-ttu-id="ccd3c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd3c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd3c-128">Request body</span></span>

<span data-ttu-id="ccd3c-129">No corpo da solicitação, fornece uma representação JSON do objeto [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="ccd3c-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="ccd3c-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="ccd3c-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="ccd3c-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccd3c-131">Property</span></span>|<span data-ttu-id="ccd3c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccd3c-132">Type</span></span>|<span data-ttu-id="ccd3c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd3c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd3c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ccd3c-134">displayName</span></span>|<span data-ttu-id="ccd3c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-135">String</span></span>|<span data-ttu-id="ccd3c-136">O nome de exibição da conexão local.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="ccd3c-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="ccd3c-137">subscriptionId</span></span>|<span data-ttu-id="ccd3c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-138">String</span></span>|<span data-ttu-id="ccd3c-139">A ID da assinatura do Azure de destino que está associada ao seu locatário.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="ccd3c-140">adDomainName</span><span class="sxs-lookup"><span data-stu-id="ccd3c-140">adDomainName</span></span>|<span data-ttu-id="ccd3c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-141">String</span></span>|<span data-ttu-id="ccd3c-142">O nome de domínio totalmente qualificado (FQDN) do domínio do Active Directory no qual você deseja ingressar.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="ccd3c-143">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="ccd3c-143">adDomainUsername</span></span>|<span data-ttu-id="ccd3c-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-144">String</span></span>|<span data-ttu-id="ccd3c-145">O nome de usuário de uma conta do Active Directory (usuário ou conta de serviço) que tem permissões para criar objetos de computador no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="ccd3c-146">Formato obrigatório: username@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-146">Required format: username@contoso.com.</span></span>|
|<span data-ttu-id="ccd3c-147">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="ccd3c-147">adDomainPassword</span></span>|<span data-ttu-id="ccd3c-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-148">String</span></span>|<span data-ttu-id="ccd3c-149">A senha associada a adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="ccd3c-150">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="ccd3c-150">resourceGroupId</span></span>|<span data-ttu-id="ccd3c-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-151">String</span></span>|<span data-ttu-id="ccd3c-152">A ID do grupo de recursos de destino.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-152">The ID of the target resource group.</span></span> <span data-ttu-id="ccd3c-153">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="ccd3c-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="ccd3c-154">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="ccd3c-154">virtualNetworkId</span></span>|<span data-ttu-id="ccd3c-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-155">String</span></span>|<span data-ttu-id="ccd3c-156">A ID da rede virtual de destino.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-156">The ID of the target virtual network.</span></span> <span data-ttu-id="ccd3c-157">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="ccd3c-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="ccd3c-158">subnetId</span><span class="sxs-lookup"><span data-stu-id="ccd3c-158">subnetId</span></span>|<span data-ttu-id="ccd3c-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccd3c-159">String</span></span>|<span data-ttu-id="ccd3c-160">A ID da sub-rede de destino.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-160">The ID of the target subnet.</span></span> <span data-ttu-id="ccd3c-161">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="ccd3c-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="ccd3c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd3c-162">Response</span></span>

<span data-ttu-id="ccd3c-163">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccd3c-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ccd3c-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccd3c-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd3c-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ccd3c-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd3c-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ccd3c-167">C#</span><span class="sxs-lookup"><span data-stu-id="ccd3c-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccd3c-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccd3c-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccd3c-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccd3c-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccd3c-170">Java</span><span class="sxs-lookup"><span data-stu-id="ccd3c-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ccd3c-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd3c-171">Response</span></span>

<span data-ttu-id="ccd3c-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ccd3c-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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
