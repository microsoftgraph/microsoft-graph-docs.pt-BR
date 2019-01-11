---
title: Excluir directoryObject
description: Exclua directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: e291004f13eaf6d0f24750002c8068d3e97b3052
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865190"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="835b6-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="835b6-103">Delete directoryObject</span></span>

> <span data-ttu-id="835b6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="835b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="835b6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="835b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="835b6-106">Exclua directoryObject.</span><span class="sxs-lookup"><span data-stu-id="835b6-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="835b6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="835b6-107">Permissions</span></span>
<span data-ttu-id="835b6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="835b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="835b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="835b6-110">Permission type</span></span>      | <span data-ttu-id="835b6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="835b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="835b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="835b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="835b6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="835b6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="835b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="835b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="835b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="835b6-115">Not supported.</span></span>    |
|<span data-ttu-id="835b6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="835b6-116">Application</span></span> | <span data-ttu-id="835b6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="835b6-117">Not supported.</span></span> |

<span data-ttu-id="835b6-118">**Observação:** Usuários, grupos e contatos são tipos de objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="835b6-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="835b6-119">Como resultado, se você precisar excluir usuários, a seguinte permissão pode e deve ser usada: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="835b6-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="835b6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="835b6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="835b6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="835b6-121">Request headers</span></span>
| <span data-ttu-id="835b6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="835b6-122">Name</span></span>       | <span data-ttu-id="835b6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="835b6-123">Type</span></span> | <span data-ttu-id="835b6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="835b6-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="835b6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="835b6-125">Authorization</span></span>  | <span data-ttu-id="835b6-126">string</span><span class="sxs-lookup"><span data-stu-id="835b6-126">string</span></span>  | <span data-ttu-id="835b6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="835b6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="835b6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="835b6-129">Request body</span></span>
<span data-ttu-id="835b6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="835b6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="835b6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="835b6-131">Response</span></span>

<span data-ttu-id="835b6-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="835b6-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="835b6-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="835b6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="835b6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="835b6-135">Request</span></span>
<span data-ttu-id="835b6-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="835b6-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="835b6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="835b6-137">Response</span></span>
<span data-ttu-id="835b6-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="835b6-138">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
