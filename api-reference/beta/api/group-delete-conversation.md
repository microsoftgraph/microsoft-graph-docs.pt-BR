---
title: Excluir conversa
description: Excluir um objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8eda987cb30d4ffbdda32bf9df750c58f3b77f37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859056"
---
# <a name="delete-conversation"></a><span data-ttu-id="634aa-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="634aa-103">Delete conversation</span></span>

> <span data-ttu-id="634aa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="634aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="634aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="634aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="634aa-106">Excluir um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="634aa-106">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="634aa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="634aa-107">Permissions</span></span>
<span data-ttu-id="634aa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="634aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="634aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="634aa-110">Permission type</span></span>      | <span data-ttu-id="634aa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="634aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="634aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="634aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="634aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="634aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="634aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="634aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="634aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="634aa-115">Not supported.</span></span>    |
|<span data-ttu-id="634aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="634aa-116">Application</span></span> | <span data-ttu-id="634aa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="634aa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="634aa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="634aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="634aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="634aa-119">Request headers</span></span>
| <span data-ttu-id="634aa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="634aa-120">Name</span></span>       | <span data-ttu-id="634aa-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="634aa-121">Type</span></span> | <span data-ttu-id="634aa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="634aa-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="634aa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="634aa-123">Authorization</span></span>  | <span data-ttu-id="634aa-124">string</span><span class="sxs-lookup"><span data-stu-id="634aa-124">string</span></span>  | <span data-ttu-id="634aa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="634aa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="634aa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="634aa-127">Request body</span></span>
<span data-ttu-id="634aa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="634aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="634aa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="634aa-129">Response</span></span>
<span data-ttu-id="634aa-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="634aa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="634aa-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="634aa-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="634aa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="634aa-133">Request</span></span>
<span data-ttu-id="634aa-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="634aa-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="634aa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="634aa-135">Response</span></span>
<span data-ttu-id="634aa-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="634aa-136">The following is an example of the response.</span></span> 
><span data-ttu-id="634aa-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="634aa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
