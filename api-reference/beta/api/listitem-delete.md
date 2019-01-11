---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.openlocfilehash: 71be680ae2d29d083d06c9d18aa79675ebdd01dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849277"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="ac69f-102">Excluir um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="ac69f-102">Delete an item from a list</span></span>

> <span data-ttu-id="ac69f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac69f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac69f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac69f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac69f-105">Remover um item de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="ac69f-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="ac69f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac69f-107">Permissions</span></span>

<span data-ttu-id="ac69f-108">Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="ac69f-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="ac69f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac69f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac69f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac69f-111">Permission type</span></span>      | <span data-ttu-id="ac69f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac69f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac69f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac69f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ac69f-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac69f-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac69f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac69f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac69f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac69f-116">Not supported.</span></span>    |
|<span data-ttu-id="ac69f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac69f-117">Application</span></span> | <span data-ttu-id="ac69f-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac69f-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac69f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac69f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ac69f-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ac69f-120">Optional request headers</span></span>

| <span data-ttu-id="ac69f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ac69f-121">Name</span></span>       | <span data-ttu-id="ac69f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac69f-122">Value</span></span> | <span data-ttu-id="ac69f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac69f-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="ac69f-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="ac69f-124">_if-match_</span></span> | <span data-ttu-id="ac69f-125">etag</span><span class="sxs-lookup"><span data-stu-id="ac69f-125">etag</span></span>  | <span data-ttu-id="ac69f-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="ac69f-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="ac69f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac69f-127">Request body</span></span>

<span data-ttu-id="ac69f-128">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="ac69f-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="ac69f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac69f-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="ac69f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac69f-130">Response</span></span>

<span data-ttu-id="ac69f-131">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="ac69f-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
