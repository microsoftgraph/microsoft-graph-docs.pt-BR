---
title: Recuperar as propriedades de um item excluído recentemente
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c02246e6dccea52e1a973312f2add6cb1232c0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518053"
---
# <a name="get-deleted-item"></a><span data-ttu-id="cc691-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="cc691-103">Get deleted item</span></span>

<span data-ttu-id="cc691-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc691-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc691-105">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="cc691-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="cc691-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="cc691-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc691-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc691-107">Permissions</span></span>
<span data-ttu-id="cc691-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="cc691-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="cc691-110">For applications:</span></span>

|<span data-ttu-id="cc691-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc691-111">Permission type</span></span>      | <span data-ttu-id="cc691-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc691-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc691-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc691-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cc691-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc691-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc691-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc691-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc691-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc691-116">Not supported.</span></span>    |
|<span data-ttu-id="cc691-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc691-117">Application</span></span> | <span data-ttu-id="cc691-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc691-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="cc691-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="cc691-119">For users:</span></span>

|<span data-ttu-id="cc691-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc691-120">Permission type</span></span>      | <span data-ttu-id="cc691-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc691-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc691-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc691-122">Delegated (work or school account)</span></span> | <span data-ttu-id="cc691-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc691-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="cc691-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc691-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc691-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc691-125">Not supported.</span></span> |
|<span data-ttu-id="cc691-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc691-126">Application</span></span> | <span data-ttu-id="cc691-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc691-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="cc691-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="cc691-128">For groups:</span></span>

|<span data-ttu-id="cc691-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc691-129">Permission type</span></span>      | <span data-ttu-id="cc691-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc691-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc691-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc691-131">Delegated (work or school account)</span></span> | <span data-ttu-id="cc691-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc691-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cc691-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc691-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc691-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc691-134">Not supported.</span></span>    |
|<span data-ttu-id="cc691-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc691-135">Application</span></span> | <span data-ttu-id="cc691-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc691-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc691-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc691-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc691-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc691-138">Optional query parameters</span></span>
<span data-ttu-id="cc691-139">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc691-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc691-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc691-140">Request headers</span></span>
| <span data-ttu-id="cc691-141">Nome</span><span class="sxs-lookup"><span data-stu-id="cc691-141">Name</span></span>      |<span data-ttu-id="cc691-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc691-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cc691-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc691-143">Authorization</span></span>  | <span data-ttu-id="cc691-144">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="cc691-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="cc691-145">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc691-145">Accept</span></span>  | <span data-ttu-id="cc691-146">application/json</span><span class="sxs-lookup"><span data-stu-id="cc691-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc691-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc691-147">Request body</span></span>
<span data-ttu-id="cc691-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc691-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc691-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc691-149">Response</span></span>

<span data-ttu-id="cc691-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc691-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc691-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc691-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc691-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc691-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cc691-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc691-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="cc691-154">C#</span><span class="sxs-lookup"><span data-stu-id="cc691-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc691-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc691-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc691-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc691-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc691-157">Java</span><span class="sxs-lookup"><span data-stu-id="cc691-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc691-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc691-158">Response</span></span>
<span data-ttu-id="cc691-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc691-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
