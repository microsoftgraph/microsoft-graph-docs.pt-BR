---
title: Excluir conector
description: Excluir (cancelar o registro) de um conector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1404bbf5851770eec12c3234ac80e84461ffb029
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895583"
---
# <a name="delete-connector"></a><span data-ttu-id="5c1bf-103">Excluir conector</span><span class="sxs-lookup"><span data-stu-id="5c1bf-103">Delete connector</span></span>

<span data-ttu-id="5c1bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c1bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c1bf-105">Excluir (cancelar o registro) de um **Reconectador**.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c1bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c1bf-106">Permissions</span></span>
<span data-ttu-id="5c1bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c1bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5c1bf-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5c1bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c1bf-110">Permission type</span></span> | <span data-ttu-id="5c1bf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c1bf-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5c1bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c1bf-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5c1bf-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="5c1bf-113">Users.Read.All</span></span> |
|<span data-ttu-id="5c1bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c1bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c1bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-115">Not Supported.</span></span>|
|<span data-ttu-id="5c1bf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c1bf-116">Application</span></span>|<span data-ttu-id="5c1bf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c1bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c1bf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5c1bf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1bf-119">Request headers</span></span>
| <span data-ttu-id="5c1bf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5c1bf-120">Name</span></span>          | <span data-ttu-id="5c1bf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c1bf-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5c1bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c1bf-122">Authorization</span></span> | <span data-ttu-id="5c1bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c1bf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1bf-125">Request body</span></span>
<span data-ttu-id="5c1bf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c1bf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1bf-127">Response</span></span>
<span data-ttu-id="5c1bf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="5c1bf-130">Condições e mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="5c1bf-130">Error conditions and messages</span></span>

|<span data-ttu-id="5c1bf-131">Cenário</span><span class="sxs-lookup"><span data-stu-id="5c1bf-131">Scenario</span></span>|<span data-ttu-id="5c1bf-132">Método</span><span class="sxs-lookup"><span data-stu-id="5c1bf-132">Method</span></span>|<span data-ttu-id="5c1bf-133">Código</span><span class="sxs-lookup"><span data-stu-id="5c1bf-133">Code</span></span>|<span data-ttu-id="5c1bf-134">Mensagem</span><span class="sxs-lookup"><span data-stu-id="5c1bf-134">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="5c1bf-135">O usuário tenta excluir um conector que tem uma ou mais impressoras registradas</span><span class="sxs-lookup"><span data-stu-id="5c1bf-135">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="5c1bf-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="5c1bf-136">DELETE</span></span>|<span data-ttu-id="5c1bf-137">409</span><span class="sxs-lookup"><span data-stu-id="5c1bf-137">409</span></span>|<span data-ttu-id="5c1bf-138">Antes de excluir o conector, cancele o registro das impressoras associadas.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-138">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="5c1bf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c1bf-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c1bf-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1bf-140">Request</span></span>
<span data-ttu-id="5c1bf-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="5c1bf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1bf-142">Response</span></span>
<span data-ttu-id="5c1bf-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-143">The following is an example of the response.</span></span>
><span data-ttu-id="5c1bf-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c1bf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->