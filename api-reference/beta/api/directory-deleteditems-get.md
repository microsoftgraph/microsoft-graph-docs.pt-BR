---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02e56eac0d0e3ac8b2b0132f321098f0ea45b0de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435448"
---
# <a name="get-deleted-item"></a><span data-ttu-id="1cbe2-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="1cbe2-103">Get deleted item</span></span>

<span data-ttu-id="1cbe2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1cbe2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cbe2-105">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="1cbe2-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="1cbe2-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="1cbe2-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cbe2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cbe2-107">Permissions</span></span>
<span data-ttu-id="1cbe2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cbe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="1cbe2-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="1cbe2-110">For applications:</span></span>

|<span data-ttu-id="1cbe2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cbe2-111">Permission type</span></span>      | <span data-ttu-id="1cbe2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cbe2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1cbe2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cbe2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1cbe2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cbe2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-116">Not supported.</span></span>    |
|<span data-ttu-id="1cbe2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cbe2-117">Application</span></span> | <span data-ttu-id="1cbe2-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cbe2-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="1cbe2-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="1cbe2-119">For users:</span></span>

|<span data-ttu-id="1cbe2-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cbe2-120">Permission type</span></span>      | <span data-ttu-id="1cbe2-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cbe2-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-122">Delegated (work or school account)</span></span> | <span data-ttu-id="1cbe2-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cbe2-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="1cbe2-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cbe2-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-125">Not supported.</span></span> |
|<span data-ttu-id="1cbe2-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cbe2-126">Application</span></span> | <span data-ttu-id="1cbe2-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbe2-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="1cbe2-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="1cbe2-128">For groups:</span></span>

|<span data-ttu-id="1cbe2-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cbe2-129">Permission type</span></span>      | <span data-ttu-id="1cbe2-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cbe2-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-131">Delegated (work or school account)</span></span> | <span data-ttu-id="1cbe2-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cbe2-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1cbe2-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cbe2-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cbe2-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-134">Not supported.</span></span>    |
|<span data-ttu-id="1cbe2-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cbe2-135">Application</span></span> | <span data-ttu-id="1cbe2-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbe2-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cbe2-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cbe2-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cbe2-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1cbe2-138">Optional query parameters</span></span>
<span data-ttu-id="1cbe2-139">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cbe2-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cbe2-140">Request headers</span></span>
| <span data-ttu-id="1cbe2-141">Nome</span><span class="sxs-lookup"><span data-stu-id="1cbe2-141">Name</span></span>      |<span data-ttu-id="1cbe2-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cbe2-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1cbe2-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cbe2-143">Authorization</span></span>  | <span data-ttu-id="1cbe2-144">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="1cbe2-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="1cbe2-145">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1cbe2-145">Accept</span></span>  | <span data-ttu-id="1cbe2-146">application/json</span><span class="sxs-lookup"><span data-stu-id="1cbe2-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cbe2-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cbe2-147">Request body</span></span>
<span data-ttu-id="1cbe2-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cbe2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cbe2-149">Response</span></span>

<span data-ttu-id="1cbe2-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1cbe2-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cbe2-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cbe2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cbe2-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1cbe2-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cbe2-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="1cbe2-154">C#</span><span class="sxs-lookup"><span data-stu-id="1cbe2-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cbe2-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cbe2-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cbe2-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cbe2-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1cbe2-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cbe2-157">Response</span></span>
<span data-ttu-id="1cbe2-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cbe2-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
