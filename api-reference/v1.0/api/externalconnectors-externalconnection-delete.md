---
title: Excluir externalConnection
description: Exclui um objeto externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e365c09fca03a97894a53b23eef2d500527a774f
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467180"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="a7eb3-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="a7eb3-103">Delete externalConnection</span></span>
<span data-ttu-id="a7eb3-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="a7eb3-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="a7eb3-105">Exclui um [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="a7eb3-105">Deletes an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7eb3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7eb3-106">Permissions</span></span>
<span data-ttu-id="a7eb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7eb3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7eb3-109">Permission type</span></span>|<span data-ttu-id="a7eb3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7eb3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7eb3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7eb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7eb3-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="a7eb3-112">Not applicable</span></span>|
|<span data-ttu-id="a7eb3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7eb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7eb3-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="a7eb3-114">Not applicable</span></span>|
|<span data-ttu-id="a7eb3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7eb3-115">Application</span></span>| <span data-ttu-id="a7eb3-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a7eb3-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7eb3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7eb3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionsId}
```

## <a name="request-headers"></a><span data-ttu-id="a7eb3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7eb3-118">Request headers</span></span>
|<span data-ttu-id="a7eb3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a7eb3-119">Name</span></span>|<span data-ttu-id="a7eb3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7eb3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a7eb3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7eb3-121">Authorization</span></span>|<span data-ttu-id="a7eb3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7eb3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7eb3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7eb3-124">Request body</span></span>
<span data-ttu-id="a7eb3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7eb3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7eb3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7eb3-126">Response</span></span>

<span data-ttu-id="a7eb3-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7eb3-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7eb3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7eb3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7eb3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7eb3-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalconnection"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/connections/contosohr
```


### <a name="response"></a><span data-ttu-id="a7eb3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7eb3-131">Response</span></span>
<span data-ttu-id="a7eb3-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7eb3-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

