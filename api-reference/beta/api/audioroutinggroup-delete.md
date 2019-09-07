---
title: Excluir grupo de roteamento de áudio
description: Exclua o grupo de roteamento de áudio especificado.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2e1bea10e2aa19f1503ca96fa34ceac6c033d891
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792468"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="b40b3-103">Excluir grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="b40b3-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b40b3-104">Exclua o [audioRoutingGroup](../resources/audioroutinggroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="b40b3-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b40b3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b40b3-105">Permissions</span></span>
<span data-ttu-id="b40b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b40b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b40b3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b40b3-108">Permission type</span></span> | <span data-ttu-id="b40b3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b40b3-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="b40b3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b40b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b40b3-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b40b3-111">Not Supported</span></span>        |
| <span data-ttu-id="b40b3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b40b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b40b3-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b40b3-113">Not Supported</span></span>        |
| <span data-ttu-id="b40b3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b40b3-114">Application</span></span>     | <span data-ttu-id="b40b3-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="b40b3-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b40b3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b40b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b40b3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b40b3-117">Request headers</span></span>
| <span data-ttu-id="b40b3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b40b3-118">Name</span></span>          | <span data-ttu-id="b40b3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b40b3-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b40b3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b40b3-120">Authorization</span></span> | <span data-ttu-id="b40b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b40b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b40b3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b40b3-123">Request body</span></span>
<span data-ttu-id="b40b3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b40b3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b40b3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b40b3-125">Response</span></span>
<span data-ttu-id="b40b3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b40b3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b40b3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b40b3-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b40b3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b40b3-129">Request</span></span>
<span data-ttu-id="b40b3-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b40b3-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b40b3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b40b3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b40b3-132">C#</span><span class="sxs-lookup"><span data-stu-id="b40b3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b40b3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b40b3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b40b3-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b40b3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b40b3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b40b3-135">Response</span></span>

> <span data-ttu-id="b40b3-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b40b3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
