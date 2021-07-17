---
title: Criar externalConnection
description: Crie um novo objeto externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d556b4925625ac929c1b13f6559c048de1b55366
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467183"
---
# <a name="create-externalconnection"></a><span data-ttu-id="5c457-103">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="5c457-103">Create externalConnection</span></span>
<span data-ttu-id="5c457-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="5c457-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="5c457-105">Crie um novo objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="5c457-105">Create a new externalConnection object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c457-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c457-106">Permissions</span></span>
<span data-ttu-id="5c457-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c457-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c457-109">Permission type</span></span>|<span data-ttu-id="5c457-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c457-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c457-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c457-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c457-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="5c457-112">Not applicable</span></span>|
|<span data-ttu-id="5c457-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c457-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c457-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="5c457-114">Not applicable</span></span>|
|<span data-ttu-id="5c457-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c457-115">Application</span></span>| <span data-ttu-id="5c457-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="5c457-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c457-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c457-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="5c457-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c457-118">Request headers</span></span>
|<span data-ttu-id="5c457-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c457-119">Name</span></span>|<span data-ttu-id="5c457-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c457-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c457-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c457-121">Authorization</span></span>|<span data-ttu-id="5c457-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c457-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5c457-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c457-124">Content-Type</span></span>|<span data-ttu-id="5c457-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c457-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c457-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c457-127">Request body</span></span>
<span data-ttu-id="5c457-128">No corpo da solicitação, fornece uma representação JSON do [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="5c457-128">In the request body, supply a JSON representation of the [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

<span data-ttu-id="5c457-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="5c457-129">The following table shows the properties that are required when you create the [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

|<span data-ttu-id="5c457-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c457-130">Property</span></span>|<span data-ttu-id="5c457-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c457-131">Type</span></span>|<span data-ttu-id="5c457-132">Obrigatório (Y/N)</span><span class="sxs-lookup"><span data-stu-id="5c457-132">Required (Y/N)</span></span> |<span data-ttu-id="5c457-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c457-133">Description</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="5c457-134">id</span><span class="sxs-lookup"><span data-stu-id="5c457-134">id</span></span>|<span data-ttu-id="5c457-135">String</span><span class="sxs-lookup"><span data-stu-id="5c457-135">String</span></span>|<span data-ttu-id="5c457-136">Y</span><span class="sxs-lookup"><span data-stu-id="5c457-136">Y</span></span>|<span data-ttu-id="5c457-137">A ID da conexão</span><span class="sxs-lookup"><span data-stu-id="5c457-137">The connection ID</span></span>|
|<span data-ttu-id="5c457-138">nome</span><span class="sxs-lookup"><span data-stu-id="5c457-138">name</span></span>|<span data-ttu-id="5c457-139">String</span><span class="sxs-lookup"><span data-stu-id="5c457-139">String</span></span>|<span data-ttu-id="5c457-140">Y</span><span class="sxs-lookup"><span data-stu-id="5c457-140">Y</span></span>|<span data-ttu-id="5c457-141">O nome da conexão</span><span class="sxs-lookup"><span data-stu-id="5c457-141">The connection name</span></span>|
|<span data-ttu-id="5c457-142">description</span><span class="sxs-lookup"><span data-stu-id="5c457-142">description</span></span>|<span data-ttu-id="5c457-143">String</span><span class="sxs-lookup"><span data-stu-id="5c457-143">String</span></span>|<span data-ttu-id="5c457-144">Y</span><span class="sxs-lookup"><span data-stu-id="5c457-144">Y</span></span>|<span data-ttu-id="5c457-145">A descrição da conexão</span><span class="sxs-lookup"><span data-stu-id="5c457-145">The connection description</span></span>|
|<span data-ttu-id="5c457-146">configuração</span><span class="sxs-lookup"><span data-stu-id="5c457-146">configuration</span></span>|[<span data-ttu-id="5c457-147">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="5c457-147">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md)|<span data-ttu-id="5c457-148">N</span><span class="sxs-lookup"><span data-stu-id="5c457-148">N</span></span>|<span data-ttu-id="5c457-149">As configurações de conexão</span><span class="sxs-lookup"><span data-stu-id="5c457-149">The connection configurations</span></span>|



## <a name="response"></a><span data-ttu-id="5c457-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c457-150">Response</span></span>

<span data-ttu-id="5c457-151">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto externalConnection](../resources/externalconnectors-externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c457-151">If successful, this method returns a `201 Created` response code and an [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c457-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c457-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c457-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c457-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/external/connections
Content-Type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```


### <a name="response"></a><span data-ttu-id="5c457-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c457-154">Response</span></span>
<span data-ttu-id="5c457-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c457-155">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 200 Created
Content-Type: application/json

{
  "id": "0a4f4e74-4e74-0a4f-744e-4f0a744e4f0a",
  "name": "String",
  "description": "String",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

