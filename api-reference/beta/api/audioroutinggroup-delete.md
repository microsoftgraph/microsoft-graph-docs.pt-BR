---
title: Excluir grupo de roteamento de áudio
description: Exclua o grupo de roteamento de áudio especificado.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 87cada1f74e36398fef2f1eda82d622540c7ac47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991709"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="aac13-103">Excluir grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="aac13-103">Delete audio routing group</span></span>

<span data-ttu-id="aac13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aac13-105">Exclua o [audioRoutingGroup](../resources/audioroutinggroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="aac13-105">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aac13-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aac13-106">Permissions</span></span>
<span data-ttu-id="aac13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aac13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aac13-109">Permission type</span></span> | <span data-ttu-id="aac13-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aac13-110">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="aac13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aac13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aac13-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="aac13-112">Not Supported</span></span>        |
| <span data-ttu-id="aac13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aac13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac13-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="aac13-114">Not Supported</span></span>        |
| <span data-ttu-id="aac13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aac13-115">Application</span></span>     | <span data-ttu-id="aac13-116">Calls. JoinGroupCalls. All, Calls.InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="aac13-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aac13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aac13-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="aac13-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="aac13-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="aac13-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="aac13-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aac13-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aac13-120">Request headers</span></span>
| <span data-ttu-id="aac13-121">Nome</span><span class="sxs-lookup"><span data-stu-id="aac13-121">Name</span></span>          | <span data-ttu-id="aac13-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac13-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="aac13-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aac13-123">Authorization</span></span> | <span data-ttu-id="aac13-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aac13-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aac13-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aac13-126">Request body</span></span>
<span data-ttu-id="aac13-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aac13-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac13-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac13-128">Response</span></span>
<span data-ttu-id="aac13-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aac13-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac13-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aac13-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aac13-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aac13-132">Request</span></span>
<span data-ttu-id="aac13-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="aac13-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aac13-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="aac13-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="aac13-135">C#</span><span class="sxs-lookup"><span data-stu-id="aac13-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aac13-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aac13-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aac13-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aac13-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aac13-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac13-138">Response</span></span>

> <span data-ttu-id="aac13-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aac13-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


