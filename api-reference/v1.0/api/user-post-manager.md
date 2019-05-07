---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 205e38eefe02fb17e41542bb653e78dd2d621507
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601692"
---
# <a name="assign-a-manager"></a><span data-ttu-id="9f39f-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="9f39f-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f39f-104">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9f39f-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="9f39f-105">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="9f39f-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f39f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f39f-106">Permissions</span></span>
<span data-ttu-id="9f39f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f39f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f39f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f39f-109">Permission type</span></span>      | <span data-ttu-id="9f39f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f39f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f39f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f39f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f39f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f39f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f39f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f39f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f39f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f39f-114">Not supported.</span></span>    |
|<span data-ttu-id="9f39f-115">Application</span><span class="sxs-lookup"><span data-stu-id="9f39f-115">Application</span></span> | <span data-ttu-id="9f39f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f39f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f39f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f39f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9f39f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f39f-118">Request headers</span></span>
| <span data-ttu-id="9f39f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9f39f-119">Name</span></span>       | <span data-ttu-id="9f39f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f39f-120">Type</span></span> | <span data-ttu-id="9f39f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f39f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f39f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f39f-122">Authorization</span></span>  | <span data-ttu-id="9f39f-123">string</span><span class="sxs-lookup"><span data-stu-id="9f39f-123">string</span></span>  | <span data-ttu-id="9f39f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f39f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f39f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f39f-126">Request body</span></span>
<span data-ttu-id="9f39f-127">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="9f39f-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9f39f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f39f-128">Response</span></span>

<span data-ttu-id="9f39f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f39f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f39f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f39f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f39f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f39f-132">Request</span></span>
<span data-ttu-id="9f39f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f39f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="9f39f-134">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="9f39f-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="9f39f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f39f-135">Response</span></span>
<span data-ttu-id="9f39f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f39f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f39f-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9f39f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9f39f-140">Basic</span><span class="sxs-lookup"><span data-stu-id="9f39f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f39f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f39f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
