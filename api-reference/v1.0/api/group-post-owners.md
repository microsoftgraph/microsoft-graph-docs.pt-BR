---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
ms.openlocfilehash: 8c879430c78cb1d06150bade842addcb4ba0af38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005334"
---
# <a name="add-group-owner"></a><span data-ttu-id="4589f-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="4589f-104">Add group owner</span></span>
<span data-ttu-id="4589f-p102">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="4589f-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4589f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4589f-107">Permissions</span></span>
<span data-ttu-id="4589f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4589f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4589f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4589f-110">Permission type</span></span>      | <span data-ttu-id="4589f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4589f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4589f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4589f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4589f-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4589f-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4589f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4589f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4589f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4589f-115">Not supported.</span></span>    |
|<span data-ttu-id="4589f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4589f-116">Application</span></span> | <span data-ttu-id="4589f-117">Group.ReadWrite.All e User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4589f-117">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4589f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4589f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4589f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4589f-119">Request headers</span></span>
| <span data-ttu-id="4589f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4589f-120">Name</span></span>       | <span data-ttu-id="4589f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4589f-121">Type</span></span> | <span data-ttu-id="4589f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4589f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4589f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4589f-123">Authorization</span></span>  | <span data-ttu-id="4589f-124">string</span><span class="sxs-lookup"><span data-stu-id="4589f-124">string</span></span>  | <span data-ttu-id="4589f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4589f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4589f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4589f-127">Request body</span></span>
<span data-ttu-id="4589f-128">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="4589f-128">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="4589f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4589f-129">Response</span></span>
<span data-ttu-id="4589f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4589f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4589f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4589f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4589f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4589f-133">Request</span></span>
<span data-ttu-id="4589f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4589f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="4589f-135">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="4589f-135">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="4589f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4589f-136">Response</span></span>
<span data-ttu-id="4589f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4589f-137">The following is an example of the response.</span></span>
><span data-ttu-id="4589f-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4589f-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4589f-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4589f-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
