---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: a788d9b7ed6b71163bb1b189681cdf7c5fee7575
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850978"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="34624-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="34624-103">Remove directory role member</span></span>

<span data-ttu-id="34624-104">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="34624-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="34624-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34624-105">Permissions</span></span>

<span data-ttu-id="34624-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="34624-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34624-108">Permission type</span></span>      | <span data-ttu-id="34624-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34624-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34624-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34624-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34624-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="34624-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="34624-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34624-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34624-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34624-113">Not supported.</span></span>    |
|<span data-ttu-id="34624-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34624-114">Application</span></span> | <span data-ttu-id="34624-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34624-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34624-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34624-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="34624-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34624-117">Request headers</span></span>

| <span data-ttu-id="34624-118">Nome</span><span class="sxs-lookup"><span data-stu-id="34624-118">Name</span></span>       | <span data-ttu-id="34624-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="34624-119">Type</span></span> | <span data-ttu-id="34624-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="34624-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34624-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34624-121">Authorization</span></span>  | <span data-ttu-id="34624-122">string</span><span class="sxs-lookup"><span data-stu-id="34624-122">string</span></span>  | <span data-ttu-id="34624-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34624-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34624-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34624-125">Request body</span></span>

<span data-ttu-id="34624-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34624-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34624-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="34624-127">Response</span></span>

<span data-ttu-id="34624-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34624-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34624-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34624-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="34624-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34624-131">Request</span></span>

<span data-ttu-id="34624-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34624-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="34624-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="34624-133">Response</span></span>

<span data-ttu-id="34624-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34624-134">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
