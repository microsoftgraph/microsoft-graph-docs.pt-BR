---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e33dc95d60e56c0f2796f5eb9c3aa88b343d8634
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041187"
---
# <a name="add-group-owner"></a><span data-ttu-id="ab314-103">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="ab314-103">Add group owner</span></span>

<span data-ttu-id="ab314-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab314-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab314-105">Adicione um usuário ou diretor de serviço aos proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="ab314-105">Add a user or service principal to the group's owners.</span></span> <span data-ttu-id="ab314-106">Os proprietários são um conjunto de usuários ou os diretores de serviço que têm permissão para modificar o objeto do grupo.</span><span class="sxs-lookup"><span data-stu-id="ab314-106">The owners are a set of users or service principals who are allowed to modify the group object.</span></span>

><span data-ttu-id="ab314-107">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ab314-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="ab314-108">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="ab314-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ab314-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab314-109">Permissions</span></span>
<span data-ttu-id="ab314-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab314-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab314-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab314-112">Permission type</span></span>      | <span data-ttu-id="ab314-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab314-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab314-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab314-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ab314-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab314-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab314-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab314-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab314-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab314-117">Not supported.</span></span>    |
|<span data-ttu-id="ab314-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab314-118">Application</span></span> | <span data-ttu-id="ab314-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab314-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab314-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab314-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ab314-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab314-121">Request headers</span></span>
| <span data-ttu-id="ab314-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ab314-122">Name</span></span>       | <span data-ttu-id="ab314-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab314-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab314-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab314-124">Authorization</span></span>  | <span data-ttu-id="ab314-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab314-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab314-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="ab314-127">Content-type</span></span> | <span data-ttu-id="ab314-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab314-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab314-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab314-130">Request body</span></span>
<span data-ttu-id="ab314-131">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ab314-131">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ab314-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab314-132">Response</span></span>
<span data-ttu-id="ab314-133">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ab314-133">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ab314-134">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab314-134">It does not return anything in the response body.</span></span> <span data-ttu-id="ab314-135">Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="ab314-135">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="ab314-136">Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.</span><span class="sxs-lookup"><span data-stu-id="ab314-136">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="example"></a><span data-ttu-id="ab314-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab314-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ab314-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab314-138">Request</span></span>
<span data-ttu-id="ab314-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab314-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab314-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab314-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="ab314-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab314-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab314-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab314-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ab314-143">C#</span><span class="sxs-lookup"><span data-stu-id="ab314-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab314-144">Java</span><span class="sxs-lookup"><span data-stu-id="ab314-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ab314-145">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ab314-145">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="ab314-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab314-146">Response</span></span>
<span data-ttu-id="ab314-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab314-147">The following is an example of the response.</span></span>
><span data-ttu-id="ab314-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab314-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


