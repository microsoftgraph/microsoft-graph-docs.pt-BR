---
title: Excluir grupo de roteamento de áudio
description: Exclua o grupo de roteamento de áudio especificado.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: de1ac6aa2a296cf95fddb33c075f52ce57da0d81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048019"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="bfbf1-103">Excluir grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="bfbf1-103">Delete audio routing group</span></span>

<span data-ttu-id="bfbf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfbf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfbf1-105">Exclua [o audioRoutingGroup especificado.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="bfbf1-105">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bfbf1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfbf1-106">Permissions</span></span>
<span data-ttu-id="bfbf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfbf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bfbf1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfbf1-109">Permission type</span></span> | <span data-ttu-id="bfbf1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfbf1-110">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="bfbf1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfbf1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfbf1-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bfbf1-112">Not Supported</span></span>        |
| <span data-ttu-id="bfbf1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfbf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfbf1-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bfbf1-114">Not Supported</span></span>        |
| <span data-ttu-id="bfbf1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfbf1-115">Application</span></span>     | <span data-ttu-id="bfbf1-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="bfbf1-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfbf1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfbf1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="bfbf1-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="bfbf1-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfbf1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbf1-120">Request headers</span></span>
| <span data-ttu-id="bfbf1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bfbf1-121">Name</span></span>          | <span data-ttu-id="bfbf1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfbf1-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bfbf1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfbf1-123">Authorization</span></span> | <span data-ttu-id="bfbf1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfbf1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbf1-126">Request body</span></span>
<span data-ttu-id="bfbf1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfbf1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfbf1-128">Response</span></span>
<span data-ttu-id="bfbf1-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfbf1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfbf1-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bfbf1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbf1-132">Request</span></span>
<span data-ttu-id="bfbf1-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bfbf1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfbf1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="bfbf1-135">C#</span><span class="sxs-lookup"><span data-stu-id="bfbf1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfbf1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfbf1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfbf1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfbf1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfbf1-138">Java</span><span class="sxs-lookup"><span data-stu-id="bfbf1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bfbf1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfbf1-139">Response</span></span>

> <span data-ttu-id="bfbf1-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bfbf1-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


