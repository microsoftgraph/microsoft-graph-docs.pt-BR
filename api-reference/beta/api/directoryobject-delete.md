---
title: Excluir directoryObject
description: Excluir directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cef22c9deb67d9e1ac7c083fc9e3152bf6c78fa5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436929"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="ea9f8-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="ea9f8-103">Delete directoryObject</span></span>

<span data-ttu-id="ea9f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea9f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea9f8-105">Excluir directoryObject.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-105">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea9f8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea9f8-106">Permissions</span></span>
<span data-ttu-id="ea9f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea9f8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea9f8-109">Permission type</span></span>      | <span data-ttu-id="ea9f8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea9f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea9f8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea9f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea9f8-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea9f8-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea9f8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea9f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea9f8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-114">Not supported.</span></span>    |
|<span data-ttu-id="ea9f8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea9f8-115">Application</span></span> | <span data-ttu-id="ea9f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-116">Not supported.</span></span> |

<span data-ttu-id="ea9f8-117">**OBSERVAÇÃO:** usuários, grupos e contatos são tipos de objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-117">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="ea9f8-118">Como resultado, se você precisar excluir usuários, a seguinte permissão pode e deve ser usada: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9f8-118">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="ea9f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea9f8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ea9f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9f8-120">Request headers</span></span>
| <span data-ttu-id="ea9f8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ea9f8-121">Name</span></span>       | <span data-ttu-id="ea9f8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea9f8-122">Type</span></span> | <span data-ttu-id="ea9f8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea9f8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ea9f8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea9f8-124">Authorization</span></span>  | <span data-ttu-id="ea9f8-125">string</span><span class="sxs-lookup"><span data-stu-id="ea9f8-125">string</span></span>  | <span data-ttu-id="ea9f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea9f8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9f8-128">Request body</span></span>
<span data-ttu-id="ea9f8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea9f8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea9f8-130">Response</span></span>

<span data-ttu-id="ea9f8-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea9f8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea9f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea9f8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9f8-134">Request</span></span>
<span data-ttu-id="ea9f8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="ea9f8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea9f8-136">Response</span></span>
<span data-ttu-id="ea9f8-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea9f8-137">Here is an example of the response.</span></span> 
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


