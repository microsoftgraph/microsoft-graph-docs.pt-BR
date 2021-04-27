---
title: Criar cloudPcOnPremisesConnection
description: Crie uma conexão local para provisionar PCs de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3f37d57516d78c1f9027346633213b7520d35dd8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053325"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="f67b9-103">Criar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="f67b9-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="f67b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f67b9-105">Crie um novo [objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) para provisionar PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="f67b9-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f67b9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f67b9-106">Permissions</span></span>

<span data-ttu-id="f67b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f67b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f67b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f67b9-109">Permission type</span></span>|<span data-ttu-id="f67b9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f67b9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f67b9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f67b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f67b9-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f67b9-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f67b9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f67b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f67b9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67b9-114">Not supported.</span></span>|
|<span data-ttu-id="f67b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f67b9-115">Application</span></span>|<span data-ttu-id="f67b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f67b9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f67b9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="f67b9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f67b9-118">Request headers</span></span>

| <span data-ttu-id="f67b9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f67b9-119">Name</span></span>          | <span data-ttu-id="f67b9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67b9-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="f67b9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f67b9-121">Authorization</span></span> | <span data-ttu-id="f67b9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f67b9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f67b9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f67b9-124">Content-Type</span></span>  | <span data-ttu-id="f67b9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f67b9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f67b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f67b9-127">Request body</span></span>

<span data-ttu-id="f67b9-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="f67b9-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="f67b9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f67b9-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="f67b9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f67b9-130">Property</span></span>|<span data-ttu-id="f67b9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f67b9-131">Type</span></span>|<span data-ttu-id="f67b9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f67b9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f67b9-133">displayName</span></span>|<span data-ttu-id="f67b9-134">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-134">String</span></span>|<span data-ttu-id="f67b9-135">O nome de exibição da conexão local.</span><span class="sxs-lookup"><span data-stu-id="f67b9-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="f67b9-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="f67b9-136">subscriptionId</span></span>|<span data-ttu-id="f67b9-137">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-137">String</span></span>|<span data-ttu-id="f67b9-138">A ID da assinatura de destino do Azure associada ao seu locatário.</span><span class="sxs-lookup"><span data-stu-id="f67b9-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="f67b9-139">adDomainName</span><span class="sxs-lookup"><span data-stu-id="f67b9-139">adDomainName</span></span>|<span data-ttu-id="f67b9-140">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-140">String</span></span>|<span data-ttu-id="f67b9-141">O FQDN (nome de domínio totalmente qualificado) do domínio do Active Directory que você deseja ingressar.</span><span class="sxs-lookup"><span data-stu-id="f67b9-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="f67b9-142">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="f67b9-142">adDomainUsername</span></span>|<span data-ttu-id="f67b9-143">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-143">String</span></span>|<span data-ttu-id="f67b9-144">O nome de usuário de uma conta do Active Directory (conta de usuário ou serviço) que tem permissões para criar objetos de computador no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f67b9-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="f67b9-145">Formato obrigatório: admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="f67b9-145">Required format: admin@contoso.com.</span></span>|
|<span data-ttu-id="f67b9-146">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="f67b9-146">adDomainPassword</span></span>|<span data-ttu-id="f67b9-147">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-147">String</span></span>|<span data-ttu-id="f67b9-148">A senha associada a adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="f67b9-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="f67b9-149">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="f67b9-149">resourceGroupId</span></span>|<span data-ttu-id="f67b9-150">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-150">String</span></span>|<span data-ttu-id="f67b9-151">A ID do grupo de recursos de destino.</span><span class="sxs-lookup"><span data-stu-id="f67b9-151">The ID of the target resource group.</span></span> <span data-ttu-id="f67b9-152">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="f67b9-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="f67b9-153">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="f67b9-153">virtualNetworkId</span></span>|<span data-ttu-id="f67b9-154">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-154">String</span></span>|<span data-ttu-id="f67b9-155">A ID da rede virtual de destino.</span><span class="sxs-lookup"><span data-stu-id="f67b9-155">The ID of the target virtual network.</span></span> <span data-ttu-id="f67b9-156">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="f67b9-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="f67b9-157">subnetId</span><span class="sxs-lookup"><span data-stu-id="f67b9-157">subnetId</span></span>|<span data-ttu-id="f67b9-158">String</span><span class="sxs-lookup"><span data-stu-id="f67b9-158">String</span></span>|<span data-ttu-id="f67b9-159">A ID da sub-rede de destino.</span><span class="sxs-lookup"><span data-stu-id="f67b9-159">The ID of the target subnet.</span></span> <span data-ttu-id="f67b9-160">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="f67b9-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="f67b9-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67b9-161">Response</span></span>

<span data-ttu-id="f67b9-162">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f67b9-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f67b9-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f67b9-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f67b9-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f67b9-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f67b9-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="f67b9-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpconpremisesconnection_from_cloudpconpremisesconnection"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
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
# <a name="c"></a>[<span data-ttu-id="f67b9-166">C#</span><span class="sxs-lookup"><span data-stu-id="f67b9-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f67b9-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f67b9-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f67b9-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f67b9-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f67b9-169">Java</span><span class="sxs-lookup"><span data-stu-id="f67b9-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f67b9-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67b9-170">Response</span></span>

<span data-ttu-id="f67b9-171">**Observação:** Aqui está um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f67b9-171">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="f67b9-172">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="f67b9-172">The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "ac2ad805-167e-49ee-9bef-196c4ce7ffff",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
  "healthCheckStatus": "pending"
}
```
