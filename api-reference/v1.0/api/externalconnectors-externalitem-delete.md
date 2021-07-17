---
title: Excluir externalItem
description: Exclui um objeto externalItem.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6cf75898963765192ef5f380bddc10794c616a66
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467223"
---
# <a name="delete-externalitem"></a><span data-ttu-id="c3333-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="c3333-103">Delete externalItem</span></span>
<span data-ttu-id="c3333-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="c3333-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="c3333-105">Exclui um [objeto externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="c3333-105">Deletes an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3333-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3333-106">Permissions</span></span>
<span data-ttu-id="c3333-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3333-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3333-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3333-109">Permission type</span></span>|<span data-ttu-id="c3333-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3333-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3333-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3333-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3333-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="c3333-112">Not applicable</span></span>|
|<span data-ttu-id="c3333-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3333-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3333-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="c3333-114">Not applicable</span></span>|
|<span data-ttu-id="c3333-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3333-115">Application</span></span>| <span data-ttu-id="c3333-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3333-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3333-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3333-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionsId}/items/{externalItemId}
```

## <a name="request-headers"></a><span data-ttu-id="c3333-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3333-118">Request headers</span></span>
|<span data-ttu-id="c3333-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c3333-119">Name</span></span>|<span data-ttu-id="c3333-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3333-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3333-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3333-121">Authorization</span></span>|<span data-ttu-id="c3333-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3333-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3333-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3333-124">Request body</span></span>
<span data-ttu-id="c3333-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3333-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3333-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3333-126">Response</span></span>

<span data-ttu-id="c3333-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3333-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c3333-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3333-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3333-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3333-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
```


### <a name="response"></a><span data-ttu-id="c3333-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3333-130">Response</span></span>
<span data-ttu-id="c3333-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3333-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

