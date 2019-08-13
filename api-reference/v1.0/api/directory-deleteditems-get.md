---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd511a85349012dbd8ea7c5230a7e74cd22be7b9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373851"
---
# <a name="get-deleted-item"></a><span data-ttu-id="f827f-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="f827f-103">Get deleted item</span></span>

<span data-ttu-id="f827f-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="f827f-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f827f-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f827f-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="f827f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f827f-106">Permissions</span></span>
<span data-ttu-id="f827f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f827f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="f827f-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="f827f-109">For users:</span></span>

|<span data-ttu-id="f827f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f827f-110">Permission type</span></span>      | <span data-ttu-id="f827f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f827f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f827f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f827f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f827f-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f827f-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="f827f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f827f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f827f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f827f-115">Not supported.</span></span> |
|<span data-ttu-id="f827f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f827f-116">Application</span></span> | <span data-ttu-id="f827f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f827f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="f827f-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="f827f-118">For groups:</span></span>

|<span data-ttu-id="f827f-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f827f-119">Permission type</span></span>      | <span data-ttu-id="f827f-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f827f-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f827f-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f827f-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f827f-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f827f-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f827f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f827f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f827f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f827f-124">Not supported.</span></span>    |
|<span data-ttu-id="f827f-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f827f-125">Application</span></span> | <span data-ttu-id="f827f-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f827f-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f827f-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f827f-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f827f-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f827f-128">Optional query parameters</span></span>
<span data-ttu-id="f827f-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f827f-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f827f-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f827f-130">Request headers</span></span>
| <span data-ttu-id="f827f-131">Nome</span><span class="sxs-lookup"><span data-stu-id="f827f-131">Name</span></span>      |<span data-ttu-id="f827f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f827f-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f827f-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="f827f-133">Authorization</span></span>  | <span data-ttu-id="f827f-134">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="f827f-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f827f-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f827f-135">Accept</span></span>  | <span data-ttu-id="f827f-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f827f-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f827f-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f827f-137">Request body</span></span>
<span data-ttu-id="f827f-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f827f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f827f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f827f-139">Response</span></span>

<span data-ttu-id="f827f-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f827f-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f827f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f827f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f827f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f827f-142">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f827f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f827f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f827f-144">C#</span><span class="sxs-lookup"><span data-stu-id="f827f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f827f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f827f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f827f-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f827f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f827f-147">Java</span><span class="sxs-lookup"><span data-stu-id="f827f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f827f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f827f-148">Response</span></span>
<span data-ttu-id="f827f-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f827f-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
