---
title: Listar externalConnections
description: Obter uma lista dos objetos externalConnection e suas propriedades.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 07b0db1eb735999263bc5d2855e7c263351f02e0
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467222"
---
# <a name="list-externalconnections"></a><span data-ttu-id="24839-103">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="24839-103">List externalConnections</span></span>
<span data-ttu-id="24839-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="24839-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="24839-105">Obter uma lista dos [objetos externalConnection](../resources/externalconnectors-externalconnection.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="24839-105">Get a list of the [externalConnection](../resources/externalconnectors-externalconnection.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="24839-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24839-106">Permissions</span></span>
<span data-ttu-id="24839-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24839-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24839-109">Permission type</span></span>|<span data-ttu-id="24839-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24839-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24839-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24839-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24839-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="24839-112">Not applicable</span></span>|
|<span data-ttu-id="24839-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24839-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24839-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="24839-114">Not applicable</span></span>|
|<span data-ttu-id="24839-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24839-115">Application</span></span>| <span data-ttu-id="24839-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="24839-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="24839-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24839-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24839-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24839-118">Optional query parameters</span></span>
<span data-ttu-id="24839-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24839-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="24839-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="24839-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="24839-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24839-121">Request headers</span></span>
|<span data-ttu-id="24839-122">Nome</span><span class="sxs-lookup"><span data-stu-id="24839-122">Name</span></span>|<span data-ttu-id="24839-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="24839-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24839-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="24839-124">Authorization</span></span>|<span data-ttu-id="24839-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24839-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24839-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24839-127">Request body</span></span>
<span data-ttu-id="24839-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24839-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24839-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="24839-129">Response</span></span>

<span data-ttu-id="24839-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos externalConnection](../resources/externalconnectors-externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24839-130">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnectors-externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24839-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24839-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24839-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24839-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections
```


### <a name="response"></a><span data-ttu-id="24839-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="24839-133">Response</span></span>
<span data-ttu-id="24839-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24839-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.externalConnectors.externalConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    }
  ]
}
```

