---
title: Excluir directoryObject
description: Excluir directoryobject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e3d9021a07e028561c45e196bbca62291a5e532e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435042"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="788d0-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="788d0-103">Delete directoryObject</span></span>

<span data-ttu-id="788d0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="788d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="788d0-105">Excluir directoryobject.</span><span class="sxs-lookup"><span data-stu-id="788d0-105">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="788d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="788d0-106">Permissions</span></span>
<span data-ttu-id="788d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="788d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="788d0-109">Permission type</span></span>      | <span data-ttu-id="788d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="788d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="788d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="788d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="788d0-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="788d0-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="788d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="788d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="788d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="788d0-114">Not supported.</span></span>    |
|<span data-ttu-id="788d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="788d0-115">Application</span></span> | <span data-ttu-id="788d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="788d0-116">Not supported.</span></span> |

<span data-ttu-id="788d0-117">**OBSERVAÇÃO:** usuários, grupos e contatos são tipos de objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="788d0-117">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="788d0-118">Como resultado, se você precisar excluir usuários, a permissão a seguir poderá e deve ser usada: user. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="788d0-118">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="788d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="788d0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="788d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="788d0-120">Request headers</span></span>
| <span data-ttu-id="788d0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="788d0-121">Name</span></span>       | <span data-ttu-id="788d0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="788d0-122">Type</span></span> | <span data-ttu-id="788d0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="788d0-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="788d0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="788d0-124">Authorization</span></span>  | <span data-ttu-id="788d0-125">string</span><span class="sxs-lookup"><span data-stu-id="788d0-125">string</span></span>  | <span data-ttu-id="788d0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="788d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="788d0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="788d0-128">Request body</span></span>
<span data-ttu-id="788d0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="788d0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="788d0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="788d0-130">Response</span></span>

<span data-ttu-id="788d0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="788d0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="788d0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="788d0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="788d0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="788d0-134">Request</span></span>
<span data-ttu-id="788d0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="788d0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="788d0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="788d0-136">Response</span></span>
<span data-ttu-id="788d0-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="788d0-137">Here is an example of the response.</span></span> 
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
