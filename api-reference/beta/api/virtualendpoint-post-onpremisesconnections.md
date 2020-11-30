---
title: Criar cloudPcOnPremisesConnection
description: Crie uma conexão local para o provisionamento de PCs em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 41cb092a18f56d28120ecf953a1700cdd35dfd51
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378247"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="d014e-103">Criar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="d014e-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="d014e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d014e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d014e-105">Criar um novo objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) para provisionar PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="d014e-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

## <a name="permissions"></a><span data-ttu-id="d014e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d014e-106">Permissions</span></span>

<span data-ttu-id="d014e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d014e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d014e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d014e-109">Permission type</span></span>|<span data-ttu-id="d014e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d014e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d014e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d014e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d014e-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d014e-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d014e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d014e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d014e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d014e-114">Not supported.</span></span>|
|<span data-ttu-id="d014e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d014e-115">Application</span></span>|<span data-ttu-id="d014e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d014e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d014e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d014e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="d014e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d014e-118">Request headers</span></span>

| <span data-ttu-id="d014e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d014e-119">Name</span></span>          | <span data-ttu-id="d014e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d014e-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="d014e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d014e-121">Authorization</span></span> | <span data-ttu-id="d014e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d014e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d014e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d014e-124">Content-Type</span></span>  | <span data-ttu-id="d014e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d014e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d014e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d014e-127">Request body</span></span>

<span data-ttu-id="d014e-128">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="d014e-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="d014e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d014e-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="d014e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d014e-130">Property</span></span>|<span data-ttu-id="d014e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d014e-131">Type</span></span>|<span data-ttu-id="d014e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d014e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d014e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d014e-133">displayName</span></span>|<span data-ttu-id="d014e-134">String</span><span class="sxs-lookup"><span data-stu-id="d014e-134">String</span></span>|<span data-ttu-id="d014e-135">O nome de exibição para a conexão local.</span><span class="sxs-lookup"><span data-stu-id="d014e-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="d014e-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="d014e-136">subscriptionId</span></span>|<span data-ttu-id="d014e-137">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-137">String</span></span>|<span data-ttu-id="d014e-138">A ID da assinatura de destino do Azure que está associada ao seu locatário.</span><span class="sxs-lookup"><span data-stu-id="d014e-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="d014e-139">adDomainName</span><span class="sxs-lookup"><span data-stu-id="d014e-139">adDomainName</span></span>|<span data-ttu-id="d014e-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-140">String</span></span>|<span data-ttu-id="d014e-141">O FQDN (nome de domínio totalmente qualificado) do domínio do Active Directory que você deseja ingressar.</span><span class="sxs-lookup"><span data-stu-id="d014e-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="d014e-142">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="d014e-142">adDomainUsername</span></span>|<span data-ttu-id="d014e-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-143">String</span></span>|<span data-ttu-id="d014e-144">O nome de usuário de uma conta do Active Directory (usuário ou conta de serviço) que tem permissões para criar objetos de computador no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d014e-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="d014e-145">Formato obrigatório: contoso@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="d014e-145">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="d014e-146">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="d014e-146">adDomainPassword</span></span>|<span data-ttu-id="d014e-147">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-147">String</span></span>|<span data-ttu-id="d014e-148">A senha associada ao adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="d014e-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="d014e-149">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="d014e-149">resourceGroupId</span></span>|<span data-ttu-id="d014e-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-150">String</span></span>|<span data-ttu-id="d014e-151">A ID do grupo de recursos de destino.</span><span class="sxs-lookup"><span data-stu-id="d014e-151">The ID of the target resource group.</span></span> <span data-ttu-id="d014e-152">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="d014e-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="d014e-153">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="d014e-153">virtualNetworkId</span></span>|<span data-ttu-id="d014e-154">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-154">String</span></span>|<span data-ttu-id="d014e-155">A ID da rede virtual de destino.</span><span class="sxs-lookup"><span data-stu-id="d014e-155">The ID of the target virtual network.</span></span> <span data-ttu-id="d014e-156">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="d014e-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="d014e-157">subnetid</span><span class="sxs-lookup"><span data-stu-id="d014e-157">subnetId</span></span>|<span data-ttu-id="d014e-158">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d014e-158">String</span></span>|<span data-ttu-id="d014e-159">A ID da sub-rede de destino.</span><span class="sxs-lookup"><span data-stu-id="d014e-159">The ID of the target subnet.</span></span> <span data-ttu-id="d014e-160">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="d014e-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="d014e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d014e-161">Response</span></span>

<span data-ttu-id="d014e-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d014e-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d014e-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d014e-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d014e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d014e-164">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="d014e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d014e-165">Response</span></span>

<span data-ttu-id="d014e-166">**Observação:** Veja um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d014e-166">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="d014e-167">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="d014e-167">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d014e-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d014e-168">All of the properties will be returned from an actual call.</span></span>
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
