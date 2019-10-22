---
title: Adicionar membro
description: Adicione um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação de **membros**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: caa00e74298eb7d744412ffdc85298d804ef615d
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621354"
---
# <a name="add-member"></a><span data-ttu-id="8a28f-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="8a28f-103">Add member</span></span>
<span data-ttu-id="8a28f-104">Adicione um membro a um grupo do Office 365 ou a um grupo de segurança através da propriedade de navegação de **membros**.</span><span class="sxs-lookup"><span data-stu-id="8a28f-104">Add a member to an Office 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="8a28f-105">É possível adicionar usuários, contatos organizacionais ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="8a28f-105">You can add users or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="8a28f-106">É possível adicionar somente usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8a28f-106">You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a28f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a28f-107">Permissions</span></span>
<span data-ttu-id="8a28f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a28f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a28f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a28f-110">Permission type</span></span>      | <span data-ttu-id="8a28f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a28f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a28f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a28f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a28f-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a28f-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a28f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a28f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a28f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a28f-115">Not supported.</span></span>    |
|<span data-ttu-id="8a28f-116">Application</span><span class="sxs-lookup"><span data-stu-id="8a28f-116">Application</span></span> | <span data-ttu-id="8a28f-117">Group.ReadWrite.All e Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a28f-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a28f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a28f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8a28f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a28f-119">Request headers</span></span>
| <span data-ttu-id="8a28f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a28f-120">Header</span></span>       | <span data-ttu-id="8a28f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8a28f-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8a28f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a28f-122">Authorization</span></span>  | <span data-ttu-id="8a28f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a28f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a28f-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="8a28f-125">Content-type</span></span>   | <span data-ttu-id="8a28f-126">appication/json.</span><span class="sxs-lookup"><span data-stu-id="8a28f-126">appication/json.</span></span> <span data-ttu-id="8a28f-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a28f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a28f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a28f-128">Request body</span></span>
<span data-ttu-id="8a28f-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="8a28f-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8a28f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a28f-130">Response</span></span>
<span data-ttu-id="8a28f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a28f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a28f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a28f-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8a28f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a28f-134">Request</span></span>
<span data-ttu-id="8a28f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a28f-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8a28f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a28f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a28f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a28f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a28f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a28f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="8a28f-139">C#</span><span class="sxs-lookup"><span data-stu-id="8a28f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8a28f-140">Java</span><span class="sxs-lookup"><span data-stu-id="8a28f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8a28f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a28f-141">Response</span></span>
<span data-ttu-id="8a28f-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a28f-142">The following is an example of the response.</span></span>

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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
