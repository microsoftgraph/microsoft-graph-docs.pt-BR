---
title: Excluir directoryObject
description: Excluir directoryobject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8bf24eae152fb31c766f2b395d2c6c37e2c91ddd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326054"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="e8926-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="e8926-103">Delete directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8926-104">Excluir directoryobject.</span><span class="sxs-lookup"><span data-stu-id="e8926-104">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8926-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8926-105">Permissions</span></span>
<span data-ttu-id="e8926-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e8926-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8926-108">Permission type</span></span>      | <span data-ttu-id="e8926-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8926-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8926-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8926-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8926-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8926-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8926-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8926-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8926-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8926-113">Not supported.</span></span>    |
|<span data-ttu-id="e8926-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8926-114">Application</span></span> | <span data-ttu-id="e8926-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8926-115">Not supported.</span></span> |

<span data-ttu-id="e8926-116">**OBSERVAÇÃO:** usuários, grupos e contatos são tipos de objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="e8926-116">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="e8926-117">Como resultado, se você precisar excluir usuários, a permissão a seguir poderá e deve ser usada: user. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8926-117">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="e8926-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8926-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e8926-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8926-119">Request headers</span></span>
| <span data-ttu-id="e8926-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e8926-120">Name</span></span>       | <span data-ttu-id="e8926-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8926-121">Type</span></span> | <span data-ttu-id="e8926-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8926-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8926-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8926-123">Authorization</span></span>  | <span data-ttu-id="e8926-124">string</span><span class="sxs-lookup"><span data-stu-id="e8926-124">string</span></span>  | <span data-ttu-id="e8926-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8926-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8926-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8926-127">Request body</span></span>
<span data-ttu-id="e8926-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8926-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8926-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8926-129">Response</span></span>

<span data-ttu-id="e8926-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8926-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8926-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8926-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8926-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8926-133">Request</span></span>
<span data-ttu-id="e8926-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8926-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="e8926-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8926-135">Response</span></span>
<span data-ttu-id="e8926-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8926-136">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
