---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0c218351d9c8e556220630f150f5e43592c626f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956135"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="f99e6-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="f99e6-103">Remove directory role member</span></span>

> <span data-ttu-id="f99e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f99e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f99e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f99e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f99e6-106">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="f99e6-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="f99e6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f99e6-107">Permissions</span></span>

<span data-ttu-id="f99e6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f99e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f99e6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f99e6-110">Permission type</span></span>      | <span data-ttu-id="f99e6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f99e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f99e6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f99e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f99e6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f99e6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f99e6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f99e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f99e6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f99e6-115">Not supported.</span></span>    |
|<span data-ttu-id="f99e6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99e6-116">Application</span></span> | <span data-ttu-id="f99e6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f99e6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f99e6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f99e6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f99e6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f99e6-119">Request headers</span></span>

| <span data-ttu-id="f99e6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f99e6-120">Name</span></span>       | <span data-ttu-id="f99e6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f99e6-121">Type</span></span> | <span data-ttu-id="f99e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f99e6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f99e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f99e6-123">Authorization</span></span>  | <span data-ttu-id="f99e6-124">string</span><span class="sxs-lookup"><span data-stu-id="f99e6-124">string</span></span>  | <span data-ttu-id="f99e6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f99e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f99e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f99e6-127">Request body</span></span>

<span data-ttu-id="f99e6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f99e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f99e6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f99e6-129">Response</span></span>

<span data-ttu-id="f99e6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f99e6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99e6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f99e6-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f99e6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f99e6-133">Request</span></span>

<span data-ttu-id="f99e6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f99e6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="f99e6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f99e6-135">Response</span></span>

<span data-ttu-id="f99e6-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f99e6-136">Here is an example of the response.</span></span> 
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
