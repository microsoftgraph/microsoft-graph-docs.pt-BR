---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ab48aa46fcdb35418f891d6290f6fc8e5d214f2
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287763"
---
# <a name="get-deleted-item"></a><span data-ttu-id="06957-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="06957-103">Get deleted item</span></span>

<span data-ttu-id="06957-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06957-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06957-105">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="06957-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="06957-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="06957-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="06957-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="06957-107">Permissions</span></span>
<span data-ttu-id="06957-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="06957-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="06957-110">For applications:</span></span>

|<span data-ttu-id="06957-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06957-111">Permission type</span></span>      | <span data-ttu-id="06957-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06957-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06957-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06957-113">Delegated (work or school account)</span></span> | <span data-ttu-id="06957-114">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="06957-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06957-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06957-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06957-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06957-116">Not supported.</span></span>    |
|<span data-ttu-id="06957-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06957-117">Application</span></span> | <span data-ttu-id="06957-118">Application. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="06957-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="06957-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="06957-119">For users:</span></span>

|<span data-ttu-id="06957-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06957-120">Permission type</span></span>      | <span data-ttu-id="06957-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06957-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06957-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06957-122">Delegated (work or school account)</span></span> | <span data-ttu-id="06957-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06957-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="06957-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06957-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06957-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06957-125">Not supported.</span></span> |
|<span data-ttu-id="06957-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06957-126">Application</span></span> | <span data-ttu-id="06957-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06957-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="06957-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="06957-128">For groups:</span></span>

|<span data-ttu-id="06957-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06957-129">Permission type</span></span>      | <span data-ttu-id="06957-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06957-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06957-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06957-131">Delegated (work or school account)</span></span> | <span data-ttu-id="06957-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06957-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="06957-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06957-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06957-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06957-134">Not supported.</span></span>    |
|<span data-ttu-id="06957-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06957-135">Application</span></span> | <span data-ttu-id="06957-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06957-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06957-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06957-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06957-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06957-138">Optional query parameters</span></span>
<span data-ttu-id="06957-139">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06957-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06957-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06957-140">Request headers</span></span>
| <span data-ttu-id="06957-141">Nome</span><span class="sxs-lookup"><span data-stu-id="06957-141">Name</span></span>      |<span data-ttu-id="06957-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="06957-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06957-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="06957-143">Authorization</span></span>  | <span data-ttu-id="06957-144">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="06957-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="06957-145">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06957-145">Accept</span></span>  | <span data-ttu-id="06957-146">application/json</span><span class="sxs-lookup"><span data-stu-id="06957-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="06957-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06957-147">Request body</span></span>
<span data-ttu-id="06957-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06957-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06957-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="06957-149">Response</span></span>

<span data-ttu-id="06957-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06957-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06957-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06957-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06957-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06957-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="06957-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="06957-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="06957-154">C#</span><span class="sxs-lookup"><span data-stu-id="06957-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06957-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06957-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06957-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06957-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06957-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="06957-157">Response</span></span>
<span data-ttu-id="06957-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06957-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
