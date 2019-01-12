---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f138be1632c72f8c31eb08fcdaefc50e7affb3e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991528"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="375da-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="375da-103">Add directory role member</span></span>

<span data-ttu-id="375da-104">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="375da-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="375da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="375da-105">Permissions</span></span>
<span data-ttu-id="375da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="375da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="375da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="375da-108">Permission type</span></span>      | <span data-ttu-id="375da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="375da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="375da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="375da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="375da-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="375da-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="375da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="375da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375da-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="375da-113">Not supported.</span></span>    |
|<span data-ttu-id="375da-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="375da-114">Application</span></span> | <span data-ttu-id="375da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="375da-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="375da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="375da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="375da-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="375da-117">Request headers</span></span>
| <span data-ttu-id="375da-118">Nome</span><span class="sxs-lookup"><span data-stu-id="375da-118">Name</span></span>       | <span data-ttu-id="375da-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="375da-119">Type</span></span> | <span data-ttu-id="375da-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="375da-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="375da-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="375da-121">Authorization</span></span>  | <span data-ttu-id="375da-122">string</span><span class="sxs-lookup"><span data-stu-id="375da-122">string</span></span>  | <span data-ttu-id="375da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="375da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="375da-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="375da-125">Content-Type</span></span>  | <span data-ttu-id="375da-126">string</span><span class="sxs-lookup"><span data-stu-id="375da-126">string</span></span>  | <span data-ttu-id="375da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="375da-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="375da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="375da-128">Request body</span></span>
<span data-ttu-id="375da-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="375da-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="375da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="375da-130">Response</span></span>

<span data-ttu-id="375da-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="375da-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="375da-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="375da-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="375da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="375da-133">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="375da-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="375da-134">Response</span></span>
<span data-ttu-id="375da-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="375da-135">Note: The response object shown here may be truncated for brevity.</span></span> 
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
