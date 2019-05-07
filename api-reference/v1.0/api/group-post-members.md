---
title: Adicionar membro
description: Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 2457c12654da11cf54fb503bdf752f4fe60dc021
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613985"
---
# <a name="add-member"></a><span data-ttu-id="23084-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="23084-103">Add member</span></span>
<span data-ttu-id="23084-104">Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.</span><span class="sxs-lookup"><span data-stu-id="23084-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="23084-105">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="23084-105">You can add users or other groups.</span></span> <span data-ttu-id="23084-106">Importante: só é possível adicionar usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="23084-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="23084-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="23084-107">Permissions</span></span>
<span data-ttu-id="23084-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23084-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23084-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23084-110">Permission type</span></span>      | <span data-ttu-id="23084-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23084-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23084-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23084-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23084-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23084-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="23084-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23084-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23084-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23084-115">Not supported.</span></span>    |
|<span data-ttu-id="23084-116">Application</span><span class="sxs-lookup"><span data-stu-id="23084-116">Application</span></span> | <span data-ttu-id="23084-117">Group.ReadWrite.All e Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23084-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23084-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23084-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="23084-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23084-119">Request headers</span></span>
| <span data-ttu-id="23084-120">Nome</span><span class="sxs-lookup"><span data-stu-id="23084-120">Name</span></span>       | <span data-ttu-id="23084-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="23084-121">Type</span></span> | <span data-ttu-id="23084-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="23084-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23084-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23084-123">Authorization</span></span>  | <span data-ttu-id="23084-124">string</span><span class="sxs-lookup"><span data-stu-id="23084-124">string</span></span>  | <span data-ttu-id="23084-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23084-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23084-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23084-127">Request body</span></span>
<span data-ttu-id="23084-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="23084-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="23084-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="23084-129">Response</span></span>
<span data-ttu-id="23084-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23084-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23084-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23084-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="23084-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23084-133">Request</span></span>
<span data-ttu-id="23084-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="23084-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="23084-135">No corpo da solicitação, forneça uma representação JSON da `id` do objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="23084-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="23084-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="23084-136">Response</span></span>
<span data-ttu-id="23084-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23084-137">The following is an example of the response.</span></span>
><span data-ttu-id="23084-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23084-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="23084-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23084-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="23084-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="23084-140">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23084-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="23084-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
