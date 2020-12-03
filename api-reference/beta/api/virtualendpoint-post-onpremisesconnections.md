---
title: Criar cloudPcOnPremisesConnection
description: Crie uma conexão local para o provisionamento de PCs em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 0cbdbd6cb135e6adecf110ed6d18d03f9dfa5dd9
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563462"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="c8050-103">Criar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c8050-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="c8050-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8050-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8050-105">Criar um novo objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) para provisionar PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="c8050-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="c8050-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8050-106">Permissions</span></span>

<span data-ttu-id="c8050-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8050-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8050-109">Permission type</span></span>|<span data-ttu-id="c8050-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8050-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8050-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8050-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8050-112">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c8050-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c8050-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8050-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8050-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8050-114">Not supported.</span></span>|
|<span data-ttu-id="c8050-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8050-115">Application</span></span>|<span data-ttu-id="c8050-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8050-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8050-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8050-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="c8050-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8050-118">Request headers</span></span>

| <span data-ttu-id="c8050-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c8050-119">Name</span></span>          | <span data-ttu-id="c8050-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8050-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="c8050-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8050-121">Authorization</span></span> | <span data-ttu-id="c8050-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8050-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c8050-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8050-124">Content-Type</span></span>  | <span data-ttu-id="c8050-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8050-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8050-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8050-127">Request body</span></span>

<span data-ttu-id="c8050-128">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="c8050-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="c8050-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="c8050-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="c8050-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8050-130">Property</span></span>|<span data-ttu-id="c8050-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8050-131">Type</span></span>|<span data-ttu-id="c8050-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8050-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8050-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c8050-133">displayName</span></span>|<span data-ttu-id="c8050-134">String</span><span class="sxs-lookup"><span data-stu-id="c8050-134">String</span></span>|<span data-ttu-id="c8050-135">O nome de exibição para a conexão local.</span><span class="sxs-lookup"><span data-stu-id="c8050-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="c8050-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="c8050-136">subscriptionId</span></span>|<span data-ttu-id="c8050-137">String</span><span class="sxs-lookup"><span data-stu-id="c8050-137">String</span></span>|<span data-ttu-id="c8050-138">A ID da assinatura de destino do Azure que está associada ao seu locatário.</span><span class="sxs-lookup"><span data-stu-id="c8050-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="c8050-139">adDomainName</span><span class="sxs-lookup"><span data-stu-id="c8050-139">adDomainName</span></span>|<span data-ttu-id="c8050-140">String</span><span class="sxs-lookup"><span data-stu-id="c8050-140">String</span></span>|<span data-ttu-id="c8050-141">O FQDN (nome de domínio totalmente qualificado) do domínio do Active Directory que você deseja ingressar.</span><span class="sxs-lookup"><span data-stu-id="c8050-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="c8050-142">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="c8050-142">adDomainUsername</span></span>|<span data-ttu-id="c8050-143">String</span><span class="sxs-lookup"><span data-stu-id="c8050-143">String</span></span>|<span data-ttu-id="c8050-144">O nome de usuário de uma conta do Active Directory (usuário ou conta de serviço) que tem permissões para criar objetos de computador no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8050-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="c8050-145">Formato obrigatório: contoso@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="c8050-145">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="c8050-146">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="c8050-146">adDomainPassword</span></span>|<span data-ttu-id="c8050-147">String</span><span class="sxs-lookup"><span data-stu-id="c8050-147">String</span></span>|<span data-ttu-id="c8050-148">A senha associada ao adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="c8050-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="c8050-149">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="c8050-149">resourceGroupId</span></span>|<span data-ttu-id="c8050-150">String</span><span class="sxs-lookup"><span data-stu-id="c8050-150">String</span></span>|<span data-ttu-id="c8050-151">A ID do grupo de recursos de destino.</span><span class="sxs-lookup"><span data-stu-id="c8050-151">The ID of the target resource group.</span></span> <span data-ttu-id="c8050-152">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="c8050-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="c8050-153">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="c8050-153">virtualNetworkId</span></span>|<span data-ttu-id="c8050-154">String</span><span class="sxs-lookup"><span data-stu-id="c8050-154">String</span></span>|<span data-ttu-id="c8050-155">A ID da rede virtual de destino.</span><span class="sxs-lookup"><span data-stu-id="c8050-155">The ID of the target virtual network.</span></span> <span data-ttu-id="c8050-156">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="c8050-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="c8050-157">subnetid</span><span class="sxs-lookup"><span data-stu-id="c8050-157">subnetId</span></span>|<span data-ttu-id="c8050-158">String</span><span class="sxs-lookup"><span data-stu-id="c8050-158">String</span></span>|<span data-ttu-id="c8050-159">A ID da sub-rede de destino.</span><span class="sxs-lookup"><span data-stu-id="c8050-159">The ID of the target subnet.</span></span> <span data-ttu-id="c8050-160">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="c8050-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="c8050-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8050-161">Response</span></span>

<span data-ttu-id="c8050-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8050-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8050-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c8050-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8050-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8050-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c8050-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8050-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c8050-166">C#</span><span class="sxs-lookup"><span data-stu-id="c8050-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8050-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8050-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8050-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8050-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8050-169">Java</span><span class="sxs-lookup"><span data-stu-id="c8050-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8050-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8050-170">Response</span></span>

<span data-ttu-id="c8050-171">**Observação:** Veja um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8050-171">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="c8050-172">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="c8050-172">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c8050-173">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8050-173">All of the properties will be returned from an actual call.</span></span>
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
  "healthCheckStatus": "pending",
  "inUse": false
}
```
