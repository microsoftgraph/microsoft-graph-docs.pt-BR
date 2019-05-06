---
title: Excluir grupo-API do Microsoft Graph
description: Descreve o método Delete do recurso de grupo (entidade) da API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 686c8f55a1b617c3e26f7fbcf6e789fe6ddee790
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593215"
---
# <a name="delete-group"></a><span data-ttu-id="17d84-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="17d84-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17d84-104">Exclui um grupo.</span><span class="sxs-lookup"><span data-stu-id="17d84-104">Deletes a group.</span></span>  

<span data-ttu-id="17d84-105">Quando excluídos, os grupos do Office 365 são movidos para um contêiner temporário e podem ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="17d84-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="17d84-106">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="17d84-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="17d84-107">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="17d84-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="17d84-108">Isso se aplica apenas aos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="17d84-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="17d84-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="17d84-109">Permissions</span></span>

<span data-ttu-id="17d84-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17d84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17d84-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17d84-112">Permission type</span></span>      | <span data-ttu-id="17d84-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17d84-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17d84-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17d84-114">Delegated (work or school account)</span></span> | <span data-ttu-id="17d84-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d84-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="17d84-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17d84-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17d84-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17d84-117">Not supported.</span></span>    |
|<span data-ttu-id="17d84-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17d84-118">Application</span></span> | <span data-ttu-id="17d84-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d84-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17d84-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17d84-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="17d84-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17d84-121">Request headers</span></span>

| <span data-ttu-id="17d84-122">Nome</span><span class="sxs-lookup"><span data-stu-id="17d84-122">Name</span></span>       | <span data-ttu-id="17d84-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d84-123">Type</span></span> | <span data-ttu-id="17d84-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d84-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17d84-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="17d84-125">Authorization</span></span>  | <span data-ttu-id="17d84-126">string</span><span class="sxs-lookup"><span data-stu-id="17d84-126">string</span></span>  | <span data-ttu-id="17d84-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17d84-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17d84-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17d84-129">Request body</span></span>

<span data-ttu-id="17d84-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17d84-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17d84-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="17d84-131">Response</span></span>

<span data-ttu-id="17d84-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17d84-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17d84-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17d84-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="17d84-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17d84-135">Request</span></span>

<span data-ttu-id="17d84-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17d84-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="17d84-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="17d84-137">Response</span></span>

<span data-ttu-id="17d84-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17d84-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="17d84-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="17d84-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="17d84-140">Basic</span><span class="sxs-lookup"><span data-stu-id="17d84-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17d84-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17d84-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
