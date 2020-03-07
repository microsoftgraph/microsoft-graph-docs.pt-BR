---
title: Adicionar membro
description: Adicione um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação de **membros**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6700d5fe6185e15fe016c4ca58219442c60c2a01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516981"
---
# <a name="add-member"></a><span data-ttu-id="eabed-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="eabed-103">Add member</span></span>

<span data-ttu-id="eabed-104">Namespace: microsoft.graph Adicione um membro a um grupo do Office 365 ou a um grupo de segurança através da propriedade de navegação de **membros**.</span><span class="sxs-lookup"><span data-stu-id="eabed-104">Namespace: microsoft.graph Add a member to an Office 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="eabed-105">É possível adicionar usuários, contatos organizacionais ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="eabed-105">You can add users, organizational contacts, or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="eabed-106">Só é possível adicionar usuários aos grupos do Office 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="eabed-106">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="eabed-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eabed-107">Permissions</span></span>
<span data-ttu-id="eabed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eabed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eabed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eabed-110">Permission type</span></span>      | <span data-ttu-id="eabed-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eabed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eabed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eabed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eabed-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eabed-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eabed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eabed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eabed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eabed-115">Not supported.</span></span>    |
|<span data-ttu-id="eabed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eabed-116">Application</span></span> | <span data-ttu-id="eabed-117">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eabed-117">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eabed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eabed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="eabed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eabed-119">Request headers</span></span>
| <span data-ttu-id="eabed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eabed-120">Header</span></span>       | <span data-ttu-id="eabed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eabed-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="eabed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eabed-122">Authorization</span></span>  | <span data-ttu-id="eabed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eabed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eabed-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="eabed-125">Content-type</span></span>   | <span data-ttu-id="eabed-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eabed-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eabed-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eabed-128">Request body</span></span>
<span data-ttu-id="eabed-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="eabed-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="eabed-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eabed-130">Response</span></span>
<span data-ttu-id="eabed-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eabed-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eabed-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eabed-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eabed-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eabed-134">Request</span></span>
<span data-ttu-id="eabed-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eabed-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eabed-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="eabed-136">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="eabed-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eabed-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eabed-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eabed-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="eabed-139">C#</span><span class="sxs-lookup"><span data-stu-id="eabed-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eabed-140">Java</span><span class="sxs-lookup"><span data-stu-id="eabed-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="eabed-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eabed-141">Response</span></span>
<span data-ttu-id="eabed-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eabed-142">The following is an example of the response.</span></span>

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
