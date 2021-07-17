---
title: Obter externalConnection
description: Leia as propriedades e as relações de um objeto externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ca5dc2d998cfa327f3c263222583de0c42aaaab4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467181"
---
# <a name="get-externalconnection"></a><span data-ttu-id="f369c-103">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="f369c-103">Get externalConnection</span></span>
<span data-ttu-id="f369c-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="f369c-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="f369c-105">Leia as propriedades e as relações de um [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="f369c-105">Read the properties and relationships of an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f369c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f369c-106">Permissions</span></span>
<span data-ttu-id="f369c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f369c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f369c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f369c-109">Permission type</span></span>|<span data-ttu-id="f369c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f369c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f369c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f369c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f369c-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="f369c-112">Not applicable</span></span>|
|<span data-ttu-id="f369c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f369c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f369c-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="f369c-114">Not applicable</span></span>|
|<span data-ttu-id="f369c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f369c-115">Application</span></span>| <span data-ttu-id="f369c-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f369c-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="f369c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f369c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f369c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f369c-118">Optional query parameters</span></span>
<span data-ttu-id="f369c-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f369c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f369c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f369c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f369c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f369c-121">Request headers</span></span>
|<span data-ttu-id="f369c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f369c-122">Name</span></span>|<span data-ttu-id="f369c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f369c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f369c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f369c-124">Authorization</span></span>|<span data-ttu-id="f369c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f369c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f369c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f369c-127">Request body</span></span>
<span data-ttu-id="f369c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f369c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f369c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f369c-129">Response</span></span>

<span data-ttu-id="f369c-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto externalConnection](../resources/externalconnectors-externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f369c-130">If successful, this method returns a `200 OK` response code and an [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f369c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f369c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f369c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f369c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr
```


### <a name="response"></a><span data-ttu-id="f369c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f369c-133">Response</span></span>
<span data-ttu-id="f369c-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f369c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```

