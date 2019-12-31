---
title: Excluir grupo de roteamento de áudio
description: Exclua o grupo de roteamento de áudio especificado.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7f89c223c7e45ccaa5a25fe7bbdd7a53f529880f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911809"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="a8299-103">Excluir grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="a8299-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8299-104">Exclua o [audioRoutingGroup](../resources/audioroutinggroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="a8299-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8299-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8299-105">Permissions</span></span>
<span data-ttu-id="a8299-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8299-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8299-108">Permission type</span></span> | <span data-ttu-id="a8299-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8299-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="a8299-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8299-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8299-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="a8299-111">Not Supported</span></span>        |
| <span data-ttu-id="a8299-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8299-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8299-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="a8299-113">Not Supported</span></span>        |
| <span data-ttu-id="a8299-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8299-114">Application</span></span>     | <span data-ttu-id="a8299-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="a8299-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8299-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8299-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="a8299-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="a8299-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="a8299-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="a8299-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8299-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8299-119">Request headers</span></span>
| <span data-ttu-id="a8299-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a8299-120">Name</span></span>          | <span data-ttu-id="a8299-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8299-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a8299-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8299-122">Authorization</span></span> | <span data-ttu-id="a8299-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8299-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8299-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8299-125">Request body</span></span>
<span data-ttu-id="a8299-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8299-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8299-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8299-127">Response</span></span>
<span data-ttu-id="a8299-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8299-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8299-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8299-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a8299-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8299-131">Request</span></span>
<span data-ttu-id="a8299-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8299-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8299-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8299-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8299-134">C#</span><span class="sxs-lookup"><span data-stu-id="a8299-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8299-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8299-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8299-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8299-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a8299-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8299-137">Response</span></span>

> <span data-ttu-id="a8299-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8299-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
