---
title: Excluir uma configuração de grupo
description: Excluir uma configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 55a9c1d51e03eaea785d351c0700803915b2fe33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839064"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="bc868-103">Excluir uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="bc868-103">Delete a group setting</span></span>

<span data-ttu-id="bc868-104">Excluir uma configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc868-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc868-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc868-105">Permissions</span></span>

<span data-ttu-id="bc868-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bc868-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc868-108">Permission type</span></span>      | <span data-ttu-id="bc868-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc868-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc868-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc868-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc868-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc868-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc868-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc868-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc868-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc868-113">Not supported.</span></span>    |
|<span data-ttu-id="bc868-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc868-114">Application</span></span> | <span data-ttu-id="bc868-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc868-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc868-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc868-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="bc868-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc868-117">Request headers</span></span>

| <span data-ttu-id="bc868-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bc868-118">Name</span></span> | <span data-ttu-id="bc868-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc868-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bc868-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc868-120">Authorization</span></span>  | <span data-ttu-id="bc868-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc868-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc868-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc868-123">Content-Type</span></span>  | <span data-ttu-id="bc868-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc868-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc868-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc868-125">Request body</span></span>
<span data-ttu-id="bc868-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc868-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc868-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc868-127">Response</span></span>

<span data-ttu-id="bc868-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc868-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc868-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc868-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc868-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc868-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="bc868-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc868-132">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
