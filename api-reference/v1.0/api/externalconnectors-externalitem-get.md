---
title: Obter externalItem
description: Leia as propriedades e as relações de um objeto externalItem.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6defb4476d5d34b148e8e18c4757333f9bc3ca81
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467221"
---
# <a name="get-externalitem"></a><span data-ttu-id="fc138-103">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="fc138-103">Get externalItem</span></span>
<span data-ttu-id="fc138-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="fc138-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="fc138-105">Leia as propriedades e as relações de um [objeto externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="fc138-105">Read the properties and relationships of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc138-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc138-106">Permissions</span></span>
<span data-ttu-id="fc138-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc138-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc138-109">Permission type</span></span>|<span data-ttu-id="fc138-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc138-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc138-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc138-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc138-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="fc138-112">Not applicable</span></span>|
|<span data-ttu-id="fc138-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc138-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc138-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="fc138-114">Not applicable</span></span>|
|<span data-ttu-id="fc138-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc138-115">Application</span></span>| <span data-ttu-id="fc138-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc138-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc138-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc138-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/items/{externalItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc138-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc138-118">Optional query parameters</span></span>
<span data-ttu-id="fc138-119">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc138-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc138-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc138-120">Request headers</span></span>
|<span data-ttu-id="fc138-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fc138-121">Name</span></span>|<span data-ttu-id="fc138-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc138-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fc138-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc138-123">Authorization</span></span>|<span data-ttu-id="fc138-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc138-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc138-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc138-126">Request body</span></span>
<span data-ttu-id="fc138-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc138-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc138-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc138-128">Response</span></span>

<span data-ttu-id="fc138-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [externalItem](../resources/externalconnectors-externalitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc138-129">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalconnectors-externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc138-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc138-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc138-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc138-131">Request</span></span>
<span data-ttu-id="fc138-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc138-132">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```


### <a name="response"></a><span data-ttu-id="fc138-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc138-133">Response</span></span>
<span data-ttu-id="fc138-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc138-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```

