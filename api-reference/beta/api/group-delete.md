---
title: Excluir grupo-API do Microsoft Graph
description: Descreve o método Delete do recurso de grupo (entidade) da API do Microsoft Graph (REST).
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6eec50e07253bd380c6253f2aad7105f29ee7474
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123794"
---
# <a name="delete-group"></a><span data-ttu-id="8a642-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="8a642-103">Delete group</span></span>

<span data-ttu-id="8a642-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a642-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a642-105">Exclui um grupo.</span><span class="sxs-lookup"><span data-stu-id="8a642-105">Deletes a group.</span></span>  

<span data-ttu-id="8a642-106">Quando excluídos, os grupos do Office 365 são movidos para um contêiner temporário e podem ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="8a642-106">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="8a642-107">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="8a642-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="8a642-108">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8a642-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="8a642-109">Isso se aplica apenas aos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8a642-109">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a642-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a642-110">Permissions</span></span>

<span data-ttu-id="8a642-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a642-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a642-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a642-113">Permission type</span></span>      | <span data-ttu-id="8a642-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a642-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a642-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a642-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8a642-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a642-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="8a642-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a642-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a642-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a642-118">Not supported.</span></span>    |
|<span data-ttu-id="8a642-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a642-119">Application</span></span> | <span data-ttu-id="8a642-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a642-120">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a642-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a642-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a642-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a642-122">Request headers</span></span>

| <span data-ttu-id="8a642-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8a642-123">Name</span></span>       | <span data-ttu-id="8a642-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a642-124">Type</span></span> | <span data-ttu-id="8a642-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a642-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a642-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a642-126">Authorization</span></span>  | <span data-ttu-id="8a642-127">string</span><span class="sxs-lookup"><span data-stu-id="8a642-127">string</span></span>  | <span data-ttu-id="8a642-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a642-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a642-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a642-130">Request body</span></span>

<span data-ttu-id="8a642-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a642-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a642-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a642-132">Response</span></span>

<span data-ttu-id="8a642-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a642-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a642-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a642-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a642-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a642-136">Request</span></span>

<span data-ttu-id="8a642-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a642-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a642-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a642-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```
# <a name="c"></a>[<span data-ttu-id="8a642-139">C#</span><span class="sxs-lookup"><span data-stu-id="8a642-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a642-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a642-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a642-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a642-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a642-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a642-142">Response</span></span>

<span data-ttu-id="8a642-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a642-143">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
