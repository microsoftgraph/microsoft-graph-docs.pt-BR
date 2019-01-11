---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 11b06eac57d0850e8df5233bba47966f6b7932d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886636"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="82db5-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="82db5-103">Add directory role member</span></span>

<span data-ttu-id="82db5-104">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="82db5-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="82db5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="82db5-105">Permissions</span></span>
<span data-ttu-id="82db5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82db5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82db5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82db5-108">Permission type</span></span>      | <span data-ttu-id="82db5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82db5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82db5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82db5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82db5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82db5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82db5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82db5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82db5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82db5-113">Not supported.</span></span>    |
|<span data-ttu-id="82db5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82db5-114">Application</span></span> | <span data-ttu-id="82db5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82db5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82db5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82db5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="82db5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82db5-117">Request headers</span></span>
| <span data-ttu-id="82db5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="82db5-118">Name</span></span>       | <span data-ttu-id="82db5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="82db5-119">Type</span></span> | <span data-ttu-id="82db5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="82db5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82db5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="82db5-121">Authorization</span></span>  | <span data-ttu-id="82db5-122">string</span><span class="sxs-lookup"><span data-stu-id="82db5-122">string</span></span>  | <span data-ttu-id="82db5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82db5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82db5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82db5-125">Content-Type</span></span>  | <span data-ttu-id="82db5-126">string</span><span class="sxs-lookup"><span data-stu-id="82db5-126">string</span></span>  | <span data-ttu-id="82db5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82db5-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82db5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82db5-128">Request body</span></span>
<span data-ttu-id="82db5-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="82db5-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="82db5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="82db5-130">Response</span></span>

<span data-ttu-id="82db5-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82db5-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82db5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82db5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82db5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82db5-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="82db5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="82db5-134">Response</span></span>
<span data-ttu-id="82db5-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="82db5-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
